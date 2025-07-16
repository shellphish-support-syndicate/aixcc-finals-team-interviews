# Team Theori's AI Cyber Challenge System - Technical Summary

This transcript details Team Theori's "Robo-Duck" cyber reasoning system (CRS) developed for the DARPA AI Cyber Challenge (AIxCC). Here are the key technical aspects:

## System Architecture

**Core Design**: Single Python process using asyncio with 20-25 remote Docker hosts for distributed compute. This centralized approach allows easy inter-component communication and shared state management.

**LLM-Heavy Approach**: Unlike other teams that augmented traditional fuzzing with AI, Theori went "LLM-first" - their system can find bugs effectively even with fuzzing disabled, though they retain it as a component.

## Technical Workflow

**Initial Processing**: When a new repository arrives, the system:
- Builds projects multiple ways (different sanitizers, coverage instrumentation, debug info)
- Uses both Clang and Joern for static analysis
- Extracts source information and CFGs

**Bug Discovery Pipeline**:
1. **Static Analysis**: Uses Infer plus custom LLM-based static analysis on every line of code
2. **Candidate Generation**: Produces thousands of potential vulnerabilities per project
3. **False Positive Filtering**: Two-stage process using LLM classifiers and analysis agents
4. **High-Signal Output**: Achieves ~50% false positive rate (vs 99%+ from raw static analysis)

## Agent Architecture

The system contains **~12 specialized agents**, each with narrow, well-defined tasks:

### Core Agents
- **Diff Agent**: Analyzes code diffs for delta-mode tasks
- **Vuln Analyzer**: Filters and annotates vulnerability candidates with high precision
- **POV Producer**: Writes Python code to generate binary inputs that trigger vulnerabilities
- **Harness Input Encoder/Decoder**: Abstracts binary formats into semantic representations
- **Patcher Agent**: Creates minimal patches with sophisticated diff handling
- **Debug Agent**: Uses GDB/JDB to inspect runtime behavior
- **Branch Flipper**: LLM-based "driller" that helps fuzzing get unstuck by flipping execution paths

### Key Design Principles
- Agents don't have terminal access (too open-ended)
- Limited tool sets: read-definition, find-references, minimal source reading
- Extensive guard rails and baby-proofing
- Feedback loops between components

## Models and Performance

**Model Usage**: 
- Multiple models run in parallel (Sonnet 3.5, Sonnet 4, O1-03)
- Budget allocation system to prevent early exhaustion
- Different models for different tasks (cheaper models for classification, expensive ones for complex reasoning)

**Performance Observations**:
- Clear improvements with better models (e.g., 5% to 90% success rate when upgrading models)
- O1-03 became favorite after price reduction
- ~20,000 lines of Python code, 2,000 lines of prompts

## Technical Innovations

**Deduplication**: Uses LLM classifiers with token probabilities to match bug reports to existing vulnerabilities based on root cause analysis.

**Dynamic Programming for Patches**: Custom sequence alignment algorithm to handle LLM-generated diffs, with sanity checks for common errors (like missing curly braces).

**Fuzzing Integration**: POV attempts that fail become fuzzing seeds, creating a feedback loop where LLM guidance helps fuzzing reach deeper code paths.

## Strategy and Scoring

**Submission Logic**: 
- Immediate submission of bugs with POVs
- 30-45 minute delay for patches without POVs  
- 2:1 ratio of patches without POVs to patches with POVs (risk management)
- Special handling for diff-mode challenges (higher confidence)

**Game Theory**: Unlike the original Cyber Grand Challenge's complex attack-defense dynamics, AIxCC's simpler scoring allowed focus on bug discovery rather than strategic timing.

## Key Technical Insights

1. **LLM Specialization**: Narrow, task-specific agents with limited tools work better than general-purpose agents
2. **False Positive Management**: The two-stage filtering (classifier + analyzer agent) was identified as their potential "secret sauce"
3. **Multi-Modal Integration**: Successful combination of static analysis, dynamic testing, and LLM reasoning
4. **Reliability Focus**: Extensive testing and crash recovery mechanisms, though single-process design remains a reliability concern

The system represents a novel approach to automated vulnerability discovery that leverages LLMs' code understanding capabilities while maintaining the precision needed for practical security analysis.