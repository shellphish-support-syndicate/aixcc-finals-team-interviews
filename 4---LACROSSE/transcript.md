# CTF Radio: Team LACROSSE AIxCC Interview Transcript

## Introduction

**Adam:** Hello everyone. Welcome to CTF radio. I'm Adam D and I'm super excited to be here with Yan. Yan, say hi.

**Yan:** Hello hackers. I'm also very excited. This is going to be an interesting chat - the first of these we've done where I'm coming in close to blind.

**Adam:** Wait, you're saying you've done prep work for the rest of these episodes we've done?

**Yan:** You know, 

**Adam:** Coz I feel like you just show up and talk and then leave, and then I do the pre-stuff and the post stuff.

**Yan:** You know, I take on a more advisory role.

**Adam:** See, that's the wrong tack to take here. Here, You should say you're talent.

**Yan:** But, Adam, Why don't you introduce, for those joining mid-season, let me talk about what the goal of the season is and why I'm kind of coming in blind.

**Adam:** So yeah, we are doing our fourth AIxCC team interview. We are after the final submission, so all the teams have submitted their AIxCC cyber reasoning systems. We're still before knowing the results, and we've actually crossed the midway point - we now have over half the teams that have done interviews with us. So hopefully we'll be able to apply that peer pressure to everyone else and make sure that we can capture these stories from the teams.

If you are listening for the very first time and you want some background on the AI cyber competition, please listen to one of our previous episodes. I think the first AIxCC episode where we talk with Shellphish discusses the final competition and all the components. That way what we can really do here is dig in with our guests and hear about their team and their CRS.

**Yan:** Speaking of this, our guests today are team LACROSSE. For me personally, a bit of a dark horse in the AIxCC. You know, the previous people that we have interviewed - it's not that we have AIxCC hangouts because obviously they were the enemy until late June. But you know, we've collaborated on other things. I'm very excited for team LACROSSE to talk to you guys here because I think I learned a lot and hopefully the audience will learn a lot.

## Team Introductions

**Adam:** So why don't we have our guests introduce themselves first? We want to go Dave, Mike, and Matt. Is that a good order?

**Dave:** Sure. So I'm Dave Musliner. I'm a team lead for team LACROSSE and I have to tell you that we've been your enemy for longer than you know because we also participated in the Cyber Grand Challenge in the semi-finals, but we did not qualify for the finals. We tied for ninth is the way I like to put it. So we were just barely out of the top seven. But we were playing against you then too.

So yeah, I'm Dave Musliner. All of our team LACROSSE members are employees of Smart Information Flow Technologies or SIFT. So even though Matt's sign-in here doesn't say he's from SIFT, he is. So we're one company team and our history in cyber security goes back a long way. We could talk about that maybe later.

Briefly, my background is as an AI planning and scheduling guy and then moved into autonomous cyber security. We'll talk about all that stuff after Mike introduces himself.

**Mike:** All right. Yeah, also we're all SIFT people. Dave and I have been working together since the 90s on some of the code that was running here. I think we co-developed back then the first generation of this agent-based infrastructure that became a CRS and also has become other interesting research projects at SIFT.

So my background is in that AI planning and scheduling, which you know becomes building agents, building reliable secure software, and then turning it on itself and saying "hey, what's not so reliable and secure about this software?"

**Adam:** Wow, very cool, Matt?
**Matt:** Yeah, I'm Matt McClure. I'm at SIFT too despite my lack of label there. I guess I'm kind of generally the non-conformist here. I didn't mean to be, but I'm missing the shirt too. So yeah, I'm learning something about myself.

So I joined SIFT later than these two after graduating from my grad program in 2019. At SIFT, I've been doing all sorts of things. My background in grad school was in AI and computer science and actually had a lot of exposure to Lisp there too. So I was luckily able to come into this architecture without too much ramp up. And yeah, at SIFT have gotten to do all sorts of stuff with novelty detection and more recently using these LLM pipelines and all sorts of different things that have contributed in various ways to the work on LACROSSE.

**Adam:** Nice. All right, so Matt, you can maybe tell us and be honest because I'm slightly worried about what Dave said. So this isn't like some villain origin story, right? Where this is where they confront Yan about the CGC and then now it's time to exact their revenge?

**Matt:** Yeah, no, I like to think we're the heroes, but this is not the first time I've heard us referred to as the dark horse either. So I think that's interesting. We're like maybe unlikely heroes or anti-heroes or something.

**Adam:** Yeah, I think that's great. And I think that's exactly what we're trying to do here - be able to get to know each other better and know each other's systems, even just among the competitors. Because I think that is really important because like you said, we are working in this space. We've done a lot of cool stuff and we want to learn from each other - we're academics at heart. We want to learn from the cool stuff that everyone's doing.

## The Lisp Codebase Revelation

**Dave:** Well, Mike and Matt actually revealed early some of our secret sauce, which is our enormous Lisp codebase - a massively scalable multi-agent system that dates way back, let's just say. And we have certain individuals working on that codebase who not infrequently tell me that they ran into a comment or a commit message that was done before they were born. And that's always kind of an interesting phenomenon.

**Yan:** This is incredible. I obviously we're all latching on to this right away because so far it's all been Python this and you know, children throughout the teams writing in Python. But now it's very interesting - a massive Lisp agentic framework. I'm super excited to hear about this.

**Adam:** Which makes sense, I mean, I'm a secret Lisp head. I've never gotten a chance to use it.

**Yan:** It's not secret.

**Adam:** Okay, I don't know that it's super well known. Like I don't have it on my shirt. It's not just on my website, but yes.

**Yan:** You only have it in a couple of CTF challenges over several years in the World Championships.

**Adam:** Sure. But maybe people just think I'm deranged and that's not like an interest of mine. But it makes sense - like the early AI stuff, like one of the first or second AI waves, a lot of those systems were written in Lisp. So that makes a lot of sense, evolving something kind of from there. So I'm super stoked to dive into this.

## Team Background and Company Structure [7:57](https://youtu.be/uO1LnENZV_4?t=477)

**Adam:** But first, maybe before we dive into the tech, can you give us a background on your team? I think one of the key things that people want to know is like how big are these teams, so that when they're in the audience rooting for LACROSSE, are they rooting for the three people here? Is it a 20-person team? Is it the whole company? I don't know how big the company is. So you can give us like a background - how big, how'd you come together, that kind of thing.

**Dave:** Yeah, I can talk a little bit about that. SIFT is about a 35-people company and we are a very broad research and development organization with a focus on things ranging from cyber security and highly autonomous systems to human interaction, natural language processing, and even things like medical applications of AI and developing among other things, interestingly, like games that have therapeutic impact.

So we have a really broad space of researchers, and about 15 of those researchers have been involved in the AIxCC competition since the very start. That's not quite all the way through - some people were on the team for semi-finals and qualification, and then some people joined afterwards when we had to send those other people off to do other projects. So not a consistent group of people entirely, but I'd say the core group of about 10 people worked those 24-hour days a lot. And then these three people plus two others were on some of what we called our "war zooms" that lasted 22 hours. We were just all on the Zoom channel continuously and hacking like mad, including right up until a few hours before the final submission. That was not the design and the intent, but yeah, it's a very intense process and the team was not huge.

How did we come together? You know, I grabbed every single person who I could at SIFT that was not already completely booked and unwilling to let's say put on one of these t-shirts and become a hacker. So we absorbed a ton of available time and kind of starved other projects to do this big effort.

**Adam:** And this was on your radar from the start, right? Because you guys were one of the small business track winners, right? So right about when it was announced, did you see like "okay yeah, we're going to do this" or did it take some convincing?

**Dave:** No, it was a must bid. We participated in the earlier DARPA Cyber Grand Challenge which has been mentioned in your other podcasts, and that was more than 10 years ago. Many of those people are still at SIFT, and it was an absolute no-brainer to say "hey, there's another contest, we already have all the stuff from Cyber Grand Challenge."

We've been working, by the way, on other projects that followed on from that. So it's not like we took the Cyber Grand Challenge agent, which was called Fuzzbomb, and just dropped it on the floor and never did anything. We had multiple follow-on projects. We've been developing different capabilities in the same multi-agent framework. And so when the cyber AI cyber challenge came across, we were like, "let's go. We are way ahead of everybody except Shellphish."

**Adam:** Well, except they started from scratch. But, you know.

**Yan:** First decision made: let's throw everything out except for the lessons learned. And then the second decision was: let's throw out the lessons learned.

**Adam:** Learn them again. Exactly. Yes. New people are in charge now and they need to learn them again who weren't involved.

**Yan:** That's 100%. It's you know, there's the saying: normal people learn from their mistakes. Wise people learn from the mistakes of others. There's a third kind of person that needs that lesson to get it again.

## Open Source Considerations [11:47](https://www.youtube.com/watch?v=uO1LnENZV_4&t=707s)

**Adam:** And so this is, when you thought about applying for this and competing in this, from the start it was known that you would have to open source your system. Since as you mentioned this is based on stuff that you are using in other projects, did that deter you at all? Were you a little bit hesitant, or how did that impact your decision to go after this?

**Dave:** No, it didn't really make a big difference because we've provided our software to many government customers before. So that's not the same as open sourcing it, but in terms of impacting our ability to make new projects and sell modifications of it - not the same thing, but that hasn't been a problem. And so we hope that even now that it's open sourced, people in the funding agencies, for example, won't say "well, I could get this for free." You know, that's not - we don't sell the same thing over and over. We tell them, we've already got all this, now let's go make it do something new. So I don't think that was a problem.

And since our team basically owns that software and SIFT is not a big organization with a huge bunch of management to convince, we didn't have to talk to anybody about that.

**Adam:** Awesome. Yeah, that's great. And I think that speaks to the benefits of a small business, but also like recognizing the opportunity there, which I think is really awesome.

**Yan:** And the unique position of a research-focused organization with the vision to create a vehicle that you can strap new specializations on. Like that's very cool. We do a little bit of that in the research lab side of what we do. It's cool to hear this existing in other places.

**Ada,:** Yeah. Kind of talking to the team about this, I'm like, "Yeah, but okay, yes, it's open source, but somebody's got to run it." Like there's the source code and then there's getting the beast to run. And those can be two different things.

**Yan:** And on the other side of that, I think after we recorded the previous interview with the previous team, I called Adam. I'm like, "Dude, it feels like there's room for like a CRS orchestration library that the world can build off of because we have all of these different approaches, different solutions." Maybe that'll be something. Maybe Lisp will come back.

**Adam:** It never left. Aren't you listening? It never left. Exactly.

**Yan:** So far it's all been Python this, Python that.

**Adam:** Only in your head, man.

## System Architecture Overview [14:13](https://youtu.be/uO1LnENZV_4?t=853)

**Adam:** Cool. Okay, so this is great. So now, first question: What's the CRS's name? Is it also called LACROSSE?

**Dave:** It is. Yeah, that's basically why it's not called SIFT. We always have to have a system name we call it or sysname. And so our first instinct was, yeah, what can we name the thing? Fuzzbomb for Cyber Grand Challenge was actually a combination of an earlier system called Fuzzbuster with a University of Minnesota product called Fuzzball, and we didn't feel like we could take those two and quite put them together, so we came up with Fuzzbomb. And then we decided this thing was going to do a lot more than fuzzing and it was going to involve large language models in particular, so the L at the beginning is some acronym that starts with large language...

**Adam:** Nice.

**Mike:** Yeah, we really did our homework there on knowing how to expand our own acronym.

**Dave:** It stands for LLM plus AI Cyber Reasoning Security System. I found it. 

**Adam:** Hey, nice. There you go.

**Yan:** Naming these things is always super tricky. And you guys built in - you had the same team name as your CRS name, right? Which makes it complicated because then you have to stick with it. Shellphish, we didn't talk about this in the Shellphish interview, but Shellphish had to put a name in the proposal.

**Yan:** Yeah. What was the original name?

**Adam:** It was MechAIPhish

**Yan:** Because Mechanical Phish was our CGC entry, and then ARTIPHISHELL came up later. 

**Adam:** I want to believe the students came up with that, but it may have been an LLM. I can't remember for certain.

**Yan:** This is interesting because there'll be two directions that the world may go, right? LACROSSE may become synonymous as the winner of the AIxCC with cyber security mastery, and then everyone starts having sports themes, right? So then suddenly you see a generation of systems that are like I don't know, Field Goal or...

**Adam:** This is really tapping the bottom of Yan's sports knowledge.

**Yan:** It's out of my league pretty badly, you know. Out of my wheelhouse. Pretty badly.

**Adam:** Out of my league - that's also a sports term.

**Yan:** There you go.

## High-Level CRS Architecture [16:45](https://youtu.be/uO1LnENZV_4?t=1005)

**Adam:** Great. Cool. So speaking of LACROSSE, can somebody give us like the high-level, 10,000-foot view of your CRS? Like what's kind of roughly the shape? How does it look at the high level?

**Dave:** Yeah. So we divided up the questions that you suggested might come up. So I'm going to tackle the really high-level stuff, and Mike's going to tell you what happens really when things come in and the problem solving starts to work, and then Matt's going to tell you all the magic about the large language model interactions.

Handwaving at the 10,000-foot agent level, this is an architecture dating to the dark ages where individual agents all wake up and they run the same exact code, but they know themselves as having different identities. And those identities might be selected from a set of different capabilities.

And so it's arranged in a leader-follower single-level hierarchy for this application. It's been built differently for other applications, but here there's a single agent. His name is Optimus Zero. In the Cyber Grand Challenge, we actually had a fallback series of Optimus agents. So the one that was in charge was called Optimus Prime, as you'd expect. And it could be Optimus Zero or Optimus 1 or Optimus 2, depending on what broke. That capability is all still in the code. So when you get it for free, you can find that stuff about fallbacks, but it's not active in LACROSSE because we couldn't get around to testing it and making sure it still worked.

So there's only Optimus Zero in LACROSSE. And he tells the other agents, which are historically called Fuzzbomb agents, what they should be doing, and they can do things other than fuzzing.

The fundamental agent design - I'll tell you two things about it. It's a plug-in architecture similar to what Yan was saying. We call it a plug-in architecture because there is a structured representation of tasks that it can run that take time, and we call them deliberative tasks. So they have longer duration than just quickly responding to a message. They're like start a fuzzer and think about it, or analyze the fuzzer's output, or run a symbolic analysis tool. And each of those is a plug-in capability. And so they have an outer wrapper that says how a deliberative task is performed. And all you have to do is fill in the middle. Well, you have to initialize it. You have to start it. You have to watch its output and decide when to end it or watch to see if it ended. Then you have to process its results. That kind of structure is why it's a plug-in architecture.

And then the agents all communicate in one form or another with each other. In CGC, they could all talk to each other. In LACROSSE, they all just talk to Optimus Zero, and he tells them what to do.

The other thing I'll tell you about the agent structure is that each agent is running essentially a simple loop that says "what tasks do I have right now and sort them by their priority. Pick the top one and start it." And it's going to basically consume that compute core or it's allowed to. So it only does one of these deliberative tasks at a time. But meanwhile, there's another communication loop running in true parallel that's listening to any messages it gets and being responsive. And that could include messages saying "stop doing that. Do something else." Or "here's a new thing that you should think about. Figure out what tasks would be created in your mind, but don't do them. Just put them in your queue." And then the next time the deliberation task ends and you're ready to do something else that can eat your compute core, then the loop on the other side, the task loop, will say "Okay, pick the next thing and start it."

So that's how the agent works. And as I say in LACROSSE, everything is a star communication pattern going up to Optimus. He decides what to do with the tasking, tells the Fuzzbombs what to do. When they get results they want to return, they can send them back to Optimus and he decides what to do. And so he decides how to do all the decision-making about what to submit so that the agents aren't all submitting and messing up the scoring and messing up the strategy. Very important for competitions.

So that's the vision of how it should work. And if you want to dig down more now or ask other questions about the top level first, that's probably what we should do.

**Adam:** Yeah, maybe we can understand - so this is, I mean, I think it would make sense that this is also a distributed platform where you can run on multiple - is it an agent per core because you said an agent could saturate a core?

**Dave:** Yeah, roughly, and yes, it can run across arbitrary hosts. The platform ran on our cluster in CGC on about 500 compute cores across about 17 or 18 machines. And in AIxCC because of the scalability of the Azure hosts in the final, we were actually running only on three hosts, each of which had somewhere around something like 100 cores available. So we were running about 300 agents for the final.

**Adam:** Interesting. So is the - and just trying to picture this in my head - so as more agents, is Optimus Zero telling each of the agents what they need to do, so it knows "okay I have 300 versus 500, so I can allocate things differently"?

**Dave:** Yeah. And that's a static allocation. So we didn't have the scalability and dynamic scaling that you see in some architectures. In this case - now I will say the framework has done dynamic scaling in the past in other projects - but here, no, partly because of the changing requirements on where this had to run and how it had to run. We just never got there from Kubernetes and KMPO, and then now we've got Azure and we can do whatever we want, and we were like "yay, back to our happy space where we can do whatever we want," and we just were like "Okay, we're going to do it the old school way."

And we did talk, by the way, about throwing everything out at the beginning and didn't do that, which might be a lesson learned.

**Adam:** Yeah, maybe we'll get there. But it does make sense - you're a company. This is something that you're using internally. It's not like you have used it for other projects as you mentioned. I'm sure you'll use it for other things in the future. So you know, it makes sense to build on top of a core that you already have.

Whereas a non-coordinated hacking team like Shellphish, the exact same thing happens every year with our shooter in an attack-defense capture system - like the thing that submits or runs exploits against people. I've seen in my what, 15-20 years of CTFs, Yan, like probably 20 different ones. Like it's just wild. Like every year some new person is like "how hard could it be? I'll do it better. Mine won't..." I've been that person once.

**Dave:** Yeah, the problem - well, the difference with our model is that you underestimate the difficulty of something completely different, right? With the throw-it-all-away model, you've underestimated how difficult it is to rebuild this thing that you had working over on the side. We started with a fully functioning system on the wrong platform and kept developing it and making it better, not really understanding how much work it was going to be near the end of the project to get it all working on a new platform. And so, okay, that's first system syndrome, I guess.

**Yan:** Yeah. As opposed to the 15th system syndrome.

**Dave:** Yeah. No, second system syndrome or something. First system on Azure.

**Yan:** Yes. Yeah. And that's other interesting stuff that I don't think we've got into yet of the different hosting environments and the changes that happened. Did you see that as a challenge, let's say from the environment that you had in quals to the finals environment, or was it more suited to what your system is able to do?

**Dave:** I think we liked the new environment better. The trip was more costly than we would have liked. The journey was rough, but getting there was good.

Well, there were two parts to the journey. One was undoing all the stuff we'd made it do to make it work on the semi-finals thing, which was not really compatible, and so putting it all back in the context of - you might call it rebasing, but that is not what it was. And then figuring out how Azure worked and figuring out interesting things about Azure - like certain forms of communication don't work the way we are used to, and we couldn't get them to work in time. But could we use a shared file system to make that problem go away? And the answer is sort of maybe yes. But then we found out it was really slow. But then we found out that if you bought a bigger shared file system, it got way faster. So those kinds of learnings were really important.

**Adam:** Yeah, that's fascinating. And this is at the framework orchestration layer. So the agents themselves and their logic didn't have to change depending on the environment.

**Dave:** That's pretty much right. Yeah. Yeah. I mean, I'd hope so. That's the point of having a framework. But you know, the leaky abstractions and all that - like sometimes it bleeds through.

**Yan:** Objects, man. Lisp objects.

**Dave:** Very fascinating.

## Target Processing and Task Allocation

**Adam:** So okay, so then yeah, next maybe if you could walk us through - so your system's instantiated, you have Optimus Zero ready, and a new repo comes in. What happens?

**Mike:** Yeah. So Dave was talking about tasking. I think the important architectural elements here maybe like targets, tasks, and messages between the agents.

And so Optimus is thinking about targets and turning them into tasks, in a sense. That capability exists on all the agents. It's something that - when they can take an object and figure out what needs to be done next, it's kind of fun, but it's not the way that we thought was most efficient to work on LACROSSE. So we added a new element to targets, which is "hey, this is my idea about what you should be doing next."

And so Optimus is taking these targets, and then when it passes them through the messaging system to the other agents, it's suggesting a course of action essentially, which means that although the other agents are processing the target itself and generating their own set of tasks which they are then scheduling for themselves based on priorities as they understand them locally, the tasking in this case has really been done by Optimus itself.

So that's how the incoming target is processed. Optimus says, you know, "given the state of this object, these are the next things that need to happen."

**Adam:** In - is this based on like a - is it LLM driven? Is it like reasoning based? Do you have like a workflow that you have said "this is what we think should happen"?

**Mike:** Yeah, in this case the workflow is kind of implicit in the code. Yeah. Yeah. No, that makes sense. In other cases, it's been lifted a little higher, but here we're saying, you know, "all right, this is the handler for a particular stage of the process, and I'm going to send this target off to a particular - not a particular agent, but you know, select an agent, get what are the harnesses, what are some other characteristics about this target that are going to be relevant to all the assignments that I make after that."

**Adam:** That information - harnesses become a target itself, or do you annotate the target with "this is the number of harnesses" and then you shoot out to other agents?

**Mike:** Exactly. Yeah. The latter. So we say, you know, "here's the set of harnesses. Now as I send this out to each of the different agents that are working on the target" - and you know, the allocation is based on how many agents are available and so on - "it will then say I want you to do fuzzing and I want you to use this harness to do it" and whatever other parameters might be associated with that.

So it might create like 60 tasks or 60 messages go out to 60 agents, which then have a task to do this, and they might have other tasks locally which they are then cycling through based on the priority system.

At the same time as the fuzzing happens, we would be sending messages to other agents saying "get the LLMs involved and try to start scanning the codebase for potential vulnerabilities." That's the stuff that Matt knows better than anyone else here.

And then, you know, at each stage, the information is flowing back through the messages to Optimus. Sometimes tasks complete, and so that agent will be sitting idle depending on what else might be in its queue. Or there are tasks that continuously send messages back to Optimus as they roll along. Most of the fuzzing tasks fit that model where they're "hey, here's something you should be looking at. Here's something you should be looking at." And then Optimus would be considering the state of that target as it knows it, as it gets that global picture, and then distributing new tasks to new agents in the form of targets to keep the process rolling for each one.

**Adam:** And then so like the - then so I think you talked about okay, so we like - you must have to build the targets, right? So something's got to build Optimus this...

**Mike:** You know, Optimus creates an object in its head, which it then - it writes some stuff to a common file system, but most of it's in its head. And then when you talk about like building the code that's underneath it, that's going to be a task that's distributed to one of these agents.

## Vulnerability Discovery and Patch Generation

**Adam:** Cool. So then, okay, now you found some crash - like a fuzzer found, or Optimus knows that a fuzzer found a crash, or an LLM said "I think a bug is here." What's kind of like the next rough steps or process?

**Mike:** Might be a good place to hand it back to Matt. Optimus will get a message saying "Hey, I've got a POV here." It'll evaluate it and possibly submit it in this game. And then it'll say "what we need is a patch," and then it will send or generate a patch. Maybe possibly - in semis we would ask a bunch of agents to work on patches. I think this time we only did one at a time, but that's Matt's department.

**Matt:** Yeah. Yeah. We just do one at a time. And a patch - when you say one at a time, like per POV, right?

**Mike:** Exactly. Right.

**Matt:** Yeah, we did think about kind of tasking a bunch of different LLMs with the same POV in parallel, but I don't think we ever really thought that was the best decision.

So we generally - our LLM pipeline, we kind of have three different LLM-based tasks, flavors of task. We have characterization of a vulnerability. We have the patching of the characterized vulnerability. And then we have SERIFF, which is kind of out on its own, which we did in the last week or two.

**Yan:** And classic SERIFF, right?

**Matt:** Yeah. Which ended up actually working out. It was one of the more surprising - surprising to the upside as opposed to some of the other surprises.

But yeah. So we have this characterization and patching sequence distinction between the two phases, and then you can kind of see it as like a 2x2 matrix where orthogonal to that, we have whether you have a POV or whether you're just trying to use the code alone and the diff, of course, in the case of a delta task.

And so yeah, we - this is where, you know, it becomes - we become more generic and less unique because we do end up going into the Python at this point.

**Yan:** Oh no.

**Matt:** Yes, it gets dirty.

**Yan:** What's that? No, you got to stay.

**Adam:** Yeah, I keep telling you, Yan. Lisp is not just a functional language. You heard them - they talked about objects, man.

**Yan:** Functional objects. You got the cars and stuff. There's all sorts - trucks, vans.

**Dave:** Yeah, CLOS is one of my favorite parts of Lisp.

**Matt:** So yeah. So we have these characterization and patching stages. Characterization is building this vulnerability object that generally has a description - a natural language description of what the vulnerability is. A CWE assigned to it. It has a file, a kind of a loose plan around how to repair the vulnerability, which also has specifics about which files and functions to be looking at, and an idea of what should be done. And then some additional notes which aren't very exciting.

And so that's kind of our unit that then - when we go to, you know, Optimus can be tasking - you might have a characterization task that generates multiple vulnerabilities, and Optimus can go assign those, a patching task for each one essentially.

And this is also part of the reason for this separation was also we wanted to get to LLM-driven seed generation for fuzzing, and we imagined that that would kind of be driven by these hypothesized vulnerabilities in the case we don't have a POV yet. And we never really got - that's still a dash, there's still a dash line around that box in our system diagram, literally. But yeah, that's kind of the high-level separation that I can potentially talk about, you know, what's happening inside those different modules.

**Dave:** I will say, yeah, I think we'll want to dig ahead. I say we did have LLM-based seed generation in the semi-finals, but it atrophied and it never made it up to the top of the ticket list.

**Matt:** So yeah, but please continue.

**Adam:** Yeah, this is great. So then okay, the - and how - okay, so at least from like the system perspective. So essentially all the game strategy is in Optimus Zero - is that kind of a fair way of saying that? Like the playing of the game in some sense, along with resource allocation, essentially by allocating tasks.

Now the one thing I was curious on is the priorities. So who is setting the - is it the agents themselves that decide among all the tasks they have, they prioritize, or does Optimus tell them like "this is high pri or low pri"?

**Mike:** Optimus tells them, and it's mostly very static. As far as - I think you should describe the rolling thing though, where they - as they repeat, like the fuzzers repeat, they lose priority and then another fuzzer that's on the same Fuzzbomb can take over, right?

**Dave:** Yeah. So there is a dynamic element, a local dynamic element. I think we anticipated that gameplay would incorporate a global dynamic element too. And there's some - you know, Optimus could tell agents in theory, "this is a high priority target. We don't have any POVs for this yet" or "this, you know, whatever." But this doesn't really come into play - like the capability's there.

**Mike:** Yeah. But we didn't fully implement that in time to - there was a lot of talk about scoring in the last like 3 days.

**Adam:** Yes. Mostly just like - always how we asked before we started recording. We were chatting about what Yan and I's contributions were to the team. And one of the actually strong ones I think was probably when all of the professors showed up at the hack - at the Airbnb, like this giant three-story thing that we had rented in Flagstaff. We had like a - it's kind of like this infamous 5- to 7-hour like game strategy meeting where you know, the first two hours was the captains teaching us the rules of the game and then going through "what's our strategy going to be" and then putting it into a document so we wouldn't forget the things that we had decided.

**Dave:** Then so yeah, I you know, I - it remains to be seen how well that strategy works. I guess we'll see.

**Adam:** In the professor's defense, it's not that we were - I mean the rules...

**Yan:** You're going to blame it on the students is what you're...

**Adam:** No, no, no, no, no, no, no, no. We were working with the latest version of the rules up to date with an earlier version of the rules, and this probably contributed to what you said - like you know, the last 3 days you're like "okay, we finally can get around to what should we do with the latest version of..."

Which then gets into the question I think you touched on it, Matt - what like what was the strategy or what did you do when you had a patch for something that you didn't have a POV for?

**Matt:** When we had a vulnerability, a hypothesized vulnerability that we didn't have a POV for. Yeah. So in the delta case, it was pretty - it was nicely constrained still by the delta. And in fact, when we were running kind of tests against our benchmarks, our nginx benchmarks which came out of the semi, sometimes we'd see that you know, if you had a delta, it could perform basically within noise perhaps of having a POV.

But yeah, so in the case where we had a delta, to get down a little finer grained than before, we are looking at the delta, we're extracting the functions that are mentioned that are relevant in the delta, just to kind of optimize. There's a lot of like context window optimization going on.

So we found that we did better when we focused as opposed to handing in even if the, you know, the context windows were kind of growing over the course of the competition. So that was a tricky thing to figure out how high priority that really was. But I do think that that game of trying to just densely fit in the relevant information - I still think there's a payoff even if nominally the context window allowances are, you know, plenty big now.

And so yeah, extracting those functions that are relevant to the delta, characterizing, you know, putting those into the same prompt and getting a characterization out. Perhaps yeah, I guess in the non-POV case, you really just have the code and the delta and generating the characterized vulnerability. And then on the patching side, we actually didn't - we could look at multiple files in the characterization of a bug, but we never - it never rose to the top of the priority list to patch multiple files. Although there's nothing necessarily non-trivial - like that's doable. We think it just - we had bigger fish to fry.

**Yan:** But yeah. So yeah, Shellphish to fry.

**Matt:** Yeah, that's right. There it goes. It's coming out.

## Patch Submission Strategy

**Adam:** Okay. Yeah, this is great because I think the one interesting thing that's come up - so we recorded the Theory episode yesterday. It hasn't been released yet, so you guys obviously haven't listened to it yet. But the key difference we're noticing between 42, Shellphish, and Theory and I think your guys' system, although you can correct me if I'm wrong, is 42 and Shellphish never created a patch for something they didn't have a POV for. So all the patch generation was always POV-based, whereas Theory - they have a very LLM-heavy approach. So they were similar to yours. They could patch bugs that they were very sure were there but didn't actually have a POV for. But then they brought up the fact that then we had the strategy question of "do we submit that patch?"

**Dave:** Oh yeah. Yeah. That's what I thought you were asking. And I wrote that code I think in the last 24 or 36 hours before, which was to say "all right, so we got these piles of patches for hypothetical POVs," and Matt was madly working at the same point getting scoring set up so that we could somehow set up confidence measures for each of these. And then so from a gameplay perspective, the idea was "yeah, we love those POV-based patches and we're going to submit those as soon as we find them because we think those are golden." And then we have some kind of conception about how likely there are to be other vulnerabilities, some confidence measure based on how the LLM has scored via questioning and filtering the vulnerability itself. And then at a particular time before the deadline, Optimus says, you know, "I got three POV-based patches already submitted. I'm going to look over my list. I'm going to compute some kind of like max." I'm not going to submit 50. And then I'm going to look at the confidence. And I - now I've forgotten - there was some - we had a sliding scale. How did we - I wrote this where - say you know, "I'll submit you know X really high confident ones, but some smaller Y if there's some lower confidence." And so that was how we tried to sort of flexibly handle that case of saying "well, they're probably not as good as the POV-based patches, but you still want to submit them in case they are valid patches because patches are worth so much more than POVs, and the accuracy multiplier hit is not so much until you submit a ton of them."

**Adam:** Better to be incorrect, right?

**Dave:** Yeah, you want to keep your number down to a reasonable, you know, your denominator, but you do want to take advantage of all this. I mean, and I think our assessment was the LLMs were doing nice work, so we wanted to take advantage of the patches they were creating.

And I'll add in we were also deduplicating the non-POV patches against the POV patches. So we wouldn't submit a non-POV patch if it was a duplicate.

**Adam:** You thought duplicate characterization as in it patched the crash that the POV induced in the program.

**Dave:** Yeah. Yeah. Because if we - when we're patching a POV-based vulnerability, we have more to work with. We can test against the POV, and yeah, so we trusted those more. And so yeah, if we had all this deduplication, LLM-based deduplication based on the characterizations.

**Adam:** So what did you use? Stack traces have come up previously. Did you like - what have you - what's your deduplication like?

**Matt:** Well, so as I mentioned before, we have these characterization and patching stages, and out of the characterization stage comes this vulnerability object with these different fields - the description, the CWE, the like repair plan. And so that's what we use basically is we'd look at those fields. Look at the - first we'd filter by what vulnerabilities had locations in the codebase that intersected, so we weren't deduping against anything that was like completely different files or functions. But then within that set, we would give those to an LLM and just say basically, you know, "here are the described vulnerabilities. If this looks like - if this is a POV-based one, a non-POV-based one, and it looks like a duplicate of one of these POV-based ones, just skip it. Don't create it."

And you have to worry about the other direction too. That was the more complicated case where you have a non-POV one come in first, and then later you find a POV one that matches it. And now you want to prioritize that one. So you have to go back and ax that earlier one.

So we had great plans to do various forms of fuzzing and testing on patched targets, which would be perfect for this case, and they were not realized before the deadline. But that would have been another nice way to test - just to double-check your patches.

**Dave:** Yeah. Well, and say "is this, you know, does this patch generated without a POV actually block this POV that we've identified previously?" So yeah, and then various kinds of double-checking.

**Yan:** So yeah. And we wanted - No, I mean everyone's - I'll just say we wanted to do that fuzzing against the patches because, you know, in the rules is a complicated aspect that if your patch doesn't fix other people's POVs, then you get zero. And in fact, you get penalized, right? So it would have been really nice to do a whole ton of fuzzing on our patches, but we did no fuzzing on our patches.

**Adam:** Yeah, this was something that Theory brought up - they thought about this dilemma that man, you could have the LLM create a patch for even, let's say, a zero-day non-intended vulnerability, submit it, but if no other team submits a POV for that, it's considered an incorrect patch gamewise.

**Dave:** I'm not sure that's - organizers didn't put it in there. No, if it was a zero day, they have to look at it manually, I think, afterwards. And that's a lot of work. I think if they knew it was a crash, I think to them they would just see it as "this is a patch that didn't fix anybody's POV."

**Adam:** Yeah, you might be right. Yeah, this is one of the interesting things about building a game, and we mentioned earlier the rules change in some sense. The rules change because the capabilities change and new situations come up like this.

**Dave:** Well, then the other thing - like at the very beginning of the competition that we were butting up against is this fact that like zero days were definitely in scope earlier with the Linux kernel, and we're like "why wouldn't we just hoard a bunch of zero days and then you know, cleverly seed the fuzzer like that." But like yeah, anyways, we did not do that, and the rules changed and made much more sense as we went on. This is way back in quals, like pre-quals, but it does introduce these sort of ambiguous situations, right?

Are the organizers going to look at every single otherwise inaccurate patch or invalid patch and say "oh shoot, this actually is a no-day that got patched," and in which case maybe what they would do is write a POV for that and then that patch - which is within the rules if there's an actual vulnerability, they can create them. But my reading of the rules was much more "if there's a POV that hits," because they need reference patches in order to score properly. But I yeah, this will be fascinating. We've mentioned - what if we have someone from the organizers, and they're probably much more constrained about what they could talk to us about than the teams. But that would be a great episode as well.

Because a lot of this stuff, you know, what can be frustrating is LACROSSE is out there as the top cyber reasoning system, and due to a specific reading of the rules, whether that's a difference between your reading and the organizers' reading or just something no one had thought about, the rankings don't reflect that, and you only get 2 million or 3 million instead of four million, right? Like that'd be frustrating.

**Dave:** Yeah, it would be frustrating. Hard world. We want that problem.

**Adam:** Yeah, that's a problem. Exactly. Yeah, that it's something we talked about before, right? Like the results will define - like there is for sure how the systems do, but something will - like the way the challenges are, if some challenge triggers some weird behavior in somebody's CRS that knocks it out, like that's definitely happened in the past as Yan has mentioned before and could happen. It's, you know, we're all trying our best to field the best cyber reasoning system we can, but this is real-world code that we're analyzing. So anything can go wrong.

## LLM Performance and Strategies

**Adam:** So you mentioned earlier, speaking of real-world code, just to dig into a different piece - you mentioned the LLMs are pretty good with the patching. I think I heard that. The component I worked on - much ado has been made about my incredible contributions to someone else's component in our CRS in previous episodes - but that component, we found that the LLMs insert code like a three-year-old. Like you know, like last episode we talked about "oh, they put lines of code between the if and the curly, they put like you know, lines of code inside a multi-line conditional." You...

**Yan:** And you forgot to tell - my suspicion was a lot of this is prompting. You forgot to tell it it was an expert computer programmer first.

**Adam:** Yeah. So your guys' experiences - you told it "be the best that you can be" and it was.

**Matt:** Yeah. I mean there's a lot - that's a small part of our experience. Yeah, we did have that at the beginning of every prompt was "you know, you're expert cyber security researcher" and then so on. But also, you know, we decided early on that writing a patch directly was not a good job for an LLM. And I don't know by the end of the competition if that was still true because these things were changing out from under us and advancing you know, presumably very quickly.

So we had a strategy where we were always rewriting code - rewriting different files in a codebase, and usually not. We also saw big gains early on when we were not rewriting an entire file at once. Part of that was at the time the output tokens couldn't support a lot of these files - like we didn't have a big enough output window. But also just, you know, it's going to do better when you fit less into the context window if, assuming it's all still the information you need.

And so we would rewrite functions. We had some, I think, some clever strategies about putting those back into the files in a way that was guaranteed to correspond to the right line numbers. And yeah, basically, we were doing everything we could to use the LLMs to rewrite targeted pieces and then programmatically generating a patch via a diff at the end.

I don't know if that's played into some of the issues you found with using LLMs to write these - if you were writing patches directly, but that was something we found. So we certainly had a lot of trouble with LLM patching in the semis. And in fact, I'm still not sure that we really patched anything with an LLM in the semis. We were able to, you know, while we were waiting for the next round of rules to come out, we did some forensic work on the semis and were able to improve the performance in that environment and architecture. But yeah, I guess...

**Dave:** Well, and Matt, does any of the consensus or voting behavior play into this too? Did we have checking between LLMs to make sure that patching was applicable and effective?

**Matt:** Yeah. So there's kind of a couple different aspects to this answer. And so we had two different general approaches to using different LLMs to get more robust answers. One was the serialized mechanism where we would go through a pipeline if there was a failure to even like complete the pipeline. We had - our pipelines consisted of these highly structured input and output interfaces that could be like arbitrary type definitions, and that was something that DSPI - this framework that we were working within - does really well.

And so if there were any failures to meet our like type specifications at any step along the way, that was kind of one type of failure. Then there was another type of failure which was you get to the end, you generated your patch, and you're testing against - you want to make sure your codebase builds and fixes the POV. That's a different type of failure. And in either case, we would go back and try a different LLM from this big long list of prioritized LLMs. So that's kind of the serial mechanism.

And then within given high-risk steps like the characterization step early on - if that goes awry, we had some failures in our testing where we saw that step go awry maybe one of every 10 or 20 times on this problem that otherwise we get every time. And so we wanted a mechanism that makes that like really robust - you know, like fewer than 1% of times we want to fail. And so we have a parallel consensus mechanism is what we call it, where we issue - do the same - it can actually be any arbitrary Python function, but in general it's like some DSPI module that may have submodules, some piece of the, some chunk of the pipeline - you issue it to let's say five different LLMs at once in parallel, and then you assemble those into a list, a numbered list, and you ask another, some other LLM, to give you back the representative, the most representative answer.

**Adam:** And it doesn't even need to know about the question. It just is saying like "this one is the one that basically best represents these experts." It gives you one through five.

**Matt:** Yeah. And it gives you one. Exactly. Super low output cost. It's just giving you a number, and then you index. The other cool thing is, as long as those choices can be represented as strings, you can be choosing - but you know, the items themselves can be arbitrarily structured objects because you're using that number to then index into the list.

**Adam:** And that's really cool. I think this is the first - trying to think - this is the first time you've heard something like this. A lot of people try different LLMs. I also haven't heard the serial retrying with a different LLM. That's also cool. So that's a clever way of using these.

What was the order of the LLMs? What models did you find most effective?

**Matt:** Yeah. Well, there was strategizing around effectiveness, and there was also strategizing eventually around rate limits.

**Adam:** Yes. Rate limits. Yes. Yes.

**Matt:** So not only were there different rate limits per model or - Oh, yeah. I guess there were just different rate limits per model even within a given provider. So yeah, you wanted to - we wanted to make sure that you know, different steps, if all else being equal, they should have a different priority list so that you're hitting, you know, a different first choice model for your - for your - yeah, to kind of diversify the rate limit problem there.

We had - I think in the end for our general patching pipeline, we had GPT-4o1 as our first choice, but we would interleave the list like Sonnet 3.5 might have been next. It was kind of interesting. We had, you know, you do play a game with cost. We didn't want to go right to the most expensive model. In some cases we did have some of those most expensive models at near the end of the list as like a last ditch effort. "This step needs to succeed. You're not going to get here very often." So Opus might go there. But yeah, we'd have some good but not super expensive ones near the beginning. We'd have maybe some cheaper ones in the middle, and then maybe in some cases if we really cared, some like super expensive ones at the end.

But o3 - by the time the competition rolled around, o3 was one of the best and like a mid-range price. So that was interesting because that - you know, because of rate limits and everything, you don't necessarily want to use it everywhere, but that definitely got swapped in for some high priority places.

**Adam:** Yeah, and that was one of the things that I - it sounds like you guys hit as well and I know other teams did, and this is kind of the nature of the beast - but the models underpinning this stuff was constantly changing, right? And not just the models themselves, right? You could always talk to one model, but the landscape of models was changing. And so a newer, cheaper one comes out, or a better one that's more expensive, and then you have to kind of retest, re-evaluate what your strategy is going to be.

**Matt:** We changed some of that stuff in the last 48 hours. And I wanted to mention one other kind of really interesting phenomenon which I've now forgotten. So when I remember it, I'll bring it back up.

## Benefits of Lisp and Development Environment

**Adam:** Okay. While you're thinking of that, now I can ask some Lisp-style questions. So how - like what were the benefits of using something like Lisp? I mean the classic benefits to me are either macros, being able to write domain-specific languages to do this thing. Is it having being able to hot patch functions? Is it having a REPL available to reduce dev times? Was there like a core benefit, or it's just that you and the company have been using this for so long that it's kind of like second nature and so that's what the benefit was?

**Mike:** I have a couple thoughts. For me, yeah, go ahead.

Yeah, the dev environment is the big winner for me and having the REPL and having the capability to start up a new piece of code, run a function level or module level piece of code independently at the REPL while I'm building - that's huge.

Those other things I think we get a bit of the flavor of a domain-specific language through our use of CLOS rather than the macro system. You know, we've got a pretty well-defined hierarchy of task objects, for example, and it's pretty easy to pull one off, fill in a few fields, and plug that back in and have it go.

**Dave:** I wanted to point out when we were doing the architecture overview, there's another really cool thing that we did frequently in Cyber Grand Challenge, but we didn't do at all during AI Cyber Challenge, but you can actually inject new code straight into the brain of any one of these agents with a message. And so not only could human supervisors do that, but if Optimus, if we had wanted to do the thing where Optimus decides "I want to change the priority of the fuzzing on this thing that I don't have any POVs for, I've already sent it out," we could either have a message to define to do that, or he could just send an eval message and he could tell the guy "eval this code that says on task 27 set the priority to 900," and it would just execute it.

So there - that doesn't sound like a great cyber security thing if LACROSSE itself was a target. But for development, it's really fun and really cool. And you could have your whole system up, you know, if it takes, I don't know, some amount of time to start up all 500 agents and they're not quite doing what you want and you want to inject a new piece of code, like even just a new method into all of them, we could do that with this agent infrastructure. That code is all still there. So you'll get it for free if you wanted to run it. We didn't use it, but it's all there.

**Adam:** Very, very cool. I love that. We usually ask this in a different way, but since it's Lisp, how many parentheses are in LACROSSE?

**Dave:** Great question.

**Adam:** I think the underlying question there is what's the rough like size of the code of LACROSSE? Do you guys have some notion of like we're talking I don't know, tens of files, hundreds of files, or is it you know, tens of thousands of lines of code or 100 lines of code?

I mean the Lisp code's probably a few dozen - I don't know, 20 to 30 files - but then there's a lot of supporting stuff. The Python's off in its own world being tasked at from the Lisp. I don't know, did we have anybody try to run a SLOC counter or anything on this?

**Mike:** Yeah, I don't know. But I would say you're probably under 100,000 lines of Lisp and way under 100,000 lines of Python that we wrote or Matt wrote. But in the range of other CRSs.

**Adam:** It's very cool that you got this dual - with this trend, let's say the functional design on one end - one of the big challenges with a cyber reasoning system, especially once they get very large, is like "I want to work on this one part of it and I don't want to spin up the entire thing to generate all the input. I just want to drop in here and work." And I'm going to guess that your system is very good at this. This is something that we had to explicitly support in Artificial Fish. And by we, I mean, you know, the people that were actually writing this part of it. And it's not easy in anything that's not kind of, you know, well...

Maybe then the question is how easy was it for people to just dev or work on one component? And maybe let's start there.

**Matt:** Should I talk about the LLM pipeline piece because there is an answer there. Sure.

So we did early on invest time into separating out the - you know, kind of carving out the place in the pipeline near the top where we could call these things independently outside of the Lisp architecture and just rapid - much more rapidly. It was a 3-minute test or less per problem versus a 30-minute, and so that allowed us to optimize the pipelines separately early on very quickly. And then you know, in the last month or two, we were running all our tests through the Lisp architecture, but that gave us some early traction.

**Mike:** Yeah, inside the Lisp, this was never as good as we would have liked, I would say. We did have the ability to sort of isolate a task. You know, if I was working on a specific task, I could set up the test environment so that, you know, couple steps were, you know, filled in automatically, you know, were mocked out, I guess. And then run that specific task. It still took a few minutes just to fire the sucker up and download the target and all this stuff.

And then there were really tough ones I thought - like and I mentioned already this - the patch submission near the deadline thing. I mean, setting up a test for that was really painful. And I was doing it in the last 36 hours of the contest and trying to set up things so that I could run a test in a reasonable amount of time that would get to the deadline with several POVs hanging or several non-POV patches hanging around.

**Adam:** No, this is exactly the similar problem that we had of like how to test those later parts of your pipeline that need input, and sometimes you only find bugs through testing random software and just...

**Dave:** Yeah, it's very - Lisp might be nice, but it wasn't the silver bullet in achieving this decoupling capability in the end - not in this case. But I do think that the stubbing functionality that Mike mentioned, if we'd had more time, we could have done much more with that.

And because the format of the challenge tasks changed between semi-finals and finals, our stubbing broke and most of it was never repaired. We had more ability to do that in the semi-finals where we had pre-canned POVs and you could just turn them on and the thing wouldn't fuzz at all and it would just whip right into the patching stuff. So testing the patching integration, for example, was quite easy back then. But that stubbing was broken for most of the final competition development, and I don't think it all ever got put back because the structure of the challenge task was so different.

**Adam:** Yeah. I mean it makes sense. You got to keep going.

## Secret Sauce and Technical Innovations

**Adam:** So okay. So now that we've got I think a great insight into the CRS, I'm sure we could talk for you know, several hours on this. So what would you say if you had to say like what is the secret sauce of your CRS?

**Dave:** Well, I'll go first and I'll say in addition to Lisp, which we mentioned already, which was fun. But I would say Matt told you about some of it, and the things that Yan called out like the consensus work and the generic fallback mechanisms that Matt invented and put together I thought were really great, and they fixed a lot of things for us. So I kind of nominate Matt's stuff.

**Adam:** Nice. I think Matt will nominate his stuff too, right?

**Matt:** No. Well, I'm going to give another shout out to DSPI because - just or you know, maybe not - it's probably a more general framework property of other things at this point. But this idea of having like highly typed structured input and output interfaces for modules that get more and more - you know, you're using them in a more and more kind of fine grain or like LLM microtransaction kind of way. But at the same time, you're trying to create them to be general purpose so that you've put some time into writing them here, and now when you go need to prototype the next thing, you're like "oh, you know, filter this list of strings by some arbitrary criterion. I have a module for that."

And so it's just more and more rapid prototyping as you go. If you're trying to create these nice tight modules - and you know, we tried to be good about that. A lot of things happen late at night in the heat of things. But that was a huge win I thought of our use of that framework.

**Mike:** Yeah, I'll echo those. Lisp is great. Our agent architecture that we have been working on for decades is really helpful in getting something fired up quickly. The stuff that Matt did was amazing. We have two or four other teammates who work tirelessly to make all this stuff work in the competition environment, and that was really invaluable.

A boring one that I would add which occurred to me when Adam was talking before we started recording is in addition to this agent environment and our experience in the Lisp - we've got these testing tools that we have developed over not quite as long a time, and we start out a project with Jenkins running tests on every commit and overnight, and we've got an orchestration system called PRTT which enables us to create full-on system tests and also some subsystem tests that are running frequently. Now I think as mentioned earlier, you know, then you wait - what are you testing? We're not testing on the competition environment, and so we still had to bite that off at the end, and that was a bigger job than we expected. But as far as having a running system in some environment, we pretty much had that all the way through.

**Adam:** Great. And I think that that's really helpful. That's awesome.

## Evolution of AI Perspectives

**Adam:** And so okay, Mike, you just said 10 years or decades, I think, of agents. So I've asked several teams this. I think your team will have a very interesting notion of like how is your opinion on AI changed throughout the competition? And when I say this to most teams, I'm of course meaning LLMs, like how is your thought on the current state of LLMs? But you and your company have much more experience with like AI - like the kind of - you're talking about agents. Most people when they think of agents now, they think of LLM-powered agents that can - these chat bots that can call things - where you're actually developing like autonomous running pieces of code that are collaborating and executing tasks. So how like in this competition, how has kind of your outlook on the broad state of AI changed?

**Mike:** I mean yeah, even over the course of the competition really - I talked about the semi and the patching that we saw - and going into the end, as you know, fingers crossed, my impression is that the LLMs were writing great code. I was just very much blown away by what LLMs can do. I think, you know, we're - I'm really excited about the combination of formal symbolic systems and LLMs moving forward. I wish we had had a little bit more of that going on here where we could take input from the LLMs and suggest different strategies to the agents or you know, to the different tasking. But that seems, you know, that's really cool and it's going to happen right away. It's already nice.

**Dave:** Dave, what do you think?

Yeah, I totally agree with Mike that the LLMs have made tremendous progress in their ability to handle code and reason about code. Well, reason - I hate to use the word reason because we are symbolic AI reasoning guys. We know what reasoning is, and LLMs do not. And we shouldn't make the mistake of thinking that they do. So working with code is a lot like working with language, and that's one of the reasons they do fairly well with it. They don't work with plans, and so when you try and use LLMs to try and make a projective plan out in the future, it's just not going to really do well because it can't understand.

So I think that these - meaning of agentic meaning that LLM drives everything - that's backwards. We want our symbolic systems that actually do reasoning to drive things and task the LLMs to do what needs to be done. That's the kind of systems we're building in a number of other projects, and we have other projects where the LLMs are feeding knowledge into symbolic reasoning systems. So it's much like LACROSSE, only different kinds of knowledge, and I won't talk about those right now. But overall I think that yeah, the combination of real symbolic reasoning systems that have provable characteristics about them and these LLMs that absolutely do not is a great future direction, and I'm excited about it.

**Adam:** And Matt, great. I was going to say Matt, do you have the opposite as the person dealing with the LLMs? Maybe you have the contrarian in terms of this group take of saying like "just give the LLMs the control."

**Matt:** No, no, I think that was actually dead on with how I think about it. I think if the question is like "should we allocate resources towards creating a bigger and better LLM that can do this whole problem by itself versus do we still invest time into breaking up the problem, reasoning about it in a formal way," I would bet on the latter every time. And I think what LLMs give us is this hyperflexibility at each of like the leaf nodes in that reasoning tree.

Where yeah, it should be like if - in terms of future work on LACROSSE - like LLMs should be involved in the strategy. Mike or Dave both mentioned that LLMs should be involved in all these little steps where like LLMs do really powerful things when you can constrain the problem for them and turn it into this little tight little query, and then you know, you have this formal system around the outside keeping these persistent objects and not losing a thread and doing this nice formal reasoning. So more LLMs, yes, but in small pieces. And make the structure of the solution mirror the structure of the problem.

**Dave:** So don't let the LLMs call eval on your agents to inject their own code to run on your agent.

**Matt:** No Skynet.

**Dave:** Not yet.

**Adam:** It's a very interesting thing that's kind of come out as a commonality so far. One of the few commonalities in the AIxCC is this orchestration where different small tasks are - you know, which is not like "oh my god, surprising result" - but no one has thus far just said "o3, go! Maybe here's the tarball."

**Dave:** Yeah, I like to say when it comes to reasoning, this large-scale reasoning, LLMs may not be the engine, but they may be the grease. Like they may take these approaches that we've had in the past that had this brittleness to them and help us deal with that.

**Adam:** That's I think that's great. And I think that the grease part is really interesting because the thing that always amazes me is like why aren't we more super impressed that I can just write random text into this LLM and it can know what I mean? Like this has been such a problem of interfacing with computers that we've kind of solved, but like it's - we're like "Yeah, but it can't reason and it can't do this and it can't do math." And I'm like, "But like it understands what I mean. Like this has been so hard and like now I have this thing that understands me." It's just wild.

**Dave:** See, before you have a compilation error, it's your fault. Now it's the LLM's fault. That's a big shift.

**Adam:** Exactly.

## Competition Predictions and Reflections

**Adam:** Okay, great. So we've asked all the teams this, and I think we're all, you know, similar vibes. So what place do you think LACROSSE is going to get in the AI cyber competition?

**Dave:** I'd go with three so we can get some money for all this work. And I you know, I think we're - yeah, I think we've done a solid job. Well tested, everything is - you know, everything is good. I don't know that we have any crazy brilliant new ideas that you know, out of seven teams of highly motivated researchers, I imagine someone's going to have something really special. We might not have.

**Mike:** Yeah, I think three on a - when I'm feeling optimistic, I think three. When I'm feeling utterly pessimistic, I think four because that feels like it'd be even worse than, you know, five or six. I'm hoping they don't - I'm hoping they only announce the top three, and I think that's what they'll do. Although in CGC they did give all the scores all the way down. I would love to be three. We'd be delighted to be three. Like they said, that should be our problem.

I think that they're going to give out other prizes, and I would like to say that we might get the most efficient finding and fixing of bugs prize with the LLMs. Because I think if you remember the semi-finals illustrations, they had some of these agents or systems were just whaling on the LLMs, and our system was like it asked I don't know what, 14 questions and spent $7 on the LLMs. Now it's a lot different. It's a lot different, but I don't think we're going to spend whatever it was $50,000 on LLMs. I think we're going to spend maybe $5,000 on LLMs. And if we - you know, there should be a prize for dollars in LLMs per bug found and fixed, and I think we might have a good shot.

**Adam:** Actually that makes a lot of sense. That is very cool. Yeah, I like that idea of like the most cost-effective system. And in fact, you could imagine a scoring system just built around that in either this or follow-on competition, right? Because we have all of these like you know, this is your quota, etc. And there are of course financial reasons why quotas can't be infinite, but you could just say "hey, forget the accuracy, forget this, forget that - like your multiplier is you're one over how much money you spend."

**Dave:** Yeah, it's I mean it's fascinating, especially as you think you know, as things start coming down and down, right? That $5,000 may be $5 in two or three years, which is much more reasonable than even, you know, more money from $50,000 or whatever. I think some of these systems are probably unbounded. I think some of the people on these teams could use like Yan said, just infinite LLMs if you gave it to them. So yes, I think it's interesting.

**Adam:** Need more nuclear power plants powering GPU farms.

**Dave:** That's right. Better algorithms, you don't know, better chips. Like I, you know, who knows what the future's going to bring.

## Lessons Learned and Future Improvements

**Adam:** That's great. Okay. So now 2 years after this competition - so what was there anything that like looking back you would do differently or change or I don't know, because now we're at the 2-year mark into this and is there like lessons learned that you would teleport back and tell your past self to do differently?

**Dave:** Well, I would have a couple from the high-level perspective. One would be to potentially have started two major threads: one where we threw everything out and started over, and one where we kept going with what we had, and you know, had two separate teams or perhaps overlapping teams that you know, were getting the same lessons about the rules and all that, but see if somebody could bootstrap in a pure - let's say pure Python approach that fit better within the infrastructure that they gave us in the semis. And that would have been one thing. But to do that, we would have needed more manpower or person power. We simply did not spend all the money then, and we did not spend all the money on the finals development, just for lack of people. And we didn't feel we could hire permanent employees based on this small time duration. And so we considered hiring people short-term, but that's very difficult to do and integrate into a team. And we considered having people volunteer. You know, people called us up and said "Can we help?" And we were like "Yeah, you know, I don't really want to teach you how all this stuff works. That'll take too much time. Let's just rock and roll." But that may have been a mistake. We may have just needed so many more person hours to do all the things we wanted to do. We ended up crunched at the end as you heard. I mean, 3/4 of the things we talked about were developed in the last 3 weeks or something like that. So that's just not enough hours put against the project.

**Adam:** Is this a big - it's a big task? It's a big competition. There's like even just the parsing the rules and understanding then how that should impact your system and what things you need to change and do differently. The - we mentioned earlier the deployment environments changing - like having like you said, you had two people dedicated to getting stuff working in that environment.

**Dave:** Yeah. We had at least similar - like one or three. Yeah. Exactly. You need those people who can actually get this stuff working because it doesn't matter how cool the system is if it runs on your desktop if it doesn't work in the production environment.

**Mike:** Yeah. And the scoring, that's a good point. The scoring consumed one of our guys for the whole endgame just trying to figure out the scoring stuff.

**Adam:** Yeah. All the staffing stuff. And I would agree with that. And I think even within the time period of the contest effort, I think we tended to undervalue the last few hours before the contest deadline. And I don't know why deadlines in a contest like this are much different - they're though they're very hard compared to other projects. And the deliverable is very well defined, at least to the extent like how is it going to turn over. But we were you know, sitting out 10 months out from this thing saying "well, we don't really know what the competition environment is going to be and we don't have an example and you know, well, you know, we'll have plenty of time to work on it later." And I think you underestimate how much more valuable those last few hours are. And so yeah, you can - those hours 10 months out were cheap, and we could have been spending them, and maybe we would have thrown some of that stuff away. But it would have been really nice to have, you know, a few more test examples ready to roll when the problem was better defined, or better understanding of the different examples as they came rolling through. And you know, live and learn.

**Matt:** It's a great lesson learned actually. Like I wonder if there's something here as a lesson learned for organizers of these types of competitions. After the Cyber Grand Challenge, there was a series of competitions abroad - the robotic hacking games - and they took all of the infrastructure of the CGC and ran it. And I think the first robot hacking game was literally just another cyber grand challenge, which allowed teams participating in that - the Mechanical Fish was the only open source CRS at the time, and the top three teams just ran the Mechanical Fish and customized it, which was a shocking thing that this was possible. But I mean, I wonder if a different approach to the AIxCC could have been you start with that infrastructure and you slowly... but there's so... the toy operating system that the CGC used focused...

**Dave:** Yeah. Yeah. It struck me.

**Matt:** I don't really have any good lessons beyond the ones from Dave and Mike for us. I was around in the semis. But I have been thinking a lot about - in terms speaking of lessons for the organizers - I keep thinking about how if there had been a - like of all these variables, of all these constraints, the budget, the time, yeah, the LLM budget, and then there's the like development budget. The one big constraint was the time lag between like when rules got frozen and also kind of the last I guess - or maybe first - exhibition round, the chance to actually run on their infrastructure, and the competition deadline. That amount of time was like the biggest variable for how good our CRS was going to be, more than how much money we had to spend on all this stuff. And so if the organizers for next time or whatever you know, if you want better CRSs for the same amount of money, just like work on making that time as long as possible, I would say.

**Adam:** Yeah, it's definitely interesting and it goes into Mike's point about the value of time being different depending on where you are in the competition. So kind of that insight is to like extend out the valuable time - like when you know things are locked in. But of course, like as we know, we've organized Defcon CTFs - like the organizers are kind of building things right in front of the teams. So you - it's always difficult, and they don't know - like depending on how teams point out various problems with scoring algorithms and other types of things, then you don't want that in the final game. So you want to make tweaks. It's a mess.

**Dave:** Yep.

## Closing

**Adam:** All right. Well, Yan, any final questions for our guests?

**Yan:** I think we have our favorite "What's your favorite AI?" But I think we covered that in what's your at the front of your list. I'm just - it's been awesome chatting with you guys. I'm just very excited to see what happens in the files, or what is happening, because of course all of these cyber reasoning systems are - are they already done, or maybe they're finishing up right now?

**Dave:** They're done earlier this year. Yeah, they're done. So like everything we're talking about, all of these agents and everything, they've clocked out. So it'll be interesting to see what happens.

**Adam:** Are you guys heading to Vegas?

**Dave:** Matt and I will be there. We'll have a few other teammates as well. Mike's stuck in Hawaii, so he can't make it.

**Adam:** Terrible, man. Mike, I've been seeing I think water reflections on your ceiling. It's very distracting. Like I could go for a swim right now.

**Mike:** Sorry about that. No worries.

**Adam:** Oh no. You can see a bit of a palm tree back there too.

**Mike:** Yeah, that's incredible.

**Adam:** All right. Well, thanks so much to Dave, Mike, and Matt from the SIFT LACROSSE AIxCC team for joining us today. I'm Adam D. You can find me online at Adam Dupe. He is Zardus. You can find them online at Zardus. Together we are CTF radio. You can find us online at CTFradio.com - O's, not zeros. You can send us questions through email at ctfradio@gmail.com. And your questions might end up on a future episode of CTF radio. Take care and happy hacking.