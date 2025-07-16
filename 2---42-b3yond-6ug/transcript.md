# AI Cyber Challenge Interview - Team 42-b3yond-6ug

## Introduction

**Adam:** Hello everyone. Welcome to CTF radio. In a shocking turn of events, we are now recording two episodes in less than a span of the week. So that is I think a record for us. So Yan, why don't you say hi to the people?

**Yan:** Hello hackers. Great to be here again. It just feels like nothing but podcast recordings in my life right now, which is awesome.

**Adam:** So that is the camera. You don't actually - I was going to say or you just don't work very much. Maybe that's what it is. It's just life living and podcast recording for you.

**Yan:** Podcast recording paper deadline. Podcast recording paper deadline.

**Adam:** Nice. That's great. You submitted what? Three papers within the span of the last time we talked. Is that correct?

**Yan:** Four. Four. Including one first author paper, which is something that professors just typically don't do 

**Adam:** Unless they have something to say or a statement to make.

**Yan:** Yeah, exactly. This is very different. It is just a paper to write and when you're first author and there's no professor with you. You just have to write every word of the paper. There's no one else.

**Adam:** Nobody's going to write that paper for you. You got to write it yourself. Oh man. All right. So, we are super excited today. We want to dive right into it. We have our first of a non-Shellphish team that we're going to be talking to about the AI Cyber Challenge. Because we've already had now I think this is the third or fourth episode in a row we're talking about AIxCC, we are not going to talk about that at all like what the background is. So if you want background on the AI Cyber Challenge please listen to our past episodes which of course I'm sure you all have.

So we are now the - I guess the very first question and of course the thing I should have done before we're starting this recording this episode was to understand how to pronounce the team's name or to say the team's name. I'm going to go ahead and say it's A Beyond Bug. Is that the correct way to say the team name?

## Team Name and Introduction

**Xinyu:** Our name is actually 42-b3yond-6ug. 

**Adam:** Yeah, but do you is it Hex? I mean 42 is a very or is yeah the reason that we maybe take 42 is because there was a book called Hitchhiker's Guide to the Galaxy and some of my teammate like that book a lot. 42 is the answer is the ultimate answer to the universe. So we take that one. So

**Adam:** Beautiful. 

**Xinyu:** Yeah. Even like our logo only have 42 without anything. So we want to call us 42. Okay. 

**Adam:** All right. Great. Team 42-b3yond-6ug. There we go. So I thought it was a like a hex encoding, but now this makes much more sense. The Hitchhiker's Guide to the Galaxy is one of my favorite books as well. So really great team name.

So we have 42-b3yond-6ug here with us. So we have four folks from that team. Why don't we - Xinyu, why don't you start us off and then we'll go around and everyone introduce yourselves. Maybe give us a little bit about your background and how what your role is on the team.

**Xinyu:** Sure. I'll go first. My name is Xinyu. I know my name is super hard to pronounce, but because it start with X. There are barely much English word start with X. So X pronounced as sh. So it's shin-yu. 

**Yan:** But it's awesome. You're professor X.

**Xinyu:** Yeah, thank you. So I am associate professor at Northwestern University. I am the leader of the team and basically coordinating the efforts and decide the strategy for the team and helping some of the design of the system and coordinating with DARPA and other teams. That is basically my role.

**Adam:** Nice. Awesome. Ziyi, why don't you go next?

**Ziyi:** My name is Ziyi and you can just call me Roland or Ziyi, both okay. And my role in the team is developing and design the program repair agent. And we need to automatically repair many different kinds of bugs and also we develop some kind of like a patch deduplication component. So we can try to cross validate if there is a patch that can fix multiple bugs.

**Adam:** Awesome. Great. Welcome Dang. How about you next?

**Dang:** Hey everyone. My name is Dang. You might also know me as Midas from some of my blog post maybe. I'm a second year PhD student at Northwestern and now I'm a member of 42-b3yond-6ug. So for AIxCC, I work on a few components. I do seed generation for fuzzing and bug triaging. So basically before fuzzing and after fuzzing. I also do some make some contributions to the whole infrastructure of the system. I am the main one who do the testing of the system.

**Adam:** Yeah, that's a big deal. Testing is a big deal. That's a huge part of it as we know. Great. Well, welcome. Xinqian?

**Xinqian:** Okay. Hello everyone. My name is Xinqian. Yeah, it's also very hard to pronounce. (Adam: I did my best. I'm sorry). Okay. and also a PhD student from Northwestern. In the AIxCC competition, I made it do in several components like a seed minimization and submitter and do the server evaluation and also have some test works.

**Adam:** Yeah. Awesome. Congrat awesome. Well, very happy to have you and we're a couple weeks out as we record this from the submission date. So, I guess the first question before we dive in, you guys did submit, right? Otherwise, I guess you probably wouldn't be here talking to us.

**Xinyu:** We do. We did.

**Adam:** All right. Great. Yes. You submitted something, right? That's I think the whole goal of every team is just submit something.

**Xinyu:** Yes.

**Adam:** Awesome.

**Yan:** There's the famous case from the Cyber Grand Challenge where a team that just submitted something that connected to the infrastructure and did anything small and then ceased to function would have done quite well. So, yeah. Yeah. Just showing up is half the battle. It's just like that Eminem song with the spaghetti thing. (Adam: I'm not sure. I don't know if that's the takeaway). Maybe it's not the exact takeaway, but yeah, maybe we can have Eminem on on the podcast next and ask.

**Adam:** Sure, that'd be great. Marshall Mathers, we have a standing invitation. You want to talk about capture the flags or any other types of things? We'd be happy to have you.

## Team Composition and Background

**Adam:** Cool. Okay. So then you've been spending to give slight background two years building this system. You guys were also one of the small business track teams. So you submitted to that, you won that and then you qualified as top seven and then spent the last year building your finals. So talk to us about what's the does 42-b3yond-6ug have 42 team members? I feel like that'd be good synergy.

**Xinyu:** So our team have most of the team member are grad students and university faculties and one of the common thing for the team members are majority of them are my students or my former students. So yeah when I heard about this competition I start to reach out to the people that I know. I was trying to reach out to you guys as well but I know like you're gonna compete. So, so I reach out to some people and they say, "Oh, we are interested in this." And then they form a team. We have at the very beginning we have a large team really really a lot of people. We have nearly like if I check my slack channel, we have almost like more than 50 people at the very beginning. But you know like when you have a big team is hard to manage and not all the people have the same schedule, it's hard to contribute therefore along this journey. So the team size shrunk with only a few key member or core member into it. So until the final we have about 15 people around 15 people who commit the code or participate all the meeting writing all the documents and decide what strategy we use. So we have about 15 people's inventory. So that is about the size of the team.

**Adam:** Wow. Great. Okay. Okay. So then when you said universities, so what universities are involved?

**Xinyu:** Yeah. So I would say like most of the students and the faculty come from Northwestern University and we also involve some other faculties from and grad student from other school. For example, we involve University of Waterloo in Canada. So they have really good you know expertise in kernel in semi-finals. So they help us a lot and we also involve professors from Utah, University of Utah which is very close to Arizona. So they also part of the team and we have students from there. We have faculty from UNH. We also have faculty from New Hampshire and because they have good knowledge about Java because the computation Java is part of the computation. None of none of us in Northwestern know Java that much. So we got a lot of help from them as well. So we also hire some programmers. Oh one more universities I forgot that. Yeah. So we have one faculty from University of Colorado and Boulder and he's also part of the team. He has a lot of experience on the exploitation although exploitation is not part of the game but you know some of the expertise like static analysis things could help. So we also bring universal Colorado. So this is basically the whole team. In addition to that we also hire some programmer not too many mostly from the industry they have industry experience because when we are building the system sometimes we need some industry engineering experience to help.

**Adam:** Yeah wow that's super cool so yeah so pretty I don't know sprawling isn't the right word but large team with a number of universities that are participating right?

**Xinyu:** Yes.

**Adam:** Wow, very cool. And I guess the funny thing is we talked with the Shellphish team, so I'll try to make some similarities for people. We also had about 15 16 kind of core members of the team, but the larger team is probably in the 30s or 40s just with just like you said, you have other people that wanted maybe to do one thing or one part and wanted to contribute, but not necessarily couldn't commit to doing this kind of full-time.

**Yan:** Yeah, it's interesting how there's a kind of convergence there in team design. I think on what we also saw in the cyber grand challenge as well if there are university teams both the makeup of the team and the size of the team they're much more flexible which is an interesting sort of property of universities in general.

**Adam:** That's true. Yeah, exactly. It'll be really interesting when we talk to the other teams to see if like academic teams tend more towards this kind of strong core with like other you know people still affiliated or if they you know I don't know I think that'll be super interesting but on the topic of diversity and designs maybe would you like to introduce to our listeners your cyber reasoning system so what's the name what's like the thousand-foot overall design look like?

## System Introduction: BugBuster

**Xinyu:** Sure. I think I will pass that to Dang because Dang is doing testing so he know he know he has shared the same knowledge with me.

**Adam:** I feel your pain. I that was what I got roped into for quals was writing. It was right about this time. It was right before the 4th of July. They were like guy professors we don't have anyone who's building a testing system but we don't have any bodies. And I was like I guess I'll do the CI and testing infrastructure. And I had to spend like four days figuring out how to even run their system. But then by the end I actually did know most of the components because you have to. So please if if only there was someone that kept saying testing testing testing testing.

**Dang:** Okay. So I'll introduce about our system. So I believe our system is named BugBuster. We don't use name very much internally. We just use it for I guess in the documentations and stuff for DARPA.

**Adam:** Wait, you have documentation?

**Dang:** Oh, for DARPA. For DARPA. Yeah.

## Design Philosophy

**Dang:** So like our design we have we combine traditional methods and LLMs. We don't try to use only LLMs. So we have fuzzings, we have static analysis. But we also have LLMs in patch generation seed generation. So the philosophy of our system design in the final is quite different from the semi-finals. So for the final we focus on making it stable and do testing very early. I think that is the key principle of us in the final. Yeah, so we try to keep it not not simple. It didn't end up simple but as simple as possible maybe. Yeah. We try to make it not too complicated like we don't try to come up with fancy ideas with LLMs. We don't strive ideas that we are not sure 100% that it would work properly. So we don't involve LLM in like critical task. So LLMs it plays more of a supportive role for traditional methods. So we use it to generate seeds so so that it can help with fuzzing. So fuzzing is a traditional method and LLM generates seeds to help it. The reason for that is we don't want like LLM shenanigans hallucinations to ruin the entire pipeline right so if it generates a bad seed then well whatever that seed is not going to contribute much but it doesn't ruin the fuzzing for example in patching though we do need to use LLM as the core and so we built a lot of validators and strategies around that to again minimize the possible issues with LLMs. Ziyi might know more on that. He can elaborate on that later. But yeah, testing is the main thing. We did testing very early even before the first exhibition round. Before DARPA even gave us the integration test project, before they gave us any testing APIs, we just come up with our own data set. We put a lot of efforts in preparing our own data set and do a lot of testing on that like all the time. Basically, we always have some test running and when we introduce new features, we just kill the current test and test again.

**Adam:** Nice. So, who's who drove that focus on testing?

**Dang:** I think Xinyu like at the very beginning of the final round like he told us that okay, he wants this to be like we focus a lot on testing. We want it to be stable because in the semi-finals we tested our system for like two days. That was that that was pretty terrible. But yeah.

**Xinyu:** Yeah. So I want to add something about the testing. So basically if you look at the industry software when you do the reviews at least you could have your engineer sitting behind when something bad happen you can go and intervene. But this competition is totally different. So there's no zero intervention that you can involved in the whole process. So therefore testing is super duper important. So that's why when we are developing this so we want to put more efforts and allocate more budget on testing. So this including like preparing the test cases having the people to take the code and also run it in a large scale because if we are talking about like only a single machine that is easy but if you talk about you know a large budget and running this in parallel that's is totally different story. So we spend a lot of time on that. We also spend a lot of money on that. But still I I have to say like even putting all this effort there's no guarantee there is no bug that will influence the performance of the CRS system. So we don't know that yet but I'm very very even though we put a lot of effort I'm still very worried about something could happen with a system that can completely break the whole pipeline and even like making the mistake. I'm not surprised if I see that when I see the final results, you know, it's in it's always in the in the wrong direction, right? So, you very seldom have a bug that will make everything better suddenly. There was a bug and so we found a billion bugs and fixed all the things, right? It's just somehow it's always makes things worse which is unfair.

**Adam:** And it kind of goes into like you know we were I think with with the captains of Shellphish we were having them guess you know what place they would get or whatever but even as we were doing that I was thinking like but it all depends on what the challenges are what you know random you know somebody's CRS hits a random bug in a project and then it's just out for that one target and so that could happen to any CRS like there's such crazy behavior here that it is you know it's building something that works even some of the time is impressive.

**Xinyu:** One thing that I learned from the semi-finals actually is like in the semi-finals we can see like who find the first block which team find the first block and we so I know like the some team is doing really really good at the beginning and then we catch up quickly and we go in parallel and later on when the at that time they call it the CP which is the the program the challenge that we they give us and when the new CP come up and we never ever see that I see like some teams and us like completely shut down and I don't know about I cannot say about the other team but after we diagnosed realized oh our system dead new target but some team I know like they are doing very very stable you can you can see for example like the team I see like they're very stable growing growing although they don't get the first blood but they are very stable so stability that is my hunch is like I think stability make the biggest difference that make the team win. So therefore in the final round I keep talking to the team don't make the things too complicated. The higher complicate the complexity you have the lower stability that we will have. So that will be a disaster. We have to always balance between this.

**Adam:** Nice. And that's the KISS principle. Keep it simple stupid. Awesome.

## System Workflow

**Adam:** Okay. So then can somebody walk us through? So what happens? So a let's say a new target comes into your cyber reasoning system right a repository what happens like what does your system do and maybe kind of walk us through the steps maybe in relation to who worked on what or I think it'd be super interesting to understand it from a kind of a lower level.

**Xinqian:** Okay so if a new task comes to the CRS firstly the there will be scheduler which will like distribute between the each components and send the task for to determine the task type. For example, is it a full task or delta task or a Java task and send it to different type of components. For example, if we got a like a delta type of task, we will send it to some fuzzers which including some general fuzzing and directed fuzzing. Yeah, because we have a delta. So we believe that delta fuzzing will help. Yes. And after some times of running the the fuzzers Oh okay. Yeah I forgot one point that we will also do some like a seed generations. Yeah. We have a seed generation based on a it will receive the repository of the task and then analyze the code and generate some initial seeds for the fuzzers.

**Adam:** And is this just like here's the information, generate me seeds? Is it generating like a script that generates seeds? Like what kind of a style are you using there?

**Xinqian:** Yeah, we generate a script that produce some seeds. Yeah.

**Adam:** Very cool. Yeah.

**Xinqian:** And then after fuzzing for a while, there may be some bugs that has been has been discovered and then we will send the send the POVs to a triage component. Yeah. which will determine the type of the bug and to determine if the bug is yeah it's reproducible and if there's a delta task it will determine that if it is it is related to the delta yeah because only in the delta tasks only the bugs that related to task related to the delta will be counted. Yeah. Okay. And then after triaging the patchers will receive this information that we found a bug and then we have the bug report. We have the sanitizer report and then the bug will the patch the patchers will try to patch these bugs.

**Adam:** And when you say patchers that means you had maybe several patching strategies that you're trying to use.

**Xinqian:** Yes, we have different patching strategies and also we will use different kind of models like GPT or Claude. Okay. Interesting. Yeah. And yeah if if some patches have been generated we will do a preliminary test at our side and if it's okay we just send it to the like competition server and to check the status. Yeah. because of like because that if you send a patch to the competition server, it will also return the results of the functionality test. So it can also be a oracle for our like for for for our patching components.

**Adam:** Awesome. Yeah. And and and also we have a dedicated handler for like a SARIF evaluations. Yeah. So I don't think we Let me just pause for one second or can somebody remind our listeners what the SARIF reports were? I think we did it but I kind of can't remember.

## SARIF Report Handling

**Xinqian:** Okay. So I would say SARIF reports is a kind of like JSON which describes some static analysis results. Yes. And yeah, it may like include some information like the type of the vulnerability that it detects and the code location of the like a buggy place. Yeah. And maybe there are some also like describes of the bug in in natural language.

**Adam:** Yeah, I see. Okay, cool. Okay. So then you have a SARIF report and your patches you maybe have generated a patch. So then what happens basically next?

**Xinqian:** Okay. So you know there's a task called a SARIF evaluation in this competition. Yeah the the the organizer will send our CRS some SARIF reports and some of them will are positive but some of them may be false false positives. Yeah. So when we received the SARIF report we were like also do some preliminary test preliminary analysis for the report and to check some to do some sanity check if the file that reported in the SARIF in the SARIF report exists in our repository. Yes. Because yeah because they they actually did this in the like in the dry run round two. They they just they send to they send a SARIF report to our CRS which includes a code location that never exist in the repository. So it will definitely be like false positive. But if you just feed this report to AI maybe the may think that ah it's like a reasonable so it it is a true positive. Yeah. So the naive method is not acceptable for this this kind of task. Yeah.

**Adam:** So, so after some basic evaluations we will move it to to another to another component which is a code slicing because we need to we need to confirm that if the star if the code locations in the SARIF report was reachable by the given harnesses.

**Adam:** Interesting. So more kind of sanity checking to see if those locations are even feasible.

**Xinqian:** Yes. Because like in their rule book they say that although if a bug is if there is a bug and it was reported in the SARIF report but it's not reachable by by the harnesses they provided it will be considered as a false positive. So we have this kind of check. Okay. So after this check we will send these information obtained obtained from the previous step to a directed fuzzer. Yeah because we need yeah we are in like yeah our strategy is that we we will confirm that there is a bug and can be triggered by some POV and we we will think we will confirm that this is a positive and those POVs come from the fuzzers.

**Adam:** So it's like you're trying to match the crashes then to the SARIF reports.

**Xinqian:** Yes. Very cool. So you've done you you mentioned matching to the POVs to the SARIFs. So that that confirms it fully. Then you do this in the worst case you basically ask the LLM with the reachability data is this a real bug?

**Xinqian:** Yeah, I I think yeah in worst case we will do nothing because if if you submit a an error result yeah they were minus our points.

**Adam:** See yeah so then the strategy so then would you say that the system design at least in this point is affected by the game strategy.

**Xinqian:** Yes.

**Adam:** Awesome. Okay. So then what does a system do? And I think we maybe talked a little bit earlier, but as as you're continuing to gather patches and crashes, like how does your system deal with that over time? So over the, you know, multiple hours of the

## Patch Deduplication Strategy

**Ziyi:** So that's the year introduced the patch deduplicator and reproducer. Yeah. So actually when we are working on the computation we found a very challenging stuff is like you know there always many POVs comes from fuzzers and actually it it's pretty hard to deduplicate all the POVs. So in the perfect scenario is like we can perfectly split all the POVs and we can divide it them to all different bugs but actually in the real world that's really really hard and very challenging. So our policy is like we we use we use a patching stuff to do the deduplication which is we generate the patch and we have a stage named patch deduplication which means we use a patch and try to use this patch to to fix different vulnerabilities in the same task and we can say like let's say we have vulnerability A and B and if A and B is actually they are the they are the same bug so our patch can fix A and B simultaneously so which actually becomes kind of like deduplication and also we also observe sometimes the the patch we we call it a super patch so a super patch sometimes can patch two different vulnerability and also we we we observe that the interesting stuff. Yeah.

**Adam:** Interesting. Can you tell us like when like what were cases where the LLM would create a super patch that would fix two like seemingly unrelated vulnerabilities.

**Ziyi:** Yeah, actually I think we observe we observed that from round two. Let's say we so we found a bug and also we found a zero day and we found like if we use our super patch that it it can just simultaneously fix the ground truth bug and the zero day bug. So that means this patch can simultaneous fix to different vulnerabilities. So previously we think like the duplication the the deduplication part is to verify if there is a so is to deduplicate different different POVs to a to a same bug but after that we found so sometimes the the super patch may have different impact on it. So the super patch has an impact.

**Adam:** But in if I was a open source maintainer and I received a PR that says this PR fixes two bugs, I wouldn't necessarily be upset about that. It could be even cool. Why why is the super patch a problem?

**Ziyi:** Yeah, because that actually relate to our submission policy. So we we always try to submit those patches that can cover the most bugs which means we don't want to submit let's say two to two exactly same patches which we think might you know affect our scores. So we we always try to check if the patch can can fix different groups of bugs or something like that.

**Adam:** Do you guys try to submit the super patches?

**Ziyi:** Yeah, actually is that wrong? We do submit the super patch.

**Adam:** Yeah, interesting. How do you kind of digging into this a bit more because I think at some point maybe I lost some piece of information. I remember correctly. But yeah, I would say that this design was also affected by the game rule. Yeah. represent because like there was a kind of thing called accuracy multiplier in the scoring algorithm and if you did too many like inaccuracy submissions it will significantly impact our scores. So for example if you have two ground truth bugs A and B and you have two patches patch A and patch B in the common in the general cases you submit these two patches and it got two valid submissions. But if you generate a super patch for one patch C which can repair A and B and then you submit the patch B again you will only you will receive two valid fixes and also one inaccuracy submission.

**Adam:** I see. So, so basically the two strategies to deal with that are you either make sure you only patch one bug at a time. So, you submit three patches in that case or you submit your super patch.

**Ziyi:** Yes.

**Adam:** That's interesting because I'm I think we I don't remember if we got into this with Shellphish, but the the Shellphish strategy was separating them as much as possible so that you know to avoid the same problem, just a different solution to it. Combining them as much as possible is a really interesting thing. I wonder if there's more synergy there with the LLM's reasoning capability. Maybe it can start getting into the thought process behind the bugs. Did you see any of that?

**Ziyi:** Okay. So, so I would say yeah, we we have tried the strategy that separated each box, but we find that we we find that our bugs in I mean the definition of bug in our CRS may be different to the like intended bug from the organizers. Yeah. Yes. So when we are doing some evaluations on our own side we find that one grown truth bug can produce like 20 or more more than 20 different kinds of POVs and in our CRS it will be considered that like 20 bugs and then it will be generated it it will generate 20 patches. Yeah. If we just submit this to the competition server, we will got like 19 inaccuracy submissions which is scare which is horrible. Yeah.

## AI-Based Bug Deduplication

**Adam:** And so for what you saw and I wonder if if doing more post-processing on this to try to you know identify oh we have this patch and they can be merged they're one bug versus their super patch if you merge them. Do you think that complicates the system too much?

**Dang:** I've been thinking a lot about this KISS philosophy that Adam I think in this case it's not keep it simple stupid because we're using AI now so everything is very smart it's keep it simple and stable. I think Dang have tried AI triage. Can you talk about that?

**Dang:** So like the deduplication is a big thing for for just for the scoring algorithm, right? So like we didn't do it early on but we have to do it later on because they release the the final scoring algorithm and they have penalties on duplications. So at first we tried to do the deduplication on the bugs themselves first like not deduplication the patch but the deduplication on the bugs and we we tried to use DARPA's provided deduplicator it didn't work very well because it's just a stack matching so we tried to do we tried to do LLMs to to deduplicate bugs and it seemed to work well in a few simple cases but then later on we found out that it has false positives. So when we give it two crashes for two different ground truth, it it actually say that those two come from the same ground truth and that will cause our patching agent to be super confused because like there are two different bugs like how can we fix it? It cannot fix it. So like so instead you fix them separately then you try to merge them. Is that the correct?

**Dang:** So in the very last not last minute but in the last round like right after round three we decided that we don't do the deduplication on bugs anymore. We put all of the crashes in the database and we let the patch agent patch all of them and then we do the post-processing on the patches and so in this case super patch is not super patch on the ground truth if it's actually super patch on our bugs. So we have a lot of bugs but they they a lot of them comes from the same ground truth. So if a patch can patch a large groups of those bugs in our definition, we believe that it is like a more it is more probable that that patch is the correct one because it fixes a lot of the same root cause. So this is really great because Yeah, exactly. and that will cause our patching agent to be super confused because like there are two different bugs like how can we fix it? It cannot fix it. So like so instead you fix them separately then you try to merge them. Is that the correct?

**Dang:** So in the very last not last minute but in the last round like right after round three we decided that we don't do the deduplication on bugs anymore. We put all of the crashes in the database and we let the patch agent patch all of them and then we do the post-processing on the patches and so in this case super patch is not super patch on the ground truth if it's actually super patch on our bugs. So we have a lot of bugs but they they a lot of them comes from the same ground truth. So if a patch can patch a large groups of those bugs in our definition, we believe that it is like a more it is more probable that that patch is the correct one because it fixes a lot of the same root cause. So this is really great because Yeah, exactly.

## Temporal Scoring Strategy

**Host:** I maybe we're going to say the same thing, Yan, but I I think maybe what the people at home don't realize because we probably we didn't get into the rules at such a deep level. There was a temporal component to your score, right? So submitting a POV, you had more points if you submitted it early, similar with a patch. So did that like is did you use that tradeoff of doing things fast versus waiting until you had enough POCs to generate a super patch to submit and how did you kind of find that balance?

**Dang:** Yeah, we kind of did it on the interval. So we postprocess patches on interval. Every interval we test a patch against every POCs of the same bug. That that is for for the patch. But for the bug submissions we just kind of just give in to to the rules. So the thing about deduplication in in bug submission in POV submission is that we are not penalized for deduplication but the submission that are taken into account is the latest one. So if we submitted multiple duplications only the last one counts and so we have a lower multiplier on on time. But yeah we didn't do anything about that. we just submit the all of the POVs.

**Host:** So, what about the risk of I wonder if you ran into this? What I experienced often with kind of LLM stuff in general is it works really well, but then if I give it too much data, the context windows too large, it like just gets overwhelmed and starts doing random stuff. How did you prevent that with the patch merging and the super patches? you probably have to process a lot more data. Because now you're reasoning about multiple parts of code, potentially multiple bugs. Did you find that effect at all? And and how did you kind of bypass it if you found it?

**Dang:** We actually don't try to generate super patch. We we only give one crash report to our patch agent at a time. But if it happens to generate a super patch because we have a post-processing to evaluate our patches, right? So if it happens to generate a super patch then we submit it like we don't force the patch agent to generate a super patch.

**Host:** I see. So you you patch once at a time and you evaluate them based on the the amount of crashes that they actually fixed even crash that they didn't necessarily see. Okay. I think this is actually then I misunderstood earlier. This is very similar to to the Shellfish route because basically what you're doing in some sense is patch-based deduplication. I I love this co-evolution. I I mentioned this in in previous podcasts, but I don't mean to say that your stuff's not impressive by by any means. It's super cool, right? And everyone came up with this independently. The really interesting thing with the you know contests like the CGC, the cyber grand challenge before this and and so on, right? is the convergent evolution of techniques that teams working in isolation for the same goal being you know completely without communication with each other end up with similar things. It's really cool.

**Dang:** Yeah. And I think that the other thing is also the game rules I think force this a little bit, right? because the I if I'm understanding it correctly, you're doing patch deduplication similar to how the organizers will do it at the end once they get everybody's POCs and everybody's patches, right?

**Host:** Cool. Yeah. So that it's it that makes sense too. I will say the one big difference at least that I've noticed is that I think our SARIF strategy was just LLM it and like that's it. Like I think that's it. Just just LLM it and the LLM I think in our test was right 65% of the time or something and so that's what we went with. Yeah, there was another another thought I had but it's it's it's gone for the moment.

## LLM Token Usage and Budget

**Xinyu:** Yeah, I can I can add something more. So regarding the regarding the LLM so one thing that's very interesting to me is like after the first round the DARPA actually released the the number of bugs so there is only one bug in the in the round one and the DARPA basically release like which team find it at what time and how many deduplication generated that's kind of data and in addition to that DARPA also release like the number the volume of tokens that has been consumed for the round one challenge and one thing that really worry about us at that time is like we see like our usage of token is significant lower than the average is like two times magnitude of difference from the average so we don't use that much you know LLM tokens and then they start to make us to think do we actually design our system correctly should we actually put more stuff into it and then we internally we have discussion shall we make a change or not and at that time our conclusion is like don't do anything at this moment so just keep it as it is maybe we will lose or maybe this is not the best strategy but we definitely would like to see how other team actually use LLM but it's really surprising why they are using so many tokens and I know some team they even complain to say oh the budget that you give us is not enough but for us it's like oh we still have a lot we it's not bothering us.

**Host:** This is a great point and this actually gets into the contest evolution from quals to finals Right. The quals budget was $100 in LLM credits for a specific target. And somebody will have to remind me. I don't know what the finals budget is, but it's significantly higher. 50,000 overall or 50,000. Yeah, that that's quite a lot. Yeah.

**Xinyu:** Even like I I do complain during the semifinal because at that time we have a kernel. I know like how much money we spend, how many token we need for kernel. And I talked to DARPA in in the you know one-on-one I say like oh this is too little so you should give more and they the answer they put back they send me back it's like this is one of the challenge you need to deal with and then at that time we start to think about how do we reduce the number the usage of the token and then all of a sudden in the final they say oh we give you more don't worry about it then but that's too late for us.

**Host:** When you said round one, you meant quals.

**Xinyu:** No, the round one means the the exhibition round. The exhibition round. Yes.

**Host:** Yeah. So, for those that don't know, I don't think we went into this before. The final event had three pre practice events. Basically, exhibition round one, two, and three. And these were you know, basically run basically practice of the final round. Because when you're building a system that needs to work autonomously, you can't just one-shot it. You need these practice rounds. And not only we need it, but the organizers need to build this infrastructure and they need it to understand the game and if the game is doing like and the rules are doing what they want it to do, right? And or like this thing like you know what if they if they had such a small like LLM budget that everyone hit the limit and the systems couldn't do anything. It's like that's not a good competition. And so yeah, I think it's a very important design decision that they did for going from quals to finals, whereas quals was like the one submission is all you got.

**Host:** Yeah. And and it's very I think it's a good example of of an evolution of a cutting edge challenge, right? We're not doing things like, hey, let we've had decades of car races. Let's improve the car, keep the track the same. both the track and the car being built at the same time. Which is a very interesting situation to be in. It was the same, you know, it's typically the same in almost every challenge runs because that's how cutting edge these challenges are trying to be. yeah, and so that's that's interesting in the the difference in LLM use.

## AI Model Preferences

**Host:** On this on this note, I just want to ask real quick, what's your favorite AI as a team? That's what I was going to ask, man. you've done not even as a team. I think there's interesting individually. What What is your system using exactly? What did you find is better at what thing? What do you personally use? Let's maybe start there. do you want to go first?

**Ziyi:** Yeah, I I think so in our system we so so we evaluate different models and we finally picked the GPT 4.1 and the Claude Opus which we think they are the most powerful and also we we we have we have an evaluation of that. So the Opus reaches the highest repair successful rate to to to our to our cases. We we have kind of like a data side. So we we do the evaluation. So the Opus I I think reaches the highest successful rate and also Sonnet Sonnet is a good one because it's really quick and relatively not such expensive. Yeah. Yeah. Yeah.

**Xinyu:** In my opinion, so it's really hard to answer which model is the better. The reason is it really depends how you use it. If you want to give a lot of information to AI, Opus is not a good idea because the Opus have you know smaller context window is not a good idea and if you care about the budget so say for example in the semi-final we only have $100 we even try Haiku. Haiku is cheaper that is one of the Claude series model it's cheaper but it's very very efficient but the accuracy is not that good but you can try multiple time and increase the accuracy but still the cost of using Haiku is low so it really depends on your strategy and but I overall if the budget is not your concern and you only care about the accuracy and I think Anthropic Claude model you in general give you better performance than OpenAI but It really depends on the task. So if you are trying to understand the code I would say like OpenAI is better or you know using the model to call different tool to chains OpenAI is doing better job. It really depends on the I think there's some room for scientific measurement here.

**Host:** I was going to say it's a very professor answer. I really liked it. It's also similar response if somebody asked you who your favorite PhD student is like well they're all good at different things so it depends on the task and the context. We all know that's not true. But yeah, no kidding. wait, wait. I want to hear from everyone else. Dang, what about you?

**Dang:** Yeah, so I guess again it depends on the the task, right? For for patching at the end, we use Claude, Opus, and GPT 4.1. But we use more Claude than GPT 4.1. So we we set like more budget for Claude. But for example for seed generation we we use a lot of different models because more more seeds is better right just if like different models we generate a more diverse set of seeds and that will be more helpful to fuzzing overall so we just use all of them we run them all in parallel so we run o3 mini we run 4.1 we run 4o oh we run Sonnet and just run all of them in parallel.

**Host:** Nice so then is your patching strategy also like running those models in parallel to try to generate patches or is it like serial but using one more than the other based on your budget?

**Dang:** We do run patch agents on parallel. Yeah, we have like let's say I don't remember exactly the exact amounts but like 8 to one like eight Claude to one GPT something like that. It's not the exact number but yeah.

**Host:** All right, Xinyu, do you have what's your favorite? You have to pick one. If I made you pick one AI model to use for the rest of your life right now, which one would it be?

**Xinyu:** Oh yeah. If you see in my day life, I will pick a Gemini because I have many like many smart devices in Google Home. So yeah, it can be so so Google Home can be a two core of the Gemini model.

**Host:** Nice. I like it. Very convenient. So, in a future episode of CTF radio, we need to do Marry Love Kill of of AI with the models. It would be awesome. Yeah. Our team was like highly Claude. We were very Claude and Anthropic. The credit card stuffed doll it turned out. Yeah. The Claude the Claude ant I believe. Is that what the or Anthropic I guess that makes sense of why that's an ant now that I say it out loud.

**Xinyu:** Yeah. The question that you guys ask is is very risky because you know OpenAI people and Anthropic may may watch this and then you know it's basically block us to work for them in the future.

**Host:** Exactly. That's what I that's what I was thinking. I don't know. I think you want the critics to work for you. That way you can make the models better and I'm sure you actually you already said that you have great test sets and data sets that you've used to evaluate these models so you understand what they're good for and bad for. And I think the other important thing that nobody stated but we should keep in mind right this is a snapshot in time right these models are continually being updated and actually on that note maybe you can talk about what did you see in the difference in the models from quals to finals.

## AI Evolution Over Time

**Xinyu:** Yeah we we try basically nearly old model for the past years and at that time I think remember if I remember correctly that was Claude 3 2.7 and then three and 3.1 3.2 2 3.5 3.7 and we we try all of them. One thing that made me start to believe AI will be a game-changer in cyber security is I observe they become it becomes smarter and smarter. So at the beginning I I basically don't trust AI at all to be honest the first day when I see this competition then my my first feeling is like let's use traditional approach to deal with it. But after the more like we try AI and after the AI got evolved then I start to make me to believe like AI can definitely do something and which can even do better job probably than than our human and I I do see there is a trend of changing significantly. So I'm so happy to see that and I I hope this is my my my on my wish list. I hope some days I can work with OpenAI, Anthropic or even like XAI, any large model companies and we can work together to make their model better because we have a lot of insight. We know like how to make them better. But but hopefully they will see they will hear what I say and then contact us.

**Host:** Great. It's it's super cool because these are it's it's very similar. I I have a feeling we're gonna hear something along these lines from every team is like, "Holy this stuff got good." And and I I agree like back when the AIC started, it was like, "You want us to do what?" Yeah, it's wild. And I think the the well maybe the thing I can't remember if we asked Will and Lucas about this Yan but the one reason we didn't use Gemini in our system is because we were never able to like get our limits set high enough to actually test it in our system and so we just used Claude. So, I'll be super interested if a team was able to bypass these like weird hurdles that are involved in using these models and was able and and a team says like Gemini is the best like hands down. Oh, and interestingly, there's the SEC Gemini that came out recently, right? So, I don't know if it's API queryable, but that might have been an interesting thing to investigate as well.

## System Architecture

**Host:** Cool. Okay. So I'd like to go back to kind of the architecture design because I think it was Dang you mentioned the database the seeds get put in the database. So did you have like a a centralized design? There was a central database was something like you I think somebody mentioned scheduler too. Was it coordinating all these various tasks and things? So can you talk to us about that that level of design?

**Dang:** Yeah, we do have a centralized database and we do have a kind of centralized that would send task to different components. We don't believe that it's the best but that is what we went with at the beginning and so like is it custom written or did you pick something off the shelf? The database is that your question? No, no, no. The scheduler the the scheduler we wrote it ourselves. Yeah. so like halfway through the competition like right around after round one we have some discussion on the overall infrastructure because we after round one we found some issues with this design but like at this point we cannot change the entire system. So we just went with it and tried to overcome those difficulties with that design. But yeah we do have centralized things. We don't believe that it's the best but that's what we went with.

**Host:** Nice. So can you talk about what some of the maybe either engine I mean it could be engineering tradeoffs of that centralized design it could be social tradeoffs like that's I I can tell you about the Shellfish system briefly but I'd love to hear from you guys what what like kind of those lessons learned were architecturally.

**Dang:** Yeah. So the way that the scheduler communicates with other components is through RabbitMQ. we choose RabbitMQ because we knew how to use it from the semi-finals and so we just keep using it but then we realize that it it kind of gets messy and if we only host one one port for RabbitMQ it might like when the system scale up to a certain point then it might overload that that port.

**Host:** I've never seen a RabbitMQ deployment I didn't regret.

**Dang:** Yeah, we kind of regret it, but you know, it is what it is. Yeah, at some point you just you just got to make it work. Yeah, because we we really cannot test with the scale that we will use for the competition rounds, right? We don't have that much budget during testing. So, we don't know if we scaled up to that point. Can RabbitMQ survives? So, yeah. but yeah so and also we we not only have RabbitMQ between and components later on as we develop new features we want components to communicate with each other and now components are creating more RabbitMQ connections and so it's just get messier and messier from there. Yeah, we we're just happy that and finally we make it work somehow.

**Host:** Well, I think that's honestly it's actually of I mean at a high level it's very similar to the Shellfish design. I mean there's we designed our because we're insane. We designed our own custom orchestration and it's kind of like a almost like a DAG where you have components that accept inputs and generate outputs and then once those outputs are ready like the component magically gets started and you can specify all this kind of stuff. But I think so we don't have a centralized database which scares the heck out of me especially with some of the bugs that we found in our custom you know crazy framework. But I think essentially you do have you have exactly the same problem like you have a component they need to like somebody needs to ingest the output of another component right so you need some kind of interface and then exactly like you said like okay but now other people need to use that or somebody in the middle is changing their component and now the downstream ones get like either need to they break or they need to get fixed and so yeah you guys I it sounds like just using queues as your messaging system between components while having the data stored in that centralized database and It's anything else you would have tried would have run into some issues. Right? In the CGC, we had a centralized database that implemented our queue. We had a jobs table and a blah that had a lot of issues.

**Dang:** Yeah. You just I I think I think this is just one of these kind of unsolved problems in computer science and anyone that claims that they have it solved has it solved for their specific toy use case that they struggle to have it solved for. Then you adapt it and it turns out it's Yeah. So basically we instead of trying some new things and get get new issues, we just try to fix our current issue basically.

**Host:** Well, it's Yeah. Yeah. I think everyone has to make that that call at some point like we just have to make this stuff work. I mean, kind of like you said, you know, the the keep it simple and stable philosophy, trying to trying to pivot away, you know, part like months before the end of a two-year competition, that that's that's risky.

## Fuzzing and AI Integration

**Host:** So in terms of of system design we talked a lot about patching, we talked a lot about deduplication of crash, we talked a lot about seed generation. We haven't talked a lot about the fuzzing itself. So you you use kind of this AI assistance to generate initial seeds for fuzzing. You use AI assistance to think about the the resulting crashes. What does that fuzzing component look like?

**Xinyu:** So I can talk about a little bit about fuzzing because fuzzing people is not here. So basically for the fuzzing we just use the the fuzzer existed fuzzing framework to do that. The only thing that we that we have AI into it are two there are two things that we introduce AI. Number one is the seed generation which we talked about earlier but more importantly is like we're basically leveraging a machine learning algorithm called the reinforcement learning which basically combine all the fuzzers together. So if we take a look at the fuzzer particular the research paper you know the tools there are just so many different research papers so many tools out there but different tool have different advantages for different target some target you may consider using tool A some target you may consider tool B but you know given given the competition you have no idea what kind of target you want to see so therefore our strategy is basically integrating all the fuzzers together and have a algorithm to schedule which fuzzer should be allocate more resources while doing the fuzzing. So we are basically doing that and even in the before the semi-final we test this approach on a Google sponsored fuzzing competition and we win the champion using that strategy we beat AFL AFL+ and so on and it's doing really really good and then they start to make us to believe then this is the strategy we should use. So that is basically about the fuzzing. We don't use too much LLM over there but scheduling using AI that is the key to make the fuzzing more efficient and have better coverage.

**Host:** So scheduling using AI is interesting. Why schedule? Like you can imagine a world where you have infinite compute. In that case you just spew out a ton of of fuzzing jobs. Why schedule in the AIC?

**Xinyu:** In AIC the budget is bounded. it's not unlimited resources but of course if we have unlimited resources we are happy to you know we don't need to worry about the scheduling but because of the limited resources we have to use that resources carefully and we cannot so we trust some of the fuzzer is better but we cannot fully trust that therefore we will have adaptive you know adjustment while we are going while the fuzzing is carry on.

**Host:** Very cool and so what were you using as the as the feedback loop for the reinforcement learning algorithm Was it seeds discovered like interesting inputs or is it crashes or were there I don't know maybe even further downstream like patches that came from that crashing input.

**Xinyu:** Okay so this is a very so this is a good question so the strategy the feedback is actually complicated but the high level idea is like this so I will use analogy to explain what happens so let's think about we have six people right now here and each of us have different expertise and right now we are taking taking a math contest. So we have math question and different people have different expertise but for some simple question we might everybody could do a good job but when we are seeing a hard part a hard question so it's going to take some of us longer time and some of the shorter time. So we based on the difficulty of the challenge and how quickly each of the fuzzer will be able to solve that then we will give higher you know more resources to that fuzzer. So this is dynamically adjust based on the difficulty of the target and also the time needed to address that challenge.

**Host:** That what I don't like about this is that in this scenario Adam would get all the resources. Definitely not true. I you're you're way more mathy than me. yeah and particularly I think the other super interesting thing there. So then what? So do you then that kind of inherently deals with the saturation problem kind of when you've saturated one fuzzer of inputs it kind of reverts to rand like trying the yeah if we we saturate at some time then we will basically re rearrange the resources we will randomly uniform distribute the resource and so that we can balance.

**Host:** Nice. Yeah that's awesome. We have a paper about that. So we will make that paper available even like a patch agent we submit paper to Usenix before the competition the final round got you also got it accepted before the final round.

**Xinyu:** Exactly exactly but I noticed it wasn't available until the submission deadline passed exactly I talked to the chair I say like oh we don't want to make this public available and the chair said okay I will put that into you know restricted access.

**Host:** Nice very cool awesome.

## Team Predictions and Strategy

**Host:** So from I mean, Adam, do do you have do we want to move on from the technical stuff? Like, yeah. Yeah, I think it's probably time. So, actually one more technical question. That's right. Out of everything you talked about and including things we didn't, maybe we forgot to touch on something. What is the biggest secret sauce of 42 Beyond Bug?

**Xinyu:** That's a good question, but it's not secret sauce if I say this. So it's nothing basically I can I can definitely share it. The biggest secret sauce is a stable and putting more resources on testing. That is the secret sauce. That is the only secret sauce that I have. So I'm the one who's trying to convince the whole team stability is the number one. Although many of them don't agree they want to do you know cutting edge research and they want to try this and that. They say I I basically get the paper every day from my team team members and they send me paper to say hey I see this paper and this published here it's doing great we should try this and I'm the bad person in the team to say stop doing that and focus the testing keep it simple so I would say the secret sauce for the team is testing and you know stability so that is the secret sauce I I don't think like we are outsmarts than other team like basically like teams All the team probably is going to be the same have the similar solution and some team might have a better but if you don't have stability everything is zero. So stability is definitely the most important things from my viewpoint.

**Host:** There's a very clear secret sauce from what you just said. It's you you create you that's right created the team and you have it's it's all people that you know you work with that you have worked with in the past. So, your convincing arguments were probably much more likely to land than if it was a random team member doing that.

**Xinyu:** Thank you. Thank you so much. I'm so happy to hear about that. Thank you.

**Host:** No, that's great. I have a a quick, you know, if you look at the the total amount at stake in the finals, it's like $8.5 million or something, right? There's seven teams, so the expected value, everything was random. Everyone's so good that it's just going to come out down to luck. Everyone's winning over a million bucks. What are you guys going to do with the money? wait. Stop. Before that, sorry. Before that, what place are you predicting that your team will make?

**Xinyu:** Oh, that that that's very hard question to be honest. So, when we decide to to participate, our goal of course everybody would love to win. But I I say this, I literally mean it. My goal of doing this is trying to explore. This is a great opportunity. I want to explore at the same time learn from other team and also gather experience from that and this is the most important things at that time. I have no idea like whether we will win or not but we put 100% of time our effort on that. I don't know how to answer this question. This is really really hard. I I hope we can win. But at the same time, I I I really mean it. I hope all the team will learn something from this, will get benefit from it, not just the dollar they take back home. But the money is important, but it's not the only important thing for this competition in my opinion.

**Host:** The real prize is the friends we make along the way.

**Xinyu:** Yeah, exactly. Like you guys, I I really enjoy like every time I talk to you guys. But for the people who are watching this they they probably don't know like I I have very good relationship with Adam and Yan. We we have a lot of research paper we publish a lot of research paper together and yeah so this is a fantastic you know friendship. Yeah. And also this is a great opportunity to learn you know from other team and get impressed by you know a sponsor the vendors who sponsor the competition. So that is all much more valuable than taking the money back home.

**Host:** Yeah, exactly. I think that's great great way to you know phrase it and and also I think the other thing that'll help that that learning aspect is the the fact that all the teams are forced to open source their systems. So you will be able to learn from all the systems and if somebody does have some crazy new design or technique or their patching system is just off the charts crazy good like we'll all be able to learn from that and go forward.

**Xinyu:** Exactly. Totally agree.

## Future Plans and Money

**Host:** All right. But assuming you do win, back to Yan's question, what are you going to do with the money?

**Xinyu:** So for us, we can we luckily we could have the money. What we will do is we're probably going to continue not probably I'm 100% sure I will continue along this line. More specifically, I would like to like what I said during this whole journey, we accumulate a lot of insight. We have a better understanding about the model. we have better understanding about the cyber security and we think we probably know how to make their model better. We definitely would like to work with the vendors like OpenAI, Anthropic, XAI like with Gemini we would love to work with them to make their model better but to do that is need the money it's need the so the API have the cost the infrastructure has cost GPU is expensive and student you who want to work in this product we need to get support we want to use the money for that purposes that is how we plan to use the.

**Host:** Nice yeah as a I can definitely share this because I and do it. But in the leadup to submission, I think we were using roughly 5,000 in anthropic credits a day on our internal testing and stuff. And so I just kept seeing like the credit card charges coming in. But like it's like, hey, you got to like you said, you got to test this stuff and make sure that it's working, right? And that changes that you're making don't break.

**Xinyu:** Exactly. That's not even counting compute. Yeah. Actually, the testing is very expensive. So it's cost us like 30% of the budget. not so that that's very very expensive. So my credit card you know so at the beginning when you are using API so you are in the very low tier and quickly go to the highest tier and then they they they handle your request very serious it's very expensive computation to be honestly which makes sense of why DARPA you know it's not they're not just funding it just to like incentivize people to do this but it actually is an expensive competition to be in.

**Host:** Yeah I posted I can share I posted in channel, we had like a $26,000 Azure bill that came in from all the tests that we were running towards the end. It's just kind of wild when you look at it like that.

## Academic Team Experience

**Host:** Awesome. Okay, so I have we're getting kind of close to the end. I have a little bit of a social question. So, as an academic team, how did you feel like competing in this kind of not academic kind of competition, right? It sounds like you're getting papers out of it, which is amazing. But how did I guess the team members balance the PhD with the the competition? I think it'd better have the team to answer that. So I if I answer that, this is my feeling. So I I you know I I do brains wash for quite a long time to convince them to compete. But but I really want to hear their real thoughts. Dang you want to go first?

**Dang:** Yeah, sure. I mean I am a bit anxious about not getting papers out for two years. I mean I I did got some paper out for the first year because like those are worked on before before AIC. But yeah, it's pretty anxious for me to not have papers out. But then again, I I think this is a great opportunity and everyone is giving their 100% for it. So I'm just going along with it. See how it goes. And because like like as Xinyu promised and I'm also think pretty sure we can make some paper out of the ideas that we had in this competition. So it's not like a complete tradeoff, right? We still have something out of it afterward. So yeah, I'll keep my promise for sure.

**Host:** I I love the dynamic on display. I think it's it's a very cool team dynamic. I think Adam mentioned it earlier too. It's great. Ziyi you want to say few words?

**Ziyi:** Okay. So, yeah, just like Dang and I I also like devoted almost all of my time to the AIC and was also anxious about the papers. Yeah. But but when they after our submission, we look back to our journey and we found that there are many things that can become some research ideas. So I think that's will also benefit our like academic studies and researches. Yes. And when we are doing the development we also found that the current solutions for like fuzzing or some other things are very limited and this will also like inspire us for some new ideas for academic researching.

**Host:** Nice. Xinqian you want to say few words?

**Xinqian:** Yeah, I yeah, I actually think it it's a really good opportunity because for AIC we have opportunities to dive in the whole system and try to think in depth like how can we use LLM for the cyber security and I and I do think there are many many tasks and many interesting problems that we can explore and we also we have seen some interesting problems and we will maybe publish some papers for for that. Yeah.

**Xinyu:** Yeah. I I want to add one more things. So although like most of student the research paper is definitely important and doing fantastic research is important for the student but along the journey there's a one thing that we will never ever gain if we don't participate that is the soft skill because at academia we will never ever have a chance to work to coordinate so many efforts you know in one project and making sure like we have to trust each other and so one. So only in this AIC journey for our students will be able to you know learn from this journey know how to trust each other even though sometime we have a disagree strong disagree but we know like we are not going to fight so we will you know work together we will communicate and making sure like everybody's on the same page those soft skill will never be ever to pick up if in in academia but this AIC journey give us that kind of chance to cultivate our student to let our student know how to work as a team and trust each other.

**Host:** Yeah, that's great. I mean that that's definitely echo all of those. I think the other thing is like this is a maybe a once in a PhD opportunity, right? So like not every PhD student gets an opportunity like this to compete in a competition like this. So I don't know. And I when we were talking to our PhD students, I was like are you guys crazy? Not even like thinking like I don't know. I'm just like heck yeah. like if if if this was happening like when I was a PhD student like jump right in. although I guess on the flip side you guys were doing the CGC but in my defense I was graduating so I said no thank you. I do not want any part of this craziness.

**Xinyu:** Yeah the the the team building the the that exposure to what what that need to deliver something real and functional is. For me it was life-changing in the CGC I think I mean it's actually the reason I became a professor I wasn't planning on academia before that you see you know supercharged that so I think you know you have to give up some papers during the the thing but you get that return on investment it's going to be awesome.

**Xinyu:** Yeah. So this year we have our team have the lowest number of publication across my entire career. But I think for me I think it's worth it. So we we are currently is catching up. So we hope like we could pop exactly same you know it's very very similar. And it just makes sense. It's an opportunity you have to pursue and you want to do it full-throated. But I think that's the other thing is like you you don't want to look back and be like oh well I published that one paper but man I didn't give everything I had to AIC like I really wish I had gone back.

## Lessons Learned

**Host:** So speaking of on that note is there anything now that you've done this two years later looking back what would you have done differently and it could be anything technical like I don't know is there something you look back like ah if I could do it all again I would probably change tweak this thing.

**Xinyu:** That's a good question. So I was I I definitely think about this in the past. The key here is because at that time that that time even like right now we are we have a shortage of budget. Well me I really want to touch the model and I think I have to I know how to do this make it better but the thing is like academia even like this much of a price money is not enough for us to run the GPU. That is the biggest regret that I have. If I can go back, I won't really want to. You're in luck because probably right as this airs, a meta recruiter is gonna kick down your door and kidnap you into their new AI team.

**Xinyu:** Please, they please, they should do it. Anybody else have thoughts on on things they'd maybe do differently?

**Xinqian:** Okay. So, if I go back to two years later, I will I will say like, I should embrace AI earlier. Yes, but after the semi after the semi-final we we started to like trust AI and use AI in our all components but if we find the potential of the AI earlier I think we will do better.

**Host:** Nice and especially now that Gemini is ruling your entire home so you definitely need to get used to AI. Yeah. Well, nothing really comes to mind for me. perfect. Also an AI hater two years ago, but yeah, I can't tell if this is the perfect response for a tester to say that like, nope, I would have done it all exactly the same thing. So, yeah, that's great. What about you Ziyi?

**Ziyi:** Yeah, I I actually agree with Xinqian because I I think I I should also embrace AI earlier. So so dating back to two years ago I I so at that time I I'm kind of like a so I really like those traditional techniques and very complicated to solve the problem and I I didn't expect using AI will change that much but after a so we all know the the power of the LLMs. Yeah. Yeah.

**Xinyu:** And by the way, I completely pivot our team from traditional. So my team originally do some AI. So I know in your team I have one graduate graduate student in your team and that's our one spy. Yeah, he's really good. And but I I do AI for many years and but at that time my strategy is like separate two group of people. People who work on AI, they work on AI. people working on traditional things work on traditional they talk to each other but not that intense but after so I completely merge them all together so they have to work everything have to relevant to the AI so that is the biggest change.

**Host:** Very cool that's great all right well thank you all so much for joining us today I think this was really I learned a ton so I really appreciate that all right and so now it's time to say goodbye so thanks for joining us today on the podcast so I'm Adam D you can find me online at Adam Dupe. He's Zardis. You can find him online at Zardis. Together we are CTF radio and you can find us online at CTFradio. take care and happy hacking.

**Team:** Thank you so much for having us.