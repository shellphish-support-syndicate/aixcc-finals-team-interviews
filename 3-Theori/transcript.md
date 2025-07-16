# AI Cyber Challenge Interview - Team Theori

[Video](https://www.youtube.com/watch?v=LTOyP_3aFP0&t=5133s)

## Introduction

**Adam:** Hello everyone. Welcome back to CTF radio. This is now going to be our third recording of talking to an AIxCC finals team. As always, I have with me the great Zardus. Zardus, say hi to the people.

**Yan:** Hello, hackers.

**Adam:** All right, great. See, this is what everyone wants. So, as mentioned, this is the third of hopefully seven videos and podcasts we're going to be recording about the AI cyber challenge. So, please go listen to the previous episodes. We may reference those things. We'll talk about the competition, but I don't want to waste time going into the details there because that would just be super boring continually going over that over and over.

**Yan**: Except for the details that relate to this team.

**Adam:** Of course! As things come up and maybe we'll even - I was actually thinking of prepping for this like how much did they get into modeling the game and if we need to go to like the level of the points that you get for various actions and the functions. But I guess we'll see where we go because I don't remember any of that. But I'm sure these nice people do. So Yan, why don't you introduce our guest team?

**Yan:**
Well, I would except for our guest team today doesn't need any introduction, but I'll introduce them anyways. We have Theori. Theori is a cyber security company of cyber security rock stars that have quite a lot of rep in the community and have also decided for some insane reason to spend years and years and years diving into this competition. Guys, I'll let you guys introduce yourselves personally and we can head on.

**Adam:** And you can also fix anything that Yan mentioned.

## Team Introductions

**Tyler:** Cool. I can start. So I'm Tyler. Tylerni7. I don't know, CTF player, security researcher person Theori. Yeah.

**Adam:** All right. Nice.

**Tim:** Gonna sound very similar. I'm Tim. Also CTF background, hacking background in general, and yeah, security researcher at Theori and co-lead of the AIxCC team with Tyler.

**Yan:** And you're no stranger to CTF radio either, not just CTF.

**Tyler:** That's true. Yeah. Also CTF radio alum.

**Adam:** Yeah. I was just going to say if I knew how to do any of this stuff, this is where in the corner there'd be like that YouTube button of the previous video, but I don't know how to do any of that and I don't want to learn. So, it's going to be adapt people can Google it.

**Tyler:** It's right here. Right here. If it doesn't, it's not there. It's something wrong with your computer.

**Adam:** Exactly. There you go. Exactly. Fix it. Yeah, that's great. And so, you want to rep your CTF teams, you know, to give the people a little more background.

**Tyler:** Yeah. So, Tim and I are both from Carnegie Mellon. So we played with the Plaid Parliament of Pwning. We were both team captains of PPP at different points in time. So PPP also recently has been playing the Defcon CTF merged with our Theori team as well as another team from one of our other PPP alum. So we've been playing under MMM but we've played Defcon CTF a lot of times. Won it a lot of times which is nice. We're very tired but keep doing it for whatever thing is wrong with us.

**Adam:** That's incredible. And I think at some point we'll have to talk about that because I'm finding myself and I know Yan went through this as you get older and older and your life circumstances change. It gets harder and harder to spend those weekends CTFing and justifying that to your family. But we're not here to talk about that. We're here to talk about another way I guess you waste your time on the nights and weekends.

**Tyler:** Exactly.

## Team Structure and Company Involvement

**Adam:** So this AI cyber challenge. So why don't you introduce us first to the Theori team? So what is kind of - because I think this is what it's a little hard for people on the outside to understand of what the team structure looks like and I think you guys are very interesting because you're our first industry team that we're talking to. So maybe if you want to talk to us about the team structure and like how that kind of relates to Theori's missions and goals and like why does the company let you do this?

**Tim:** Yeah, sure. So yeah, we are team Theori and we have eight members. Our company as a whole is kind of split between the US and South Korea and that is also reflected in our AIxCC team. So we have four in the US and four in Korea. And most of us come from the sort of CTF background but we have two people in Korea that have come from more of sort of an AI background. So nice. We had a little bit of AI experience and AI eval experience coming from that side which was nice. Yeah and so most of us were already with Theori before cyber grand challenge or sorry before AIxCC but we did hire two people to join us for the final round.

**Adam:** Nice. Specifically for... Yeah, that's very cool. We had similar I think I believe 42 beyond bug also did something similar of I think their case they were hiring software developers to help because they're an academic team so that definitely makes sense so then why why does a company participate in a grand challenge like this if you can share maybe the and it's okay to say because we convince them to that's also perfectly fine.

**Tyler:** I mean I think that's part of it so you know when this was announced three. And you know, we were like, "Oh, this looks cool." You know, we like hacking stuff. We like winning competitions. Maybe we'll do this. We were a little bit hesitant for a while because there was kind of - It took a while for some of the information to come out about like what exactly this was going to look like. And we're like, I'm not going to don't really want to commit to anything until we have a better idea. But then at some point, you know, they released enough that we're like, "Okay, like this looks pretty interesting." 

And I think our motivation was like, so I played in the Cyber Grand Challenge. I was on the team for all Secure Mayhem, where we won. And I think that was like I really liked the experience. I mean, it was a stressful, terrible time, but I loved it. 

**Adam:** Just like CTFs, like terrible, stressful time, but we won and I loved it. 

**Tyler:** The same mental illness that caused us to do that. But you know, I think yeah, so I was like maybe we should do this and it'll be fun and we can at least try to qualify. Our goal was kind of like we just had Tim and I work on it for the qualification round. We kind of waited until the last minute. So we only worked on it for around two months, maybe two and a half months.

**Yan:** It's a good return on investment because clearly you qualified and that's $2 million of a qualification prize.

**Tyler:** Yeah. So, we were like our hope was like we'll try to get to the point where we feel like we've made at least a 50% chance of qualification CRS and if we can get to that point in two months then like we'll be satisfied. Nice. And so that was kind of you know so it's easy to justify that from an ROI because we're not spending too much kind of resources on this. And then I guess personally it's also like this is kind of a brave new world of stuff out there and being on top of it is both like personally interesting and like as a company like trying to stay on the cutting edge of stuff I think makes sense.

## Qualification Strategy

**Adam:** Nice. Yeah, that's great. And then does this - we didn't prep you for this, but is this why then this kind of is matching with what I recall from your qual submission where you like focused on one target type. Is that right? Or two. I think was it you didn't do Linux? Is that right? Something.

**Tyler:** We didn't really do Linux. I think I mean the Linux one, you know, we looked at it. It's not that we didn't do it. It was more that we I think a lot of teams looked at everything and were like, if I can't solve all these challenges, I'm screwed. And I think for us, we were like, we can make a general solution that can work on everything but this Linux challenge. And the Linux challenge seems a little bit out of left field and we're just let's just not do that one. Like so, you know, we kind of handled it but it was never to a point where our CRS was like solving that and we were just like that's fine.

**Yan:** It's something that I observe a lot in any sort of competition attached to a conference especially any most competitions if there's a something that a 100 people are competing in doing an okay job can get you that top seven top three that that gets tougher and tougher top something is pretty easy.

**Tyler:** Our solution also ended up so you know we took a very general - we'll talk more about approach - But we took a pretty generic approach and my understanding they didn't release the official scores but in terms of all the metrics they released I think we did the best out of all the teams. So you know we still didn't get the Linux thing. But that's fine and that ended up working out.

**Tim:** Yeah, it was kind of interesting because I think the more generic approach we took ended up working better on Java than many team solutions because Java's harder to fuzz and sort of I expect the techniques that were being used were just less applicable to Java. So it ended up working out.

## System Overview

**Adam:** Yeah, that's great. Cool. Then let's maybe then we can dive in there. So can you give us like the high-level 10,000 foot overview? I guess does your cyber reasoning system have a name?

**Tim:** Yeah, so we we kind of we had to come up with a name so we did. The Theori CTF team is called the duck because in Korean is duck. So Theori is the duck. Tori is wow.

**Adam:** All right. Nice. I like it. 

**Tim:** So for AIxCC we decided to go with Robo-Duck because it's a automated version of our our CTF skills basically.

**Adam:** Love it. I love it. Awesome. Okay, so robot, which I guess now that we said it is not a term you actually use internally. It's just a the external name of the thing because you had to give it a name. 

**Tim:** It's in our read me. That's about it.

**Yan:** What do you What do you say internally?

**Yan (mixed):** The CRS. Yeah. Yeah. You broke the effing CRS. Is that just kind of the CRS escaped? The robo-duck is on the loose. Is a pretty good. Yeah. Yeah, that's pretty good. I can't wait until after the AIxCC where we get all of the like, oh no, what if the CRS's escape onto the open internet? I got a lot of that after the cyber grand challenge. I don't know if you did, Tyler, like concerned AI kind of so doomed people.

**Tyler:** This is like maybe not super relevant for this, but there's an anime called Summer Wars, and the anime is I don't know if it's specifically DARPA, but it's about a professor who makes a like a system for automated hacking and it like escapes. And there's also like a scene in the in the thing where like the background like it's not like B-roll footage, but like the background that they drew is clearly from Carnegie Mellon. And so like everyone who uses like this thing is like it's kind of canon that the professor was from Carnegie Mellon and it's just like this is real weird and really creepy.

**Adam:** When was it when did it come out?

**Tyler:** It came out like around the same time as CGC.

**Adam:** Oh, very cool. Yeah. Yeah. Very cool. Gets people thinking. Yeah. This is why you guys were so busy post CGC was fighting that CRS and making sure that And that's why it came back in the box. Yeah. It was in a cage in the Smithsonian so it wouldn't escape.

## Technical Architecture

**Adam:** Great. Okay. So then now that we know about the robo duck, what is like the high-level overview of your CRS? Like if you could kind of like paint us a picture of course with words because we are a podcast as well as video.

**Tim:** Yeah sure. Basically it's a bunch of Python a single process of Python in fact. So we have we have a sort of a distributed architecture but we have one central node which is running a single Python process and then a various like maybe 20 20 to 25 other hosts which are just running docker where the main hosts will just kind of send docker jobs to it. So we'll just spawn containers on remote docker hosts that perform any work that we need dedicated compute for. And sort of the high level overview is we went very hard on LLM agents. Very LLM heavy approach compared to other teams I would expect. We tried to instill a lot of what we think we would do as humans to solve these challenges and build agents that could that had the tools necessary to do what we would do, but not so open-ended that they could get sidetracked. So we have a lot of guard rails and a lot of like sort of handcoded like feedback from the the tools that the AIs use to try to steer them in the right direction if they're going off track. So this is sort of a high level overview.

**Yan:** This is super cool. So when we were talking to Shellphish I think hypothesized that there were two approaches to the AIxCC. One was the cyber reasoning system from the CGC which was very heavily fuzzing-based etc etc etc augmented with LLM assistance which is what shellphish and 42 beyond bug did and the other approach being the LLM first AI hacker person embedded in a CRS and it sounds like you guys went that second approach.

**Tyler:** I mean, I think our like our our qualifying submission, so we did have fuzzing in our qualifying submission, but we wrote everything, but like the fuzzing kind of came last. Like we literally wrote the whole CRS. It was working and then we're like, well, we should also fuzz because

**Yan:** Do you have the a fuzzer in your final?

**Tyler:** Yeah, we we so we still have fuzzing. But you know, if we turn fuzzing off, it's still that's that I'm not going to say it's great, but I mean we still find the same a good number of bugs. Yeah, I'm not sure how many we would lose if we turned off fuzzing. The late I mean latency wise might change things, but Mhm. 

**Adam:** Wow. Awesome. That's cool. And then so and then so is the whole I guess that the question then with fuzzing so is that a like an a tool that a the agents can use or is it something that's running separately and kind of feeding data that the agents can then pick up.

**Tyler:** I mean I think like Tim was saying we have a lot of feedback loops. So, it's it's I'm not going to say it's a mess, but it's a little bit of a mess where it's just kind of like, you know, if you're thinking about again like like a a human or anything, it's just like you have a bunch of stuff and the stuff is doing what the stuff needs to do, but sometimes you're like, I wish I had some information from that. So, I need like a channel there. I need something there. Oh, I should tell it to do this. So, this is part of why it's a single Python process is just that makes it really easy to kind of poke around in all these different directions.

**Yan:** And, sometimes you're analyzing multiple things at the same time in the contest, like multiple different programs. Is it one process per program?

**Tyler:** No, just one. That would be great, you know, but no, it's just one. I mean, I think part of the the rationale here was like, especially since we're so LM heavy, most we would hope that most of our our time is really spent kind of waiting for responses from LMS, waiting for a fuzzer to return. 

**Yan:** So, it's asynchronous. You dispatch these responses and you go and you collect.

## Reliability Concerns

**Yan:** A question that pops into my head and that's it's going to be uncomfortable. I apologize, but famously in the Cyber Grand Challenge, Mayhem, the the main processing loop fell behind the game over time. Are you worried about that with one process?

**Tyler:** Oh god. Yeah. I mean, there's a lot of things that we're worried about. I mean, I think like the main, you know, I'm sure we'll talk about stuff in general, but like the main thing that I worry about is our thing falling over. both because as software letting it run for like oh yeah we'll just run it for two weeks and like who who cares like you're fine it's like no that's really scary without like site reliability engineers that's how you run things in the real world and it's a little scary.

**Yan:** What's the longest you've run yours?

**Tyler:** So we we have run it for long periods of time (Tim: a little over a week maybe) and maybe something yeah but we also had to fix a lot of bugs along the way and new ones kept coming up (Tim: some memory leaks and) yeah yeah all all this stuff. So, are we worried about that? Yes, I'm very worried about that. We did a lot of testing. Hopefully

**Tim:** We did think about it a lot, too. Like our it is a single process, but if it crashes and restarts, everything should get picked back up. Like we have a a job database that tracks all the outstanding work and we tested that, you know, if we crash, it'll come back up and everything starts running happily again.

**Yan:** So of course Adam and I are also on the Shellphish team and in the final submission 15 minutes before the final deadline we got to ad hoc experience this that hey the CRL does restart when it crashes. Unfortunately it crashed again immediately and then it restarted and crashed and restarted and crashed. That was in the last 15 minutes we had to fix this. Not last 45 we fixed it was 45. It was 45. We noticed that it was crashing. We being the team, not me and Adam. (Adam: Well, very specifically three people on the team. I had to sit this out because it felt too much like running Defcon CTF) and we were very much not in that. So, you know, I bring this up for for actually a very specific reason. I've been when I talk about program analysis and and you know, traditional versus the the modern AI based the AI assisted etc. One thing that comes up is, you know, cyber using systems, they were brittle in the CGC. Insanely brittle. Mayhem very famously because you guys won, but and and and in the end there was that epic coast to victory. But these are the mechanical phish. Shellphish's entry crashed. I think the entire fourth place CRS fell over about a third of the way through. And like you know, there's all of these situations. Do you find like you're one Python process is there anything when you use LMS heavily can kind of the I I say this on purpose knowing that probably the answer is is something very cans help uncrash you like the AI going to say oh this is why we're crashing let's avoid this?

**Tyler:** No we don't have any no loop 

**Tim:** I did think about that briefly but I was like this is too much of a rabbit hole to be worth our time so yeah so

**Yan:** And and I think it's it's pretty interesting. One thing that's coming out of this, everyone is pretty concerned with the same brittleness question, right? Like what if AI does something insane and and and it gets around our baby proofing, right?

**Tyler:** Or I mean I I think the you know, if you look at some of the like the way the qualifier was set up, I think we like we handed them some code, but it's one instantiation of the code per challenge. Mhm. And I kind of like that a lot more because if it falls over, it falls over on one challenge. And the real issue for all this is like at some point you're running untrusted code. Like you have to run the code. You're I don't know how you're going to do this without running the code. So you have to run untrusted code. You have to run an arbitrary number of untrusted code things. And you don't even really know the shape of the untrusted code. You know it's written in C or Java and that's about it. and it can't fall over and it's got to stay running for several of these over like over a week and it's just like you know it's not that it's like I understand the constraint like I think it's reasonable but in some magical world maybe I'd prefer something where like maybe they task us for two days and then you get to log in and those challenges are done but you can clean everything up and then they're going to task you again a lot less stress there's 

**Yan:** it definitely feels like there is some middle ground that is we we lose a lot from this focus on autonomy basically. I think one thing that would have been interesting in the CGC is is exactly that right. So you log in you say oh this component fell over you can you can even apply a quick patch or something but these patches aren't quick.

**Tyler:** Yeah. Well we we even asked them we're like can you reboot us and they're like no like and which is fair like I you know makes sense. But it's just it's just the same thing where it's like the auton it's like not like I want to go in and like find bugs. I just want to be like can we let res like yeah our system will come back if it restarts but it doesn't come back if it gets really really slow. Right.

**Adam:** Yeah. And this this always reminds me you know in about a DARPA program that we were on where we had an evaluation phase and we had built a kind of more advanced cyber reason easing system and we get the results and like it completely failed like everything crashed and we're like wow why'd that happen and we looked into one of the challenges and it turns out there was a sym-link in some tarball where there had never been a sim link but the library we were using to untar it like didn't handle that and blew up. It's like this the stupidest little thing that like has no relationship to how well you're solving the core interesting problem, but is this like engineering thing and these unknown unknowns that can pop up when you're throwing untested, unknown software repos at your CRS.

**Yan:** And it kind of goes back into the competition of the competition because I I think no one in the competition would be upset. I mean, everyone people would be disappointed not winning or whatever, but no one would be upset being outplayed. Like there's a different solution that's just better. I think the upsetting the really truly upsetting thing would be my CRS fell over.

**Tyler:** Yep. Absolutely.

**Adam:** God, I mean, the thing that was terrifying our team was we found a bunch of POVs and patches, but for some reason our submitter failed to submit them to their system. Like that would that would be literally the worst is looking through those logs and seeing all these valid patches that and and and exploits that never got submitted.

**Tim:** Yep. Yep. So what makes it so stressful still keeping me up at night thinking about this. 

**Yan:** So a a afterwards sometime in September even before actually because you know functionally we're just waiting for the results. we we can create a group therapy session. Some in some sense CTF radio is a decynchronized group therapy session session. We were talking to 42 Beyond Bug and and they're like our core design philosophy. Our secret sauce is testing testing testing testing testing. That that's incredible. 

**Adam:** That's he says that's incredible because that was his push to the team which did not necessarily testing testing testing. But no 

**Tyler:** like we definitely did a lot and I think like especially I mean obvious we had some slight not disagree but like you know oh we should keep adding more stuff like there's obviously we have a long I mean there's infinite more things to add this is such a deep problem and it's like we really got to just stop because we keep making small bugs and these small bugs are really bad but we did a lot of testing and you know that CGC trauma is still there you know we spent a lot of our time like how do we make sure that like if this piece fails everything's fine. I mean that's also part of why we're like hey fuzzing doesn't work that's not a big deal like if the LLM doesn't work I mean okay it's a bit of a bigger deal but depending on which parts of the LM stuff isn't working you know as many kind of independent ways of doing everything as possible that hopefully can fail independently.

## System Workflow

**Adam:** Very cool. Yeah, this so then okay you talked so roughly how many so is it okay the main Python process would spin off different jobs and were those jobs essentially their own like agentic AI stuff that would then talk to LLMs and do stuff?

**Tim:** So yeah basically it was like a big asyncio loop so we have a bunch of in-process like asyncio tasks that are running like a lot of them are running LLM agents making you know request to the LLM providers. Other tasks are like trying to compile a project or trying to run a fuzzer and wait for the output. And those are typically like async waiting on a remote Docker job to to finish or something like that.

**Adam:** Cool. Okay. So then then take us through I think this will help kind of solidify things. So take us through so like a new repo arrives at your CRS. What happens?

**Tim:** Yeah, so I I think this is a fairly common answer. The first thing you need to do is build it. And you need to build it a bunch of different ways because these are based on OSS-fuzz and there's different sanitizers that you need to be running to try to detect different bugs. And we also utilize both coverage instrumentation and like dwarf debug info. One of our LLM agents was like a debugger agent. So it would like to inspect the program's runtime behavior. So we needed to also build everything with like a custom lib fuzzer like stuff that was an entry point that we could use for that. We also did well we also have additional building for like we use clang separately to try to pull out the source information like the basically like the cfg sort of thing. We don't really do well both for static analysis but also mostly for feeding good information about where code lives to the LMS. This is a great so many so many builds.

**Yan:** Yeah, it's it's a very common kind of challenge faced by all the teams and and did you guys look into non-clang solutions like Joern?

**Tim:** We also use Joern also use Joern.

**Tyler:** Cool. Yeah. Yep. I think but for most of those we use the so like clang produces you can run clang to produce the compile commands.json thing. So, we need to run clang first to get that or we need to run a build, pull that out, feed that to Joern, feed that to our other stuff. So, cool. 

**Yan:** What What do you use Jor versus claim for?

**Tim:** We can talk about I mean we can get into some please. Yeah. Yeah. We'll just build. So, you build stuff. Stuff is building. So, yeah, once we get the builds, the next step is well, it depends on the kind of task. So if it's a delta task then we will basically spin up an LLM agent to analyze the the diff that we're given and try to find vulnerabilities in it. If it's a full mode task we will run various static analysis techniques to try to find candidate vulnerabilities. So, we used infer as just kind of an off-the-shelf one, with a few tweaks, to fix some bugs in infer, to help find some bugs in our test projects. And then we also have, fully LLM, sort of static analysis pass where we basically throw every line of code at LLMs and ask it to find candidate vulnerabilities. 

**Tyler:** And, that also runs without a build, which is nice.

**Adam:** Yeah, that passes the build.

**Tim:** Yeah. So, we're running all of these different static analysis passes and we're getting thousands of candidate vulnerabilities per project, maybe even large projects. And this is way too much to like have an LLM agent look at each one. So we have a pipeline that tries to filter out false positives and narrow down to a set of I don't know 100 or or maybe less that we can spend a lot more resources on.

**Adam:** This is when you say resources you're specifically like LLM tokens like or is it Yeah. other types of analysis approaches?

**Tim:** Yeah, mostly just LLM spend.

## False Positive Filtering

**Adam & Yan:** Yeah. Nice. Wow. Okay. That's Yeah, it's different. Yeah. Well, yeah. So, the the first So, sorry to interject it. No, go ahead. Go ahead. Let's focus on on on on the system.

**Tyler:** Yeah. So, the first step that we do, so this we that kind of that filtering step that Tim was mentioning, there's basically like two phases. So, the first step is we use an LLM based classifier. So the basic idea is we give it kind of a bug report potentially annotated with a little bit of additional information. So sometimes we'll say like you know there's a buffer overflow when you called fubar here's a short description of foobar because it's not an agent so it can't go and fetch stuff. So we run that through an LLM classifier which just tries to output like yes or no. We think there's a bug and we use like the raw token probability outputs. So instead of just saying like binary yes no, we get like a a sliding scale of like 90% yes sounds great. In practice, it's a little bit of a bathtub curvy. So there's a lot of like absolutely and a lot of definitely nots and the middle is not so so great. But we still use this to grab the top n%. We default to like 20%.

**Yan:** Do you think and then opportunity there to be more granular? Not maybe not yes no, but like describe the reasoning and then analyze the percentages on on those parts.

**Tyler:** So part of the issue is like Tim was saying, let's say we have 10,000 things, right? At 10,000 things, we can't afford a lot of resources here. Yeah. And so like absolutely the performance is nicer if we are able to do something like use not a single token output. But the single token output is very cheap very fast. There's some other stuff that we were experimenting with but didn't really have time to do like we can do a couple slightly different classifiers because like you know part of the issue here that we kept running into is we don't just care about bugs that are real. We care about bugs that are real and that you can reach from one of the specific harnesses they gave us. Right. Right. Right. And that's a pretty big difference. So there's a lot there's kind of a lot going on there. But anyway, we get these top kind of 20%ish and then we feed those into kind of a first pass agent that we call like analyze vuln. And the idea there is not do any exploiting but just kind of look at it and just say like does this is this reachable like do we believe that we can reach this from a harness? Is this a real bug? Like do we like actually you know does it make sense to to call this a bug? And if so also annotate it with a little bit more information because some of our bug reports are like a little bit a little bit skimpy. And then when we kind of pass this down to the next phase, it'd be nice to have a little bit more of a description about what exactly is going on. So like what under what conditions can you trigger this bug? Things like.

**Adam:** Nice, and is it also like are you doing root cause or like bug classes or types? Or

**Tim:** not really bug classes, but we do ask the agent to output a root cause and the conditions required to trigger it.

**Adam:** Okay. Yeah. Cool. Nice. Wow. Okay. you can and that and that agent has like access to like runtime debug stuff and also the static analysis tool.

**Tyler:** So that agent is just static analysis based so it has access to static tools. So I guess one thing here okay (Yan: here you haven't started doing any anything dynamic so far at all). So we we potentially have I mean again it's kind of running in parallel so we don't know but but this at that point we do it would block if there's not a build completed. If a build failed, it would proceed, but if the builds, yeah. Anyway, so we use that basically because we don't give our agents something like a terminal. Like I know a lot of these like coding agents and stuff, they just have a terminal and it's like I want to find where I want, I'm going to use grep or I'm going to just CD into the directory. We really don't like that. It sound it's just there's too much going on. There's too many possible pathways. It's kind of confusing. So instead what we do is we give it a read-definition. So if it tells us a symbol we will find do our best to find that symbol and give that to it and nothing else. We also have find-references. So if it wants to know who's calling it it can find the references. We do give it the ability to read source code out of line. We really don't like it when it does that but sometimes it's required. And the tools I think especially the newer ones are probably more primed to do that and it but we try really hard to make it not do that. But there's no at this stage there's no dynamic information. Mhm. And then I know you can keep going Tim I guess.

**Tim:** Yeah sure. So this this vuln analyzer agent we by by the end of our development we were able to get it like surprisingly high integrity like very low false positive rate coming out of this agent. That's super it shocked us.

**Yan:** You guys have a Usenix paper?

**Tim:** No no not yet at least. I mean we talk about it. 

**Yan:** Sorry. Keep going. That that's a cool result.

**Tyler:** Yeah, I mean I think even even the scoring like one of the things we did originally is like we were running like this infer tool. You turn on like the buffer overflow thing. It tries to do like you know normal static analysis like bounds interval stuff. It's like great here's a 10,000 potential overflow and like yeah wonderful. We ran it with our just the scoring and it was something like in the top 100 results were like 10 out of the 11 or no no it was like it was like six out of the seven buffer overflows that we expected in the top 100 results. And so like and that was just the pretty cheap thing. And so again like you know it gets a little bit more complicated when we get more bug reports. They're not all from infer (Yan: and this is all without compilation). running static analysis was using infer uses compilation. Yeah. Yeah. But but this pipeline could be run. I mean it's it's it's only using the the compilation for kind of like silly code is hard to understand unless you have like ground truth about where code blocks live that could be done elsewhere. Yeah. Cool result. 

**Tim:** Yeah. So once we have this like very high signal set of vulnerabilities coming out we will pass those off to agents two different agents. So one of them is a POV reproducer. So it tries to basically write Python code to generate a binary input to one of the fuzzers that will trigger the vulnerability. And the other agent is the patcher agent and we will run those in parallel and then try to you know match them up later like make sure that it actually patches the vulnerability and stuff like that. So that's kind of the high-level overview of the LLM agent pipeline.

**Tyler:** Yeah. Wow. There's a there's a few other pieces around there like just like a lot of glue but I think that's kind of the more exciting part so we can focus on some of that stuff.

## Submission Logic and Game Strategy

**Adam:** Yeah. And then is there a piece at the end like how do you decide what to submit? So like patches, POVs, you come out like is there a game component that's deciding what to do?

**Tyler:** So I guess a one thing that I mean we heard a lot of people talking about like kind of this deduplication stuff. We we were kind of disappointed we we're pretty happy with our deduplication. So we use so part of this is like these things come through the pipeline. They are already kind of annotated with like we already have a bunch of descriptions about kind of what we're expecting. We also use similar agents when we get like a fuzz crash. We use similar agents to determine a root cause. If we only use an debugging comes in that comes in a couple places. But yeah, this actually does our I don't remember if our triager has a debugger. (Tim: Our triager has the debugger and the POV producer has the debugger to kind of figure out why it's not correctly triggering the bug yet). Yeah. So we'll we'll produce kind of these bug reports only if we weren't able to bucketize them otherwise. So like if a patch already fixed it, we're like it's probably the same bug that that patch was trying to fix. If it has a exact same stack hash or something, we're like whatever, we're not going to worry about that. But if it's some other intermediate thing, then we'll pass it to an LLM, ask it to try to understand what the root cause is. We get a bug description. We use another LLM classifier. We say here's the 10 bugs we found so far and their root causes. Does it match to any of these using the the same LLM classifier token like token probability thing? And so at the end of this we get a pretty clean database of here are like a root cause bug and associated with this root cause we have these POVs because we might get a bunch right like maybe we've from all sorts of sources we might have multiple patches for whatever reason and so it's not too hard to try to do something like okay well we're going to pick some POVs we're gonna pick some patches like match them up part of our stuff was like, well, when should we try to patch things that we don't have a POV for? Originally we didn't want to do this at all, but they kind of relaxed some of the rules around false stuff, which again, we were we're a little bit sad about because we were like, I think we're doing this root cause stuff better than other people seem to be. So we kind of wish that it was punished harder to to be our advantage. But but we still will do something where basically we we did like some quick math and it sounded like we do something like for every one patch that we submit that has a POV associated with it, we are willing to submit two other patches that we don't have a POV for. that ratio seemed I don't know some (Tim: I think even if all of those patches are incorrect that that the patches that we don't have a POV for even if they're all incorrect we'll still get like 90% of the 84% or something). So it seemed fine just kind of a game was just yeah and if basically any of them are correct it would be a net win. So it it felt like a good trade-off.

**Yan:** that I you guys might be the first team we've talked to that makes patches for things they don't have POV score. That's a very interesting strategy.

**Tim:** Yeah. Well, I don't know. We we weren't doing that until somewhat recently whenever the scoring algorithm was changed a little bit. So yeah. Yeah. 

**Adam:** But I think also the way that you filter down I'm trying to think some other teams have the 100 candidates thing. 100 seems to be a very common number but I don't think anyone really filters beyond that without trying to trigger dynamically so far.

**Tyler:** Yeah. Yeah. Yeah. So I would say like we probably get like the things that we patch, we probably are patching dozens. Like I think by the the final stage of that kind of filtering step like Tim said, it's it's very good about true true positives and not many false positives. We get like on some like we'll run on some things and maybe there's one false positive that makes it through. We'll run on others and there's m maybe 50% false positives, but we've never run and had like 80% false positives. Again, who knows what we're going to see next, but yeah.

**Yan:** Yeah, it could be could be the secret weapon or it could cost you 16% of your points.

**Tyler:** Yep. Yeah, I guess that's the worst case. 

**Adam:** You got to play the game, right? Or you got to I mean the other thing that at least the team was thinking about is like do we want to lose and not submit these patches that we have and like translating it to your case right it's like or do we want to lose because we submitted the patches that our system made right like you know it's kind of like you'd rather not kind of rather not lose by not playing the game.

**Tim:** Yeah. And it's a bit unfortunate too because like like we said the filtering like we were getting very good results from it. So it is like we have probably at least 50% of those patches that we're producing are valid bugs, but it might be that they're not scorable because no team produces a POV for them. And so by the rules it's not a valid patch because there's no known crash for it. So that is another concern we had which is like 

**Yan:** that's tricky because those are the hard blocks to trigger, right?

**Tyler:** We we definitely had cases like we especially so some of this we didn't see a lot of this until we were looking at stuff afterwards because we're like oh like we've ran a bunch of tests and spent tens of thousands of dollars on LLMS and like I guess we might as well look at these results and we're looking at them and like we have a lot of bugs that were not added bugs and those are like you know maybe they're upstream or whatever. Again, some of them are triggerable, some of them our system was not able to trigger. And so it's like, well, if those were too hard for any other team to get, but it's a real bug and we really patched it. And I was like, this is kind of kind of feels.

**Adam:** Yeah. So, this is this is great. And I think this is probably I don't think we dug into this much of depth, but essentially and you guys can correct me if I'm wrong. But essentially like the way it's like a post-processing step that the organizers are doing after a round to decide what actually are the POVs and the patches that are correct. And so if a team submits a patch, it's only a valid patch if it fixes somebody's POV that actually crashes it. So, if you submitted a patch, even for something that's a real bug, but you didn't have the dynamic input to trigger it, then it would technically be considered a nonvalid patch, which is kind of wild. I've never thought about it from that perspective.

**Tyler:** Yeah, I think there's Oh, no. Go ahead. I was going to say there's I don't know exactly how it might work. Like if we're very optimistic, we might say that some lovely person on the downstream DARPA side is going to be like maybe this was such a good patch and a real bug and we will add this into the set of original POVs because DARPA is also able to provide like ground truth POVs. And you know even if no team found it, if it was a real bug that they had inserted and there was a POV for it, then that counts. Don't really know how that can or would work and I doesn't really matter. It doesn't change anything we do. just make us less sad.

**Yan:** I guess if you're talking about 0 days, the kind of immediate question of course people have like did you report these bugs upstream? Or do you plan to? I mean understand until now it's been all hands on deck getting this system going.

**Tyler:** So we're we're looking at some of them. We need to like do a bit more triage and try to understand them a bit better. So some of them it's like well maybe this so for the competition all we need to do is crash right and that's not necessarily like a real security bug in all cases. So it may be interesting but like we we told our system it's it's goal is to find things that can cause crashes right if it finds a null-dereference fine. If it finds an off by one fine but yeah we'll we need to look more at them too. So we haven't yet.

**Yan:** Lacking an actual proof of vulnerability, you're stuck with the triaging problem, which is exactly what our personal experience reporting bugs to Yeah. firmware vendors and other types of things. They're like, "Oh yeah, this is a static analysis report. Yeah, give me a POV, otherwise like I'm not going to look at this."

## POV Production and Fuzzing Integration

**Tyler:** Your Yeah. So our our POV producer though also does a like it kind of does a shockingly good job I think. So again this is we changed it a lot since our qualifying round but this I mean this was a similar pipeline to what we had in the qualifying round where we just kind of look at it and then ask an LLM to write a POV for it. And I mean part of it is it's really good at the things that fuzzing is really bad at. So, you know, stuff like, okay, here's like a bunch of like URL stuff. It needs to be like a well-formed URL and you need to do all this like whatever parsing stuff or some other string thing or even like some really kind of weird binary format. You know, maybe a fuzzer gets stuck. So like we you know some of the stuff that we've seen what it'll find bugs and but exploit is kind of a weak word but it'll it'll pov them trigger them and like the fuzzer never even got to that function and so that's kind of kind of cool.

**Yan:** You also there's a feedback loop with the fuzzer where you produce so yeah 

**Tyler:** there's a couple feedback loops. So the first one is basically from the fuzzer or sorry from the from the POV producer to the fuzzer. So basically during its lifetime it has a bunch of candidate things that it might do like maybe it says like okay this I I think I made a valid POV I test it that was not a valid POV. What we do is we ship that off to the fuzzer and we're like hey this probably a good seed for fuzzing because it was trying to do something relevant and hopefully deep. So that's useful.

**Yan:** You observe that having utility.

**Tyler:** Yeah. So, we've totally seen cases where like our POV producer like even our POV producer works, it's going to make it to the end, it started off with something bad, submits it to the fuzzer, and the fuzzer beats it. Because it goes off to the fuzzing and it was like a couple bytes off or like it needed something really silly.

**Adam:** That's so cool. It kind of speaks to something about like it's clearly if you think of like the search space, it's clearly able to get a point around there that then the fuzzer is able to explore quickly that area once the fuzzer is given kind of that.

**Tyler:** I mean I think like fundamentally it feel like obviously you can you can argue about this especially for like pure static symbolic execution but symbolic execution concolic execution and fuzzing are very much search exploration strategies as opposed to like I think there's a bug you're I want to trigger that bug, you know, that's not really like you can do stuff to try to guide things, but that's not really what they're for. And having kind of a completely independent approach that is like that I think is really interesting.

## Agent Architecture Deep Dive

**Adam:** Yeah, this is great. Okay, so can you maybe talk about the shape of the CRS? Like how many agents are we talking about? Do you have a rough like I we didn't ask this to the other team, we should have, but rough order of magnitude of like code size. Like how big is this? Is this how Yeah, how much of it is prompt? Do you have a prompt pl?

**Tyler:** So we have I I like I'm working on some presentation stuff. So I have been collecting some of these things too for that. (Adam: So so you can justify all the AI like the anthropic credits that you've been spending on Theori's behalf). (Yan: Present to the shareholders). Exactly. So our our code isn't I mean I thought it was reasonably sized but I heard that your CRS is 270,000 lines.

**Yan:** So, I made this statement on the podcast. There's 270,000 lines in the repo. We vendor in some of the some of the dependency libraries. But I think it is not so far off of that. Jesus, it's it's somehow very massive. 

**Tyler:** Ours is around 20,000 lines of Python. We have maybe a couple thousand lines of like other like Rust stuff like some of our writing everything in Python. Sometimes things are slow. So there's a little bit of rust. We have around 2,000 lines of prompts. I think some of that might be duplicate, but I'm not 100% sure. I haven't totally a small amount. Yeah. But yeah, it's not I mean, a lot of the stuff is stuff that was written, thrown out, rewritten, thrown out, rewritten as opposed to just adding stuff on. Yeah. So, I guess we can go through our the agents that we have.

**Adam:** Yeah, that would be super cool if you could 

**Tyler:** maybe we have our diff agent which looks at a at a diff for a delta mode task kind of easy. We have our debug agent. So to mention both for triaging and for the POV production can run either GDB or JDB like Java debugger commands to try to get something a POV producer agent which does that the I haven't talked about this and it's kind of important the harness input encoder agent you want to talk about that Tim?

**Tim:** Yeah, sure. So, this is kind of a a sub agent of the POV producer. And as I mentioned earlier, our POV producer, it writes Python code to generate a binary input to the fuzzer. But we found that just giving it that task is a little bit too open-ended and it can spend a lot of its context window just trying to like write a basic bit of Python that can encode valid inputs, right? So we kind of split off that part of it into a sub agent. Were you gonna say that? 

**Tyler:** I'll just interject briefly with one of the other issues that we saw early on like when we got the original Jenkins task. We tried like the first thing we do is like all right like what if we just tell the LM to write an exploit for this and it's like great this is running on a web server. I'm going to import requests and send an HTTP request to the web server. And we're like you have totally misunderstood what we're trying to do here, right? We're not trying to talk to a web server and like you're not writing a PoC for this thing that's running. You need to write an input to the fuzzer thing. So that's Yeah. Anyway, keep going too. Sorry.

**Tim:** Yeah. So this is kind of like the guard rails and like the we we try to make every agent as narrow as possible. So we give we have the sub agent which is just creating a harness input encoder which is a Python function that takes semantically meaningful arguments about what the input should do and encodes them into the binary format that the fuzzer expects and it will basically iterate on this and do some like runtime checking that it is encoding correctly and then return this Python function to the POV producer to use to create its actual POV.

**Tyler:** That one gets the debugger as well, I guess, because that one is allowed it we basically if it a common example is like curl. I remember looking at curl and it has like this TLV structure or something where you get a bunch of stuff. What our input encoder does is it's like great I'm going to break this out into like four strings. There's a URL, there's like a username and a password and a response. just give me those four strings and I'll do I'll make the correct input for for it so you have an easier task. But we want to make sure that it's encoded properly. So we ask the input encoder as it's developing this run a debugger like send a user name into this thing and like break there and just make sure that like the right string showed up because that doesn't always happen.

**Adam:** Interesting. Very cool. So like a har you're like harnessing on top of the harness like you're adding other layers on top of the harnesses in some sense but dynamically.

**Tyler:** yeah it's kind of like abstracting or adding semantic meaning because like a blob of bytes is just not very useful. I think a lot of people who write CTF challenges or write write CTF solutions, one of the first things you do as you're writing this is like I'm going to write the interactor script. And I think in some ways it's kind of like you're writing the interactor script where like I need to interact with this thing and there's some whatever mystery stuff in the middle there that I don't want to think about. Please abstract that away from me.

**Tim:** Yeah. And one one other interesting note on this is that it's not specific to the POV that we're trying to produce. it's only it's specific to the harness and so any POV that we try to trigger through this harness we can use the same encoder function and we can actually like as soon as we have a a compiled project we can spin off an agent to start producing this encoder function before we even have a candidate vulnerability so it's kind of ready to go whenever we need it nice.

**Tyler:** so then our next agent is our patcher agent pretty straightforward does the actual patching the one after that we got our source questions agent. So this is kind of another thing it it's kind of like the input encoder. So the basic idea here for our POV producer. So, one of the things I guess you you all have experience with this, but maybe not all the listeners do where like you have a task relatively like maybe straightforward task, but it's going to need a lot of context and that's really unfortunate. And so, one of the things that we do is our POV producer does not have the ability to read source code. We do not give it source code reading tools. instead it can ask source code questions to another agent. And so the idea here is like that agent that it spins forks off that can use you know whatever 60,000 tokens and then it's going to return a answer to the question which is going to be 100 tokens and then all that context goes away. So you know I think there's a couple like we could use context compression. We used context compression in the qualifier round. And it it's fine, it works, but it's also just it's it's hard and there's a lot of weird questions around it. But we found that doing breaking our stuff up like this, we really didn't need it for the POV producer. So, so yeah, the POV producer can ask source code questions. It can ask debugger questions. It doesn't use the debugger directly. It spawns off an agent to do the debugging and it can like test a POV. And I think that's I think that's about it. That's basically it. So it's very limited to like a high level. Oh, it can get an input encoder. That's the only one. So it's a very high level sort of thing. yeah. So the source questions agent or triage agent which we mentioned does the the triage stuff. a deduplication classifier to kind of mention that. function summarizer that's basically just doing a brief thing where for some of our bug reports it will say like the bug exists in a call to foobar I'm going to just summarize foobar so that you can understand like with a single little bit of context why you care about that our vulnerability classifier which is thing we talked about before and the vuln analyzer agent so those two things make up that kind of filter step. Our harness input decoder. So yeah, I guess I don't know talking a lot. Tim can go describe that again.

**Tim:** Sure. As the name suggests, I guess a decoder is the opposite of an encoder. So what this tries to do is take an input to one of the harnesses, so this binary fuzzing seed basically, and decode it into its semantically meaningful representation. So it's also a Python function that takes a binary input and outputs some structured Python dictionary like nested object that is sort of the inverse of the encoder function, but it's something that we can present to LLMs to help them understand what an input is supposed to do in this harness. And we use this this decoded representation in our patcher and also in another agent which I think Tyler will probably get to soon.

**Tyler:** Yeah. Yeah. So the the next agent is our branch flipper agent. So this is another thing that we didn't talk about for fuzzing. But basically the idea is I mean obviously if you're fuzzing sometimes you hit kind of these places where you get stuck. So we have this agent which goes in and if it there's kind of some other pipeline in front of it that tries to find candidates based on coverage. We also do a quick classification before this using another LLM classifier to basically say like that's like a hard-coded flag. You're never going to be able to flip that from a thing. So don't even don't bother spinning up an agent because we're going to waste all the money. So that but yeah basically we'll say hey we have an input. The input gets to foo. Foo calls bar statically, but we have never seen bar get hit. Please take this input which reaches foo and transmute it into something that calls bar. Kind of works. So like it I would say roughly I think maybe 15% of the requests that it gets it succeeds on given that we're usually using a pretty saturated corpus. So we also like I guess I didn't talk about the corpus matching. It's not an agent but whatever. We do some stuff. So like our our fuzzing we expect to be like pretty solid starting point and we've still seen this get to new coverage places. So that's pretty cool.

**Adam:** Yeah that's awesome. That is like a LLM driller kind of a thing, right?

**Tyler:** Yeah, exactly. It's the exact same thing of like I want to unstick you. We're too lazy to integrate symbolic execution here. Maybe we can just throw an LLM at it. well, it works on the alng on you know C and Java and you don't have to worry about all that mess. 

**Yan:** First of all, and then second of all with these super real world applications, I think there is a very good question of can it symbolic execution even work in its current form.

**Tyler:** Yeah. That's about it. The the other thing that remains is our are our stuff for looking like the initial static analysis stuff of trying to say like are there bugs in this code where it looks at all the stuff. Those are those are our agents.

**Adam:** Oh, awesome. Portrait of a CRS. I loved it. Great. So then now that you've walked us through there, what would you consider to be our CRS's secret sauce? I think I know what it is, but you guys should tell tell our listeners what you think it is.

## Secret Sauce and Model Performance

**Tim:** I don't know. We may have different answers. We'll wait. (Adam: We'll separate you into two rooms and you can tell us your answers and we'll verify that. Just kidding). It's kind of hard to pick one, but I think if I had to, it would be the the false positive filtering. the the classifier plus this vone analyzer agent that outputs bugs which with very high signal roughly 50% false positive rate is very usable compared to what we're getting from these static analysis tools where it's like 99% false positives

**Tyler:**  I wish it was 99% not 99.99%. yeah yeah I guess I think I mean it's similar vein but just that the the LLM the pure LM pipline line I think is our the thing that if it if it works and we don't fall over then and we do well then it's probably going to be because of that.

**Adam:** Yeah. And I think one of the that as you were talking about it did you notice your performance improving as the models got better and better? Like was there a you could point to like oh shit we moved from [claude] 3.5 to 3.7 to four and now whatever our our performance is much better.

**Tyler:** There's definitely a decent amount of that. So I think like yeah there some of the models definitely do better. None of this has been like all of the bug like it was failing totally and now it's succeeding or else we probably wouldn't have been pursuing it as a as a route. But I know like even when we were just doing the qualifier, one of like there were a couple bugs where you know we started off running 40 because that was like the best model at the time and then sonnet 3.5 came out and something that went from like a maybe a 5% success rate went to like a 90% success rate. So there's I think there's a lot of it's usually a lot of individual bugs where like that individual bug has something difficult about triggering it and like it's just doing really poorly. Maybe it gets it 10% of the time and then some there's some new model and that succeeds. So we also do a couple things like like the POV producer. We actually run that with Sonnet 3.5, we run it with Sonnet 4 and we run it with o3. So, we run all three of those in parallel.

**Adam:** That was just gonna be what I was gonna ask. So, with all these agents, like how are you do you pre-allocate budget to each of them of what they can use of the models? Is it a more of a central thing? Is it dynamic? Is 

**Tim:** Yeah, that was one of the last things we we added actually because we were like doing some test runs like (Adam: Gotcha. That's also the terrifying part because you're making changes to what you're allowed to do). Yeah. Yeah. But, you know, if we didn't do it, what would have happened is we would run out of budget on the first couple of days and then we would not be able to participate in the last couple of (Tyler: To be fair, Tim, that still might have happened). I know. Yeah. Yeah. 

**Adam:** And so, what was in your tests? Like, did you have a ? You've mentioned I think four models there. I noticed none of them were a Gemini model.

**Tyler:** So yeah, right now we only use Gemini for our we use it for the full like the static analysis stuff. We use it a little bit there. Part of it is just especially early on like the rate limits there were not enough for us to really test with. We did some testing. All of our stuff is like very agent-based and some of the earlier Gemini stuff we just didn't have good the tool use didn't seem very good for us. So, we just kind of didn't think about it much. So we we ended up with a little bit of of Gemini stuff, but not much.

**Yan:** What's your your favorite AI?


**Tyler:** I've been watching these questions coming. You keep asking them. 

**Adam:** Yeah, we do want to know because I think it's it's funny. I you know, I don't know if it's I'm not sure how people are getting to this point, but there's definitely people that are like, I love this model and I'm just like, what? Like, I don't know. It's fine. Do you guys have favorite models?

**Tyler:** I say we we really liked Sonnet 3.5 for a very long time. So, we had we only basically stopped using it. Not like even when 3.7 came out, 3.7 wasn't really better for a lot of our stuff. Sonnet 4 seemed to be most like I think Sonnet 4 is just better. Not 100% sure. And then we really like o3. I should stop saying we I really like o3. We didn't use it for a long time because it's like way too expensive, but then they did that 80% price reduction like a couple months ago and suddenly we're like, "Oh, this is great." So we use o3 a lot.

**Adam:** Awesome. Tim, what about you? You're on a desert island with one LLM model. What are you choosing?

**Tim:** Yeah. If I had to pick one, it would it would be o3 right now. It definitely would have been Sonnet 3.5 a few months ago. And if price is a factor, it might still be Sonnet 3.5 or Sonnet 4, but o3 is a surprisingly good model for the price after the reduction. Yeah. So, surprisingly also o4 Mini gets you a lot of the way to o3 for cheaper on some of our tasks. So we also used o4-mini when o3 was prohibitively expensive for some tasks.

## AI Outlook and Development

**Adam:** Nice. Very cool. All right. So then how so you've been I think for your team specifically I think there's the question of how has your outlook on AI changed throughout this? It sounds like you went in with a very AI forward approach for quals. Are you still are you more bullish having worked on this for two years?

**Tyler:** So, I think like before Quals, I'm not sure that I was necessarily like an AI believer. It was more just like if I'm going to do this and I might as well just go the LLM route because it sounds more fun and I'm going to learn more. So I think that was part of the motivation for for why like I wanted to do that. And I think even so yeah after quals or during quals and we started seeing this work and like writing POVs from like almost nothing like just that get a description from it LLM and then feed it to another LLM and then it writes a PoV and it's like that's a pretty is really cool and it's really cool to watch and it's really cool that it works. And I think that there's also like so much untapped stuff here. Like we could keep working on this for another year or two and like even with the models just staying as they are and our system would keep getting better if if we could keep doing that. So I think there's just there's a lot I'm I'm definitely a believer that that there's a lot here.

**Adam:** Nice. Tim, what about you?

**Tim:** Yeah. Completely agree. I I think I may have been slightly less skeptical of of AI agents, but I was still very impressed at how well it worked in the semi-finals. I wasn't expecting it to work as well as it did. And I I mean, I think that there's a lot of hype around AI agents at the moment, but even like last summer when we were working on the semi-finals, it was working surprisingly well that long ago. And it's only gotten better in the last year. And I think we've learned how to scope the tasks for agents appropriately, how to like develop a good tool set for that task, and it has made a lot of very non-trivial tasks automatable with these AI agents. So, I'm yeah, I'm also very convinced that there's a lot of untapped potential here and there's probably tons of applications of of well-written AI agents that we haven't even found yet.

**Adam:** Nice. So, did you Okay. This is kind of a a question I don't think I've asked anyone else, but how much of the CRS is AI written?

**Tyler:** Very little. I think the main thing that we did for the main place where we have AI generated code is some of our Rust where it was like I have Python, my Python's slow. Oh god, we just need we just need to run this faster. It'll just translate that to Rust. So that's a little bit easier to do because it's like you already know exact like it transliterate. It's pretty nice, but I don't think any of us were really using like the coding agents for our development cycle.

**Tim:** Yeah, I I did a little bit at the end. not so much like coding agents, but just kind of using Claude or chat GPT like o3 on the web interface getting it to write some code given like an interface description I gave it just as a way to sort of speed up development in the last month there where I was like I want to implement all these things and I need to freeze the code by you know a week from now.

**Tyler:** Is that why you added all those bugs to

**Tim:** Yeah, that's exactly it.

**Adam:** No, I didn't add those bugs is what you should say exactly.

**Yan:** You're blameless.

**Tyler:** But I I do like we're we're obviously like bullish and we believe in LLM stuff, but I think that there's a lot to be said for like we have a pretty small team overall and like you know of those eight people like not all of us are kind of core members like some are more part-time and I think there's something to be said for like having a small number of people with not a huge amount of code that completely well completely understand all the code that is written makes things a lot better because every time something comes up and something's weird or you don't even know if something's weird but you need to figure out if it's weird or expected if like an LLM wrote that and you're like I don't even know what this is supposed to do or like it's really scary and it'd be really hard and I think for us it was really nice because it's like oh yeah I got to go in this file I know exactly what's going on because I saw this like thing was slow or like this thing did a bad thing and like so I I think it's obviously a double-edged sword.

## Strategy and Patching

**Adam:** Yeah, for sure.

**Yan:** On on a different part of the kind of problem that AIxCC proposed. You do do a lot of development. All your teammates have to understand all this stuff. That's on the coding side. What about the strategy side? Like when to submit, what to submit, how long to wait, how long, you know, how much modeling did you do there?

**Tyler:** Not not a lot. Not very much. Yeah. I mean, I think so like CGC I think was a little bit more complicated because it's more like the CTF as attack defense. Every time you patch you have some sort of like a penalty of downtime. I don't remember exactly how it was set up but like we had a really complicated thing there with like Bayesian classifiers trying to decide like what's going on in the state of the game who was whatever complicated. This one it's like if we get bugs we should submit the bugs. I mean, I think again, as I said, a lot of this is maybe simplified because we have we believe that we have a relatively solid ground truth for like we have a bunch of bugs and we're not we don't have a bunch of duplicates. Yeah. So, anytime we get a new bug, we submit it. If we get a new patch for a known bug, we submit it. If we get a patch and we don't have a bug, then we wait like 30 or 45 minutes before considering submitting it. And then we only submit it if it's if we've not crossed that 2x threshold. Or if it's a diff mode challenge, then we assume that for diff mode our whatever that it's more likely that if it found a bug, it's probably a true positive and so it should just submit it anyway. There's but there's we don't do a lot of like okay I'm going to I don't know this is Java and Java has this sort of base rate of false like there's nothing like that. 

**Yan:** So it's a also a fairly straightforward submission logic.Yeah I think so that people can understand it. Maybe that that's also a helpful thing. Yeah. Yeah. 

**Tim:** I I think basically the only non-trivial thing is that what do we do about patches where we don't have a POV for and that was basically like a I don't know like in the last two weeks we were like we need to do something for this and that was really the only like game logic specific thing to our CRS most of it I think is somewhat generally applicable and 

**Yan:** actually I have a question on this you talked a lot about the bug bug finding and POV part and we kind of skimmed over patching. How complex is your patching agent? Like does it do how does it make sure that functionality is not compromised? All this fun stuff.

**Tyler:** I mean so part of like I don't know I mean we didn't really make a lot of tweaks to it since the qualifier which is maybe not a good move. So our our patcher like Yeah. So I I guess one of the weird things that we had during the qualification which we just kind of solved and then never looked at again was like we want to make small patches so we don't want to rewrite the whole file. We just want diffs and the LLMs are really bad at diffs. So what we ended up doing there is we have like this somewhat obnoxious like dynamic programming thing like the the normal like sequence alignment dynamic programming approach. So it like figure out like if you give me a diff or something that kind of looks like a diff, I'm going to ignore the line numbers because you're an LLM and you don't understand numbers. I will figure out where it should go. And then as we're doing this, we'll also do some sanity checks like, yeah, you like just pretended that there was not a curly brace there. And there is a curly.

**Yan:** Oh my god. I'm I'm going to go after this now and sit in a dark room. This is like you've triggered some trauma. LLMs and the fucking curly braces.

**Tyler:** Yeah. Yeah. So it was a is a I mean it's a big problem. So we we have our thing where it's like you you tried adding a you tried submitting like a diff to like apply and you asked us to do this but you implicitly deleted a brace or added a brace. We will just say no you implicitly added or deleted a brace here and so I'm you have to fix it before I will accept this patch.

**Yan:** You know, here's what I don't understand, right? Like, and I'm sure there's some fancy fine-tuning and all of this shit thing. But Codeex, it it does this pretty well. If you did like OpenAI Codex on your on your machine, it does this well. You do the same exact thing to the same model, it can't diff. It can't It doesn't know curly braces. It can't understand if statements with a condition on multiple lines. It Let's put print fs right here.

**Tim:** Yeah. Yeah. I think part of that is that the codex tool for diffs is also is somewhat similar to what we we wrote actually and it very fuzzily applies patches and I believe they fine-tuned their models specifically for that diff tool that they have like a generic capability.

**Tyler:** I know they said for 4.1 they did a lot of work to make diffs better. We don't even use 4. We probably maybe we should whatever 

**Yan:** it's so expensive. Is this still expensive? Maybe I'm outdated. 

**Tyler:** I don't know. We were using We were using three. We still use 3.5. Oh, no. No. Sorry. No, no, we were using We're using o4 mini. Oh, it's weird. I'm just looking at our Yeah, we use o4 mini for that. I don't know why, but we do. Oh, sorry. That's the diff. Oh, god. I'm sorry. No, we use Okay, we use two models. We do use 4.1 and we use Sonnet 4. Okay. Our names for these models are kind of not great. (Yan: Both kind of expensive). Yeah, they're kind of but again we don't get a lot of false positives to this point and we don't get a lot of duplicates so we get to spend a little bit more. Yeah, but I I think that the Yeah. So the main thing is we along with our agency you we have these tools they have the tool to like great you've made three diffs that you applied now you need to test it and then we have a bunch of obviously guard rails or baby proofing trying to make baby proofing happen. (Adam: He is making trying to make that happen. Thank you for noticing). And so, we have a bunch of stuff where it's like, okay, you said that you're done and you never tried to compile it and run the tests. So we're going to do that for you and like whatever, you passed or succeeded or something. But we have a bunch of there's a bunch of guard rails and baby proofing. I mean on all of these for things like like some of it's that some of this also like one of the ones that I think is funny for our POV producer if it writes three POVs and tests them and they don't work then we just inject a new message and we're like hey you know you're you're having a hard time here like I get it you know this is a hard task and maybe you should stop and like think think a little bit about your approach like maybe think about three hypotheses for why your POVs keep failing instead of just doing the same thing again and again.

**Yan:** Interrupting those.

**Tyler:** Yeah. Yeah. One time. Yeah. Go ahead. I don't know. I was just going to say these interrupt like we have a lot of these interruptions and it's not like they make a huge difference, but we've totally seen it like stuck down a bad path and get a unstuck enough to succeed some of the time. Not all.

**Yan:** One time I prompted o3 Pro with some something and I'm I'm watching it like the the thought process that you can look at and it's like I'm it's it was a technical thing. I'm thinking about you know the effect of this the effect I'm thinking about this line of code and the next thing I'm thinking about the health benefits of a walk in the park for real. I'm like what the fuck And then it just keeps going thinking about like what just happened. It was it was amazing. The code sometimes. Yeah, maybe that's I don't I think it it came up with something reasonable because that was in my like holy shit o3 that that the phase of o3 is incredible. I wonder how much of our AIxCC token spend is random thoughts like that. Healthy healthy walks in the park while you're trying to patch. Am I a human?

## Local Models and Funny AI Moments

**Adam:** speaking of Wait, I have a better question. whatever you said question because it's quick. I think it's quick. did you guys experiment at all with local models and doing some fine-tuning and did you end up with any of those in your CRS?

**Tim:** we so basically what we tried to do is use a lot of the open weight models just kind of off the shelf and see how they performed on different tasks. We were pretty disappointed with all of them. So we didn't really go down any fine-tuning paths or anything to try to improve that. We instead decided to focus our efforts elsewhere and not go down that whole rabbit hole.

**Yan:** Makes sense. It it would be interesting looking back now because going through especially evaluating on a large data set which we should another thing that would be I mean if you had infinite time looking at a large data set and it's it's it's a great amount of feedback that you can then shunt back into fine-tuning

**Adam:** yeah after the competition is kind of

**Tyler:** I know some of like during our testing it's like our testing was very expensive because we use a bunch of models We have like another kind of like model config file where we drop in which swaps all the models to like our cheap models and like even running like instead of using like 03 it's like use haiku and that's a big downgrade in some sense but our our system like the we still get bugs all the way through and produce POVs from them obviously far fewer and there's more false positives.

**Yan:** Do you have an idea like percentage wise?

**Tyler:** I don't know because those those tests were normally like we just want to make sure it's like not falling over tests. So we didn't kind of run the full thing. I mean far less than probably less than 20% of the stuff maybe less than 10. But I know one of our other folks like in the last couple weeks has been running on I think like Qwen the newest Qwen or something and he said it's doing decently but I haven't really tested that out.

**Adam:** That's cool. So yeah, that'll be super interesting, especially when all these things are open source and like people start experimenting with local models and that kind of stuff.

**Yan:** On the topic of baby proofing, what's the most hilarious like situation that an LLM induced in your code like non-baby proofed situation?

**Tim:** I the the Jenkins one you mentioned is is pretty up there for me where we asked it to trigger this vulnerability. We told it about the fuzzing harness and it still, you know, busted out requests and tried to send an HTTP request to some madeup local host address. That's up there. I don't I don't know if you have any better ones, Tyler.

**Tyler:** I don't know. I mean, I think like, you know, we do a lot of restricting on what like again, they don't have tools for like bash, so like we've never had it try to do something too weird. We've totally had it try to do some patches where it's like I I don't remember if any of them were trying to patch out like the Jazzer sanitizer like things itself, but we we've had things where like it's like you're totally that that's not okay. Like you're trying to patch things that you are not allowed to touch. Definitely had some of that. But

**Tim:** we had to ban the harness files from the list of files it's allowed to touch because sometimes it would want to try to touch the harness files and block the bug at the source. 

**Tyler:** To be fair, sometimes there are bugs in the harness files a lot of times and it finds them and it's like what do you mean I can't fix it in the harness file? That's where the bug is like what do you want me to do? And that's 

**Yan:** some of our auto batching research like in the lab academically AIxCCS aside runs into this problem like OSS-fuzz harnesses have bugs.

**Tyler:** Yeah. Yeah. Well, I mean they gave us like that SQLite one had like that annoying thing where like it was just not a good harness, right? They wrote something and gave it to us and they probably never fuzzed it because as soon as you fuzz it, it it's a million crashes and it's just like oh those aren't real. Those don't count. You can't score those. and it's like great. not sure what I'm supposed to do with that, but yeah.

## Predictions and Retrospective

**Adam:** All right, we're getting close to time. We don't want to go too too far over. So, we've been asking all the teams this. So, what place do you think your CRS is going to get in finals?

**Tyler and Tim:** (both shrug simultaneously)

**Tim:** I'm really hoping for top three. I think like I'm pretty proud of what we built. I think the capabilities are impressive, but it's so hard to know if another team has some secret sauce that just completely blows us out of the water. I like it was such an open-ended problem. There were so many ideas to explore, and I don't think we got to all of our ideas. And I'm sure teams have ideas that we never even thought of. So, it's so hard to predict. And of course, we worry about the same thing everyone worries about where maybe we just fell over on day one and we get last place. You know, it's so hard to know.

**Tyler:** Yeah. I mean, I think it's one of like like Yan said, you know, if we if we run and we don't fall over and we don't do very well, that's sad, but that's like that's it's a game and that's what happens. I think if we don't fall over, we're going to do well because I, you know, I think like in our testing, we're finding a lot of bugs. We're submitting a lot of patches. Seems nice. I think we can, I think top three is plausible for us. I mean there's there's seven teams like top three is a little bit better than 50%. I hope we can do that but it's also possible we completely fall over. I don't know. There's a lot of there's a lot of unknowns

**Tim:** And it also depends on the shapes of the problems because if a lot of the bugs are very fuzzable, I think that you know the the more fuzzing based approaches and like what what Shellphish did with the the grammar generation might really pay off and it might be that the LLM approach is just too slow or just not as scalable as fuzzing.

**Adam:** Yeah, for sure. But then on the other hand, there's like on use-after-free-s, it finds like 18 to 20 of those POVs for a use after free, which then and each of them can generate independent patches that just fix the symptoms but not the root cause. And so there's a whole bunch of other stuff that we've had to deal with to do something like that.

**Yan:** There's there's a lot of I I'm I'm really interested in seeing the the those trade-offs between LLM first and and program analysis first. And what's really interesting to me is a lot of the designs they meet in the middle. So a lot of these ideas of you know having the LLM look at the code and try to flip branches or you know these a lot of these ideas come in to both designs eventually.

**Adam:** And actually, I mean, the more we're talking about this, Yan, the more I could see, especially like I mean, we didn't get into the exact, you know, data sharing, but it sounds like these components and these agents are kind of loosely coupled, right? you could just kind of give them a task and give them their their things which means like I don't know a year from now or three months from now when this stuff is released like people could start like our agents are also pretty independent and so you could think about like our super expensive grammar guy in there with some other things with the AIJON thing that Yan was creating. yeah, it could be super interesting. (Yan: I was helping) you you helped birth it like was it was in a bad state. It was not going to make it. 

**Yan:** I helped with but it was you know it was not my component. Yeah. Yeah. Sure. That's true. And I'm I'm saying that because as Tyler is talking about maybe we blew all the all the context. I'm thinking of all the ways that just that fucking component can go through all of our not context all of our budget. Of course. Did we have time to test that? Testing, testing, testing. 

**Adam:** Then you did not for that at that point because we were very close to the end.

## Lessons Learned and Retrospective

**Adam:** But all right. So then looking back over two years, kind of a bit of a retrospective. Is there anything you'd do differently like lessons learned? I don't know, different ways you'd approach this.

**Tyler:** I think I think it's hard partially because you know the it's a very ambitious contest which was run kind of intentionally at to stay at the bleeding edge of things right like this was announced like before GPT-4o was announced like a few month like less than a year after chat GPT was released and things keep moving and there's just a lot of unknowns during the whole thing and so obviously Like if I could look back, I would tell myself like great, here's the final budget that they were going to give us and this is the number of challenges and like you can write a CRS to fit in this exact box and here's the final rules that we didn't get until like a month ago and you know there's a lot of stuff that like great if I knew that from the beginning we would have made slightly different choices but I think you know knowing given the information that we were given at the time you know I don't think we did any huge blunders aside from starting earlier would have been nicer and having more t like some of like it was basically just me and Tim until around December or January of this year. So having more people earlier would have been helpful too but you know if it falls over then fixing that would have is my biggest 

**Adam:** well okay yes that you can't you can't know that yet I can't you can't know what to do differently without you know pre- knowing the results right it's about the process I guess or 

**Yan:** what are you going to do with the money there's expected value 

**Adam:** Wait wait wait wait Tim Tim has Tim okay go for it.

**Tim:** yeah the biggest thing for me is starting earlier because basically we we were very time crunched for our semi-final submission. We quickly threw something together and it wasn't much of an investment because a lot of the code was not going to work in our ideas for final. So we had to basically rewrite it from scratch and all of that time spent rewriting it could have been spent exploring other you know interesting features or ideas. So starting a little earlier and having a more solid infrastructure that we could continue to build on would have definitely been a good investment.

**Adam:** And is this like looking back would you have gone after the small business prize or maybe you did go submit to that?

**Tyler:** No, we we didn't submit for it. I mean, I think our our, you know, they they softened some of the rules around it, which was reasonable, but our biggest concern at the time was like, I don't really I'd feel really bad if we submitted for this. And then we're like, actually, now that you've told us what the competition is really going to be, I don't want any part of this or I have no ideas. And we were kind of worried about that and we're just like, it's not worth it. No, that's in retrospect, we should have we should Yeah. 

**Adam:** Well, since you knew you were going to do, you ended up doing it anyways, you know, do it plus get money for it. But, no, that totally, but then of, you know, you also would have spent more time on it. And I don't 

**Tyler:** I mean, it's also possible that our our wait until the last minute until we have a better understanding of the shape of the problem. That could have helped, right? Like if we started too early, we might have taken different approaches that would have been bad.

**Adam:** Yeah. or maybe tried out the models at the time like that you tried the agentic stuff maybe wasn't quite where you wanted it to be if you had started too too early. yeah, it's super interesting. I don't know. I don't know. I don't have the model timelines in my head so I can't like speak to that.

## Future Plans

**Adam:** Cool. Any other questions Yan for our great guests? 

**Yan:** What are you going to do with the money? Yeah, there we go. That's expected value. You're winning over a million dollars if you randomly throw a dart at the top seven places. 

**Tyler:** That's true. slightly more than yeah 7.5 million or something for seven places. I don't know I mean so part of this is like you know we're a company and we have been very fortunate to have been allowed to go off in our own little AIxCC world. So you know gets back into Theori we can do some (Yan: increase shareholder value) increase shareholder value. we already we Theori recently bought one of those like a DGX machines like those huge whatever I don't know how many like a terabyte of GPU memory and stuff. So we already do some stuff for our other non-AIxCC AI security stuff. So there's definitely I mean you can spend the money easily.

**Adam:** Nice. And do you see like a future where this is rolled into some stuff that Theori then ends up doing and commercializing?

**Tyler:** Yeah, we're definitely we are that's part of what we're working on now. So we're trying to see like trying to run a few more tests trying to see like I mean the nice thing is that the LLM approach is very agnostic to what you're doing. And so like you want to run Python like yeah that's fine. Like you can just have it look at Python code instead of C code. It doesn't really care. So add support for that. Look at a few more projects. Try to also just try to understand what this should look like as a as a product or commercial thing. So yeah, great.

**Adam:** That's awesome. Yeah, I think that's, you know, it's very exciting that and I can definitely see that being inside of an existing company, there's already kind of the mechanisms to then go out and use it and customers and maybe there's already problem areas that you can throw at it. So yeah, I think it's great that like the stuff lives on beyond this competition and continues to evolve while also having that kind of open source snapshot that we'll have of all the submissions so that everyone will get to learn from it and then they'll probably go off from there.

**Tim:** Yeah, very excited about that part. I I want to read through all the submissions and see what other people did and integrate some of the ideas if we can.

**Tyler:** It didn't come up much in this one, but I really like like when I talked to people too, it's the same thing that Yan was saying in some of the other interviews where it's like CGC everyone everyone basically did the exact same thing. Everyone's thing looked almost identical and in this competition like we every time we talk I'm like I have no idea what another team is going to do. Like they could do exactly what we do. They could do a completely different thing from we do. They could do like I have no idea. It's there's it's so much more open-ended and there's so many more possibilities I think and so much greener fields of research.

**Adam:** Yeah, that's cool. Exciting stuff. Yeah. All right. Well, I think we are at the end. So, thank you so much Tyler and Tim for joining us today and Theori. We wish you guys the best of luck come August. for everyone else, come out to Defcon and see them announce the winners. I believe it's like Friday morningish, which is completely destroying our our CTF time. I think it's like 10 or 11, is Is it 9? 11. All right. 11. But I But in hacker par 11 a.m. is 9:00 a.m. basically. So I know what you mean. so yeah. thank you everyone. we are CTF radio. I don't have the outro stuff here. So I'm just going to say keep watching because we're recording a lot of these this month and it should be great. All right. Thanks everyone. Bye. Tim, Tyler, Thank you for joining us. Thank you. Thanks for having us.
