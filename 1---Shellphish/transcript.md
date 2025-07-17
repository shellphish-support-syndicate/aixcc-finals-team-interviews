# AI Cyber Challenge Interview - Team Shellphish

## Introduction

**Adam:** Hello everyone. Welcome to CTF radio. We are now on what we're just going to call season 3. Apparently that'll be every year where we end up releasing episodes, we will increment the season number.

**Yan:** It's season four.

**Adam:** Man, you're not even going to let me introduce you before I... Yeah. Hi. So, I'm adamd and then I'm super happy to have with me the great Zardus.

**Yan:** Hello, hackers.

**Adam:** All right. There we go. So, you know us. We're here on CTF radio and what we wanted to talk about now. So we're sitting here about a month until Defcon and Yan said to me, "Adam, Team Shellphish has probably been playing CTFs, but we wouldn't know because we haven't really been playing CTFs with them. But the one thing we do know that Team Shellphish is doing is participating in the AI cyber challenge." So he said, "Let's talk to the teams doing the AI cyber challenge." And I said, "That's great, Yan, because as you may remember, we did an episode about that. That was season two, basically preparing for that." And then actually from Defcon, our AIxCC. So, we're going to kick off the first of hopefully all of the seven teams that are playing in finals. We don't know. We have to reach out to people. We haven't even done that yet at the time of recording, but

**Yan:** we got people on it. We got our best people.

**Adam:** You're just looking at me. It's going to be me. That's who's going to... we got our best person on the job who's definitely going to drop the ball. But anyways, I will definitely try my best to do that. And if you're listening to this and we haven't reached out to you, you feel free to reach out to us. We would love to talk with you. So, we're starting it off at home. Yan, why don't you introduce our two guests?

**Yan:** Two guests today need no introduction, but we'll give them one anyways. I'm going to kind of do my typical rewind back to the start of the universe, right? There was the big bang, etc.

**Adam:** I can't rewind that far. I was trying to do a rewind sound effect, but I can't do it long enough to go back to the big bang.

**Yan:** Exactly. Eventually, humanity evolved to create capture the flag competitions, which of course, as we know from this podcast, are the pinnacle of human achievement. And eventually the CTF community evolved to create the pinnacle of badass CTF players, which is Shellphish. And eventually Shellphish evolved to have multiple generations of hackers. And this is something that isn't unheard of in CTF, of course, you have multiple generations of a team,


**Adam:** but the way you're saying this makes it sounds like Shellphish itself begets other Shellphish members somehow.

**Yan:** Yeah, that's kind of... that is a little weird, but you know, academically, let's say it's true.

**Adam:** Ah, okay, perfect.

**Yan:** Yeah. So, there's these multiple generations of mentorship in Shellphish and if you go back to season one, I don't remember which episode, but we did an episode with several generations of Shellphish discussing this cool phenomenon. There's a number of CTF teams that are multigenerational, not as multigenerational as Shellphish, just due to raw passage of time. And I was in like generation three of Shellphish when I was the Shellphish captain for a while, etc. And then I passed the baton to generation 4, which passed the baton to generation 5, which is crazy enough to when the AIxCC, the AI cyber challenge was announced, they said, "Yeah, why not? Let's put our entire lives on hold and do this for a couple years and see if we can change the world." So today we have two incredible Shellphish who are the captains of Shellphish's AIxCC effort. And we got Clasm and Honululu aka Wil and Lukas. Guys, why don't you emerge? Boom.

**Lukas:** Guys, I think they're after me.

**Wil:** I've been here the whole time.

**Adam:** Wait, I think I have a clapping sound effect. Wait, how do I do this? Boom.

**Lukas:** What's going on? Where is everyone?

**Adam:** Wow. Okay. So, yeah, two years trapped in a room creating a cyber reasoning system does something to a person. That's what you could tell from Lukas.So, this is great. So, okay. So, now we have the two Shellphish AIxCC captains. Is that appropriate titles for you two?

**Wil:** Yeah, let's go with that.

**Adam:** All right. Great. So, then all right, Lukas, kick us off. Start us. I know we talked about AIxCC probably a year ago on this podcast. Can you tell?

**Yan:** Do you remember if we were sober on that one? Because I don't remember what we talked about, but it was...

**Lukas:** we just came from the dinner, I think. No, we went to dinner.

**Wil:** Yeah, we were going to the dinner.

**Lukas:** We were going to the dinner. I think sober.

**Adam:** We were in Las Vegas. I think the answer was no.

**Yan:** We had just found out to be qualified.

**Adam:** No, that was a pre... We did the pre interview. Following the... I added the thing at the end just screaming like crazy people. Exactly. I did way more editing than I will ever do in any other podcast, but it was fun.

**Adam:** Okay. So, Lukas, remind us what is the AI cyber challenge?

## What is the AI Cyber Challenge? [5:24](https://youtu.be/ozp7fBoOsIQ?t=324)

**Lukas:** Sure. Yeah. I mean, so the AI cyber challenge was I think like August 2023 announced and the idea was kind of in a way very simple but also incredibly complicated. The idea was at the time we had just started the hype cycle of AI and GPT and all of these LLM things and the question kind of arose, the natural question is how can we use all of this for security? Because I mean over the years we've seen various applications of machine learning and AI in security but I think we can all agree that there was never really this moment where anyone actually believed that that would work and all of the approaches that people had done were of questionable usability.

**Adam:** Yeah. Maybe people at home, you know, I think like, well, I don't know, Gmail's pretty freaking good at getting spam email out of my... and since you're in the whatever this fifth generation that Yan talked about, I remember the days of having a Hotmail account and having no spam filter and having all types of messages go through. So, you know, I think like so maybe like what area of cyber security were you not seeing the ML and AI applications of?

**Lukas:** Yeah, I mean I think we both me and Wil kind of come from the background of binary and program analysis in general. Aka trying to automatically find security vulnerabilities in programs. So trying to find these bugs that can take down entire machines or that can allow you to take over that machine and these like really security critical bugs. And that entire field has kind of traditionally been dominated by tools like fuzzing where you just repeatedly mutate and throw new inputs at the program until it eventually breaks. Where you're kind of like brute force breaking the software by just trying so many different combinations that it never expected that eventually you find something that breaks and then that's great. That's what you were looking for. And we had these tools and techniques before that were trying to find these things. And people had tried to use this machine learning approach of trying to mine data from existing software, trying to mine data from existing vulnerabilities, but I don't think anyone's seen any like super convincing arguments of like, hey, there's something here with this machine learning stuff that can really work.

**Adam:** And especially at the time, I mean, I've seen papers like research papers that came out. I reviewed research papers at the time and it was always like okay you're using like machine learning in some sense but like the features that you're using are they actually capturing what is the nature of that type of vulnerability like are you just finding minor code clone differences that really aren't going to generalize to when you throw it against something like Windows or Linux?

**Wil:** Yeah. I think I was just going to say I think that prior to AIxCC and really the introduction of LLMs into the greater society, a lot of the papers or research we were seeing being done were these AI or models that were trying to look for specific features or maybe classification of here's a function, is this function vulnerable and it would spit you out just a yes or no answer. And these things were rife with like data set problems, inaccuracies or what you were saying Adam is they were just identifying these things that they've seen before the code.

**Lukas:** Yeah. And I think a lot of the times even when there were advantages it seemed like they were mostly marginal and not really anything life-changing. And so just kind of to go back to the challenge, right, with these LLMs where I think most of the research community, us specifically too, right, was like, hey, this actually seems like there's something here that might be useful. These models have seen so much data, they've seen so much software that it's almost impossible for them to not have learned anything interesting that we might be able to mine. And clearly the folks at DARPA felt the same. And that's kind of where the AI cyber challenge started. The idea was really, let's use these LLMs, let's fund people, let's fund teams to use these LLMs to the extent that they can, right? Like, let's make sure we really mine out the possibilities that we can do and build the best system to find these kind of like critical bugs with the help of these LLMs.

**Adam:** Awesome. And then this is also in the context of, Yan, can you describe just very briefly like the previous cyber grand challenge? Like I want to make sure people understand the context here of what came before and what DARPA was and is trying to achieve with the AI cyber challenge.

## Context: The Cyber Grand Challenge

**Yan:** Yeah, this is a great piece of context.

**Adam:** You're welcome. This is my job as host.

**Yan:** There you go. DARPA is no stranger to these sort of exploratory contests, right? 10 years ago and that wasn't even the first contest DARPA ran. In fact you know if you go back to even earlier contests in this kind of related in the tech space and DARPA ran these self-driving car contests which have you know a decade and a half later resulted in you know Waymos driving in the streets and people not needing to be driven or to drive their cars. 10 years ago roughly DARPA created the cyber grand challenge. The idea being that there are all these techniques, algorithmic techniques at the time that were being created to find vulnerabilities, reason about their exploitability and a little bit to fix these vulnerabilities automatically. And DARPA wanted to both understand the actual state of these techniques, their actual usability because that can be hard to understand when reading academic papers on the topic and also to catalyze more development. They created to do this the DARPA Cyber Grand Challenge, the CGC. And the CGC had this goal of basically pushing forward the creation of cyber reasoning systems, autonomous computing platforms that could analyze code, find vulnerabilities, fix them without any human involvement just to see what is possible. Then of course after the CGC all of these techniques that were developed for the CGC were augmented, continued to be developed, productized, got humans put back in the loop because in the real world you can of course have some human effort. It's all good. And you know really advanced the state of cyber security and really set the stage for then a decade later the AI cyber challenge.

**Adam:** Excellent. All right. Thanks Yan.

## Prize Money and Competition Structure

**Adam:** And then so Wil talk to us about the one thing that everyone cares about. Cash money.

**Wil:** That's there was a lot of money online for the for AIxCC. I think it was 27 and a half million in total.

**Adam:** Got to get that half.

**Wil:** Got to get the half. I mean, I'm not missing out on $500,000. I don't know about you. I'll take it if you're leaving it on the table.

**Wil:** All right, great. So, yeah. Go ahead. Yeah, but so in the leadup to the competition, everybody, all the teams that were competing were after the $2 million semifinals prize, which is if you make it into the top seven teams, you win $2 million. It's as simple as that. One of the things that we actually managed to also win on top of this was the small business prize. We wrote a very nice proposal and the top seven best proposals also won an additional million dollars in the leadup which certainly helped fund our activities trying to get into the top seven teams.

**Adam:** Are you saying that this effort needed a lot of money? He says hinting at where we'll go later.

**Wil:** It's an expensive process. LLMs, not the cheapest things. Unfortunately, they don't run on dust and air. They use the liquid gold.

**Adam:** All right. So, what's up for August? So, what for this finals? So, we're in the AIxCC finals that are happening in August. What are what's the prize pool that teams are competing for? There's seven teams left.

**Wil:** Seven teams left. Top three take home some nice prizes with third place at 1.5. That's where your half million comes from. Second place at 3 million and then first place gets four million bucks.

**Adam:** Woo. Pretty nice.

**Yan:** In the Cyber Grand Challenge, 10 years ago

**Adam:** wait, you have to start your sentence by saying, "Back in my day."

**Yan:** Back in my day, for those that don't know, Shellphish also participated in the Cyber Grand Challenge. We got third place there, the prize was 750,000. So, that prize is doubled for third place. Why do you think the prizes are like doubled?

**Adam:** Great question.

**Wil:** So, I mean, honestly, I AIxCC seems to have a much more immediate real impact, I think, than CGC. No, not CGC's. Yeah, shots fired. But to be honest, the CGC programs were, you know, custom written, seven syscalls per program. Not to say that it wasn't like incredibly novel. I mean, for God's sakes, angr was born out of the thing, right? It was an incredibly difficult challenge at the time without LLMs, but now that we have all of what's happened in program analysis from 2015 to now, plus this introduction of LLMs that help lift the human aspect out of it, we're working on software that's used in production by millions, if not hundreds of millions of people and companies every day.

**Adam:** Yeah. So, the previous competition was crap and the new one is good.


**Wil:** I'm glad, yes exactly.

**Adam:** You missed the real answer, Wil.

**Lukas:** Inflation.

**Adam:** Inflation, dog. Yes, exactly, Lukas. Yeah, inflation. 750K doesn't get you crap anymore, man. You got to get those millies.

**Yan:** I think it's possible that there's 750K for AI and 750K for security.

**Adam:** Bridging The two. I love it. I love it.

**Yan:** But kind of pulling this thread a bit, right? So the cyber challenge you mentioned the whole way that it was run the challenge problems that these autonomous cyber reading systems had to analyze. They were custom built and very simple in their interaction with the operating system with their environment. Why do you think that is? Now, as you mentioned, AIxCC is a different beast. The challenge challenges that you have to analyze and find that your CRS has to analyze and find bugs and they're full real programs on the size of, you know, web servers and stuff. How was that shift possible? Why did the CGC start small and why did AIxCC go large?

## Technical Evolution: CGC vs AIxCC

**Lukas:** I mean, I think there's two parts to it. I think the first part that you'll kind of have to think about too is if you think about the space of the things being analyzed in program analysis at the time it's not super surprising because I mean most of the modern techniques that we use today right like most of the fuzzers were barely in their infancy at the time I mean I think like yes some people had been fuzzing since 2007 but really the fuzzing that everyone was doing with just simplest AFL with no none of the modern techniques applied to it started in was released in 2013 and which is when the cyber grand challenge started there wasn't much time for adoption and implementation and so 2015 the cyber grand challenge was already over so at the time that was the newest thing it had just come out and people hadn't figured out to how to apply it to all of these other software pieces of software at the time that communicate over the network or use encrypted communication or talk to file systems or whatever. Like at the time it was all just here's some data, do something with it, give me something back. And I think if you view it through that lens, it makes perfect sense that the competition kind of reflected that because that was what people thought these techniques were built to do. And like that that was the extent of what people thought was reasonable. It took years of research after that to figure out how to apply them to everything else. Right? Today, people are fuzzing drones in swarm algorithms of like how do they interact with there's like there's so much more that people do, but at the time that really wasn't there.

**Wil:** I think there's also a big piece here that's missing, which is that the CGC was entirely binaries. They didn't have the source code that we have for AIxCC, right? The...

**Adam:** So your competition is easier.

**Wil:** Yeah. Yeah. Yeah. Sure. I you can tell yourself that. That's great. But no, I think that that this also significantly scopes the problem. It's very very difficult to run to run tools on binaries just as they are. And then to try and do this blindly for any generic binary, you have to scope the problem somehow I think.

**Lukas:** yeah, I mean I think another part that comes into it that comes from the binary part, but that also kind of influenced part of the decision is one thing that I really liked about the AIxCC is in the AIxCC the problem is very straightforward, right? You try to find bugs and then you try to patch the bugs in the source code. Those are like the two main thrusts of what you're trying to do in AIxCC. In the cyber grand challenge, it was orchestrated a lot more like a CTF. You had to not only find the bug, you also had to exploit it and figure out how to abuse parts of the program's functionality to get you what else you wanted on top of then trying to find ways of automatically mitigating it in without being able to recompile the software, without being able to just, you know, fix the code, right? That wasn't at the time that wasn't even anything anyone considered reasonably feasible, but it also wasn't part of the goal. And so there was this entire other aspect of automatic exploit generation, automatic mitigation without having access to the source code. And so I think there was a lot of focus on parts of the competition that weren't just the program analysis part of bug finding itself.

**Adam:** Yeah. Which makes sense. And I think at least the vision of the AI cyber challenge of like, hey, we want to build systems that can help average developers and companies fix their bugs in their software, right? I think that was a big innovation.

**Yan:** And your typical developer doesn't care that someone could use this bug to do X, Y, and Z in an exploit. They just they care that there's a bug that could be used potentially and that could do something. Let's let's fix it and they want to fix it.

**Adam:** And they want it fixed. Exactly. That's what I was going to say. Yeah. 100%.

**Lukas:** I mean, or the famous Linus quote of security bug is just a bug, right? Like they don't even care that it is a security bug. They just care that it's a bug.

**Adam:** Yeah. Great. Okay. So, now that we've set the stage for the competition, now I want to focus more on Team Shellphish and what your guys's approach has been to the AI cyber challenge. So, this has been a to recap 2-year endeavor with the first year focused on qualifying, one of the top seven teams, and the second year really going whole hog 100% towards finals. So, let's start with the team. So, can you let's say Lukas, we'll start with you. Tell us about the Team Shellphish playing like in and and competing in and maybe describe your shirt. I think let's maybe we'll start there. I should have started with the teamname maybe.

## Team Shellphish's Approach

**Lukas:** Yeah. So I mean as the shirts say we have decided to term the system that we built our cyber reasoning system ARTIPHISHELL with the obvious part being left out that we're intelligent so therefore it must be artificial intelligence. But I think as a team, Shellphish kind of started as I mean it really was a relatively small circle of us where we're just like, should we do this? Should we do this? What what if we did this? What if we spent the entire two years doing it? And then it kind of grew out, right? Shellphish is a pretty big CTF team. Always has been. It's been pretty inclusive. We when people want to join, they we have friends in other clubs that want to join. They play with us. we have different universities all collaborating together. relatively open team. And so when we started, we kind of approached it from the same thing of like, hey, we have three universities that are all interested with interested students that all want to play. Let's just do it together, right? Let's do it as the team Shellphish instead of as the university. And we started out with at the beginning there wasn't that much information available about the game, right? It took until about I think December when we first got the first document of like what are we actually trying to expect because the challenge had just been announced. But we didn't want to be left behind. So we started immediately. So I remember I think in October we had our first hackathon. Or maybe it was beginning of November where we all met up and we were like okay let's imagine what this competition will look like.

**Yan:** real quick. You're talking about November 2023.

**Lukas:** Yes.

**Yan:** Or October 20.

**Lukas:** Yeah. Yes. And we were like, we don't know yet what they're going to do, but we've been running CTFs for years as a team, right? So, we have some idea of the decisions we would make if we were to host it. So, let's just build for the competition that we would run if we were the organizers. And we kind of started we had challenges that we had from CTFs from other DARPA engagements that we'd worked on from other research opportunities right we had challenges that we knew were difficult and we just picked those and we decided okay let's build a system that can solve those and then we just kind of decided to start building from there and I think one thing that we've already mentioned last time, so I'm not going to go super in-depth, but just for anyone that didn't see the last one is became pretty quickly clear after the first document was released was we'd underestimated what we thought they were going to ask us to do. Or maybe they overestimated the difficulty of the thing they gave us. We'll leave that up in the air, right? But the very first thing they gave us was the Linux kernel, and we were very much floored by that because that was not what we had expected, right? That was not anywhere near the scale of software that we built our system for. The challenges we were testing had a couple thousand lines of code. The Linux kernel has millions. The challenges we were testing were in style a lot more similar to the CGC style challenges with relatively limited interaction. The kernel has infinite ways of interacting with in some ways. And so, I remember the second hackathon, everything had changed, right? We started building all of this tooling specifically for the Linux kernel because we're like, okay, well, the Linux kernel is a big piece of software. We know how to deal with it. There's existing tools. So, we started building all of that stuff and then they released Jenkins and now it was a giant Java application with again super large amount of code, but now it's Java. Now it's an entirely different system yet again. And in classic rabbit chasing the hare rabbit chasing the turtle fashion, we're like, "Okay, well, let's build something custom for Jenkins, right?" And so that was kind of I think the end of our trying to build custom things. At that point, we were like, "Okay, clearly clearly this isn't working, right?" Like, clearly they're going to keep throwing new things at us. And the techniques we had tried hadn't generalized to the extent that we wanted to. And so I think then we kind of had this shift of like probably like February-ish February or March where we're like, "Okay, screw this custom building. let's just try to do a baseline of tools that can work. And that's when we started to look at more of these LLMs because they tend to it it doesn't really matter what code you show them, right? It's just a text interface that you feed text to. And so that was the first one where we're like, hey, this is actually kind of cool because this allows us to generalize some components that we couldn't previously.

**Yan:** So, in terms of like a sound bite, would you're saying that for the first three or four months of the AI cyber challenge, Shellphish ignored the AI part?

**Lukas:** Oh, absolutely. To be fair, partially intentionally because we very much did like the kitchen think of like, hey, we know what works, right? We've done research in cyber security and program analysis for a long time. We know the traditional techniques that work. So obviously the first thing we put in was everything that we know works already. So AFL Jazzer, right? Like our traditional fuzzers, syscaller at the time for the Linux kernel. We just put in the things that we know worked already because a me included some of our team members were still pretty skeptical of the capability of these LLMs. But also b because we just didn't think they were necessary. Right.

**Adam:** And rightfully so. At that point in time, we're talking 2023, right?

**Wil:** Yeah. Yeah. I mean, we at the very beginning, we did have like I think maybe two or three LLM components. One of of course being patching that that's just a difficult thing to solve without LLM. But then the other, you know, we had a very rudimentary asking, hey, is this code vulnerable? And we would feed it like entire files. And right when we were thinking on the scale of these thousands of lines of project, we could feed a file or two in, it would cost a couple cents, but then when they gave us the Linux kernel recalculated because it was going to cost something like $10,000 to do the whole thing. And for reference, the semifinals had the restriction of spending $100 per challenge for in terms of LLM credits.

**Adam:** There you go. Yeah. Yeah. Okay. So, you had this big LLM credit, but now, okay, before we get too deep into the because I want to get into like the architecture of the system and how you approached it. Like Wil how many people were on the Shellphish AIxCC team? You don't have to give like exact numbers, but I think people at home want to understand like how many people were working on this, right?

**Wil:** Yeah. I think we had about 12 core people working at at any given time, maybe 16, and then about another 10 that rotated on and off.

**Adam:** You mean 12 to 16 core at any time? Like like you go into the Discord and there's like 16 people hacking away at one time.

**Wil:** Yeah, exactly. No, we were all on a live call the entire time for two straight years. No, we had 12 to 12 to 16 people. It was probably 16 full-time. We were engaged in trying to make ARTIPHISHELL our CRS. Working, you know, 12 16 hour days sometimes just to to make it to the finish line. And then of course as part of a university and larger team, we had 10 or so other people that due to scheduling conflicts or availability, what have you, were able to donate some of their time as well to to help with the effort.

**Adam:** Cool. Perfect. Awesome. Okay. So then, Lukas, back to you talked about components. What does that mean? And

**Wil:** yeah, list list them all right now, Lukas. All forty-something of them.

## System Architecture: Component-Based Design [30:55](https://youtu.be/ozp7fBoOsIQ?t=1855)

**Adam:** This is of course a leading question because I know kind of some of the answers but talk about let's like like when you talk about that and maybe this gets into you had this crazy team of people rotating in and out. So how did you approach the like development of this complex cyber reasoning system?

**Lukas:** Yeah. So I mean when you start out something this right there's kind of generally two styles that people can do which is one is you build one system as a whole that is just trying to do as many of these tasks as well coordinated as possible. Everything is like linked together like maybe they just write into the same directories and everyone's trying to pull out from the same thing. And

**Adam:** Yan lit up. He heard he heard the visions of FSDB and he lit up.

**Wil:** He's seen the horrors.

**Yan:** File system was invented for a reason, guys.

**Adam:** Yes. To store files, not to store a database. Entire fields were created around databases, man. Theory and practice.

**Yan:** No one uses that stuff in real life, man.

**Lukas:** But everyone even in the database setting, right? Like even even in the database setting you would have one centralized thing that has everything that everyone relies on. Everyone like interacts with this and it's like very interlinked way of developing

**Adam:** a hub and spoke model, right? If you think about like for people at home like a bicycle wheel, right? You have the database or central component in the middle and everything else is kind of reliant on that.

**Lukas:** Yeah. Or maybe two databases, right? like maybe maybe you have some but there's some central components that link everything together and there are some central pieces of software that and like some interfaces between them that everyone kind of agrees on and that's one way of building a system it is generally probably something that I would have said we build as well if we had been a smaller team right but especially as a large team that is physically separated in three different universities right? Arizona, California, and Indiana, right? Like there's a vast physical distance and people that rotate in, right? As we were saying, people that come in for 3 months and then leave again. If you try to build this system then everyone that is trying to contribute to the system has to understand every other part of the system and has to be able to interact with every other part of the system to be able to do anything. And so that works if you have a small team. If there's like three people, that might be an architecture you go for. But especially for us with PhD students that all want to kind of work on their own thing. We kind of pretty quickly decided on doing a more decentralized approach where you have components that are more loosely linked, right? Each component just has one job. You take some data, you produce some output, and then that's it. And obviously this is a simpler model for every individual person to work on, but then it requires a lot of orchestration of like getting that data from point A to point B, making sure that if I'm trying to do a patch and I just have the vulnerability finally available, then I need to start the patcher and all of this stuff. And so you have to have an orchestration framework that be is able to do this and on demand schedule tasks on demand feed data from A to B in an data agnostic way because the idea is a new component can arrive tomorrow and the system can still handle it just as well and nothing needs to change in the underlying system. And that method of doing it obviously requires us to build that orchestration framework, but it also requires a lot of that orchestration framework to be very abstract, agnostic and like be able to deal with arbitrary pieces of data. But it has the advantage that we can all work on our own little things without breaking everything else and without having to understand everything else. And so those individual things is what we generally call components that are just like single job take some data do some analysis produce some new data that gets picked up by someone else and that's kind of how our system is orchestrated.

**Adam:** Awesome. All right. So then Wil I've given you enough time. Maybe you know this is coming. How many components did the final ARTIPHISHELL submission have?

**Lukas:** Too many.

**Wil:** We counted I think I counted and it was about 65

**Yan:** 65?? like I was

**Wil:** 65 little scripts sparing some some just were straight data pass-throughs others were very complex like mechanisms for understanding the code but in total if you were to look at the the little blips on the on the graph on the data flow graph every node there was I believe 65.

**Adam:** which is something super interesting that we didn't mention But because you basically had this, you're describing what we called the pipeline of the system with components and how data flowed in and out. You could create this graph and actually watch the system operate in real time. So as nodes had data available for input, they would then get started as jobs and then they would produce output that would start other jobs.

**Yan:** It also creates sorry to talk over you Adam. It also creates this this fascinating effect where as Lukas said you know people like to work on their own component right on the the kind of semi-final of course the the professors showed up for the very end and to to just you know mog around and chill out. But I was working on like one specific component. I had no idea there were 65. This is insane. I remember I I ran a a line counter on the whole repo and I was just blown away with the amount of lines in there.

**Adam:** Wait, how do you remember off hand what that what number was?

**Yan:** 270,000 lines of Python plus other stuff.

**Lukas:** And bash and yaml. Yeah.

**Yan:** A significant amount of bash. Yeah. Templated bash.

**Wil:** Just to just to let the folks at at home know, Lukas and I learned an incredible amount about software management and and foundational like development techniques and applied none of these.

**Adam:** Well because you learned it during while doing it, right? So if you think about like where you were 2 years ago, you guys have I know been involved in open source software. You've developed software, you've released it, but managing a team of let's say even 12 core people with 10 additional ephemeral people is a completely different beast.

**Wil:** Yeah. Especially when everybody has their own wants and needs and and...

**Adam:** are you saying these are people? They have wants and needs?

**Wil:** I mean I try not to think of them as people. It helps me sleep.

**Lukas:** They are labor.

**Wil:** Yeah, exactly. a Shellphish unit of work. But exactly in in true Shellphish fashion, instead of going with a pre-designed, you know, some sort of orchestration framework, we just rolled our own. It's an insane monolith made by Audrey (rhelmot) that's been open source this whole time, By the way, anybody at home could have decided to pick this up and make their own CRS as well.

**Adam:** Yeah. in case you could trick another team into using your infrastructure.

**Wil:** I wouldn't wish that on them. I really wouldn't.

**Yan:** So, after we open sourced the our cyber reasoning system for the cyber grand challenge, we had well this this was 10 years ago. The only open source cyber reasoning system at the time. There were a number of other competitions of you know fully autonomous hacking around the world and people kept using the Mechanical Phish our cyber reasoning system in these competitions because it was open source and every time someone would email me like hey I stood up the mechanical phish and I'm like oh my gosh

**Lukas:** you poor soul.

**Yan:** People won crazy amount of money basing their cyber reasoning system on our cyber. It was really cool to see, but like it was painful for them

**Adam:** And there were other requirements that we didn't talk about, right? So, at least in the finals, you could use tons of cluster compute and you had access to what was it? An Azure environment to spin up your machines because you had this much greater budget than $100. But at the same time, you needed people not only to be able to dev their individual components on their machine, but also dev their component is as part of the pipeline using real inputs from tests. And so you needed them to be able to run the pipeline also locally. And even I think some of us were running the the whole system just on one machine.

**Lukas:** A little bit beefier machines are required these days, but yeah.

**Adam:** Well, 64 components running, you know, you need and some and some of those are fuzzers.

**Wil:** For semis I was able I was able to run it on my laptop at one point of like 12 cores which was which was pretty good that no longer possible but

**Lukas:** I mean one thing that I will point out is that that is kind of cool about it too is I mean I think twofold is one if you if you ask Yan right now right like what was the structure of the mechanical fish I think it was a lot more of the former of the kind of system where you had one database I remember because it was called Meister I think and you had one fuzzing thing and then that was trying to communicate with the other things but there wasn't I think it was in total maybe like 10 eight components something like that I think it was

**Yan:** yeah let's say 16 or less yeah probably closer to 10 yeah

**Lukas:** and so our system has grown a lot beyond that and The other thing that was cool about this though is because we had done this early, right? We had always designed the system to work like this and we had designed it to be able to run on 12 cores as well as inci 96 cores. I think we had a lot better of a start into the semi the post semi-finals round where now you're running in a cluster. You have way more resources. You have you can spin up variable number of fuzzers. You can autoscale to whatever degree. That was a lot easier for us because our system was always designed with that in mind because we needed to test it locally. But in the game we had way more resources already.

**Yan:** Can you give us an example of that that scaling factor like what's possible?

**Lukas:** Yeah, I mean I think currently right now I don't think there's even even with the system in finals where we had over the 10 days I think $50,000 of Azure compute that buys you like thousands of cores of fuzzers.

**Wil:** It was 85,000. Yeah, it was a lot of money.

**Adam:** That's where that 3 million went. Well, part of it and the other one went to an AI provider we'll talk about in a bit.

**Lukas:** But yeah, I think I think we had per target with eight consecutive or 10 consecutive targets, I think we had like a thousand cores per target of fuzzers that automatically dynamically spin up. And the nice thing is our system when there is no challenge available also automatically spins them back down, right? So we're not wasting money while we're not using it. If it turns out we we ended up disabling some of this for resilience, but we could orchestrate the system in such a way that if we have a single target, that single target can take all 8,000 cores of fuzzing and do something with that.

**Wil:** And of course, maybe to Yan's chagrin, as more components spin up that need the resources, the fuzzers will spin down to accommodate the amount that needs to be spun up.

**Yan:** Yeah so that the reason it's to my chagrin is early on in the AIxCC based on lessons learned in the cyber grand challenge and the complexity of our dynamic allocation in our infrastructure in the mechanical fish I pushed very hard for static allocations we're going to pause on x cores and patch on y cores and etc.

**Adam:** No, but I think your advice was more almost high level than that. It was simplicity. You said build a simple system and that is part of that.

**Wil:** And that's not what we did.

**Yan:** Hey, if you I knew you wouldn't. Every child doesn't listen to their parents and has to learn the same lessons. It's just the same goes with PhD students and advisers and the same apparently goes with hacking teams in DARPA cyber challenges.

## System Pipeline: From Input to Output [43:58](https://youtu.be/ozp7fBoOsIQ?t=2638)

**Adam:** Okay, great. So then can you give the people at home like the high-level bird's eye view of the pipeline? We'll go let's go Lukas if you can give us like the what so target comes in a what is a target at a high level. Let's not get into all the minutia but like what is a target and what happened to it through the pipeline.

**Lukas:** Yeah. So maybe for quick context in terms of the what is a target. One thing that changed from semi-finals is the organizers standardized on the OSS fuzz framework as a method of what should a target look like. And if you don't know what OSS fuzz is, OSS fuzz is a service by Google. That allows open source maintainers to add their own pieces of software. That could be as simple as writing a little docker file that allows you to say how here's how I can build my target and a little script together with a description that says hey where's the repository where if this giant system that Google has built finds bugs where can they report them to me right and so as part of that they've built this interface of like how do we make arbitrary pieces of software available for analysis And it requires a little bit of work by the maintainer, right? They have to write a Docker file. They have to write a script that tells the infrastructure, here's how you can build me. And Google has has this has made this available and I think it at this point has about 1500 pieces of open source software that have been integrated into this framework. And so when this target comes to us really what it comes is as two parts optionally three depending on the type of challenge. The first one being just one archive of all of the source code of that application right you can think of this as just the git repository taken, cloned and packaged up into a file.

**Adam:** Boom. Here's the code. Find me bugs and patch them.

**Lukas:** Exactly. And then the second part is that OSS fuzz integration wrapper which is that build script and the docker file and the metadata. Optionally, there is a third component for a challenge in the AIxCC which is of type delta mode where they give you a diff and they say, "Hey, when you apply these changes to the open source software, there's bugs, Find me bugs in the now newly changed piece of software, but in that version, only report ones that were introduced by this change. Like don't report ones if they were in the original code. We only care about what has been newly introduced. So that's generally what the challenges are. They're either full mode or delta mode and they come as these packaged pieces of source code. When they enter our pipeline the very first thing that happens and that happens in OSS fuzz as well is obviously we have to build the software a bunch of time. We have to

**Adam:** maybe not obviously if you were taking a pure AI based approach.

**Lukas:** That's fair.

**Adam:** Maybe pure source code analysis and AI. You don't actually need to build it.

**Wil:** You know, Lukas, we never ask the AI how we should build the software.

**Yan:** You never ask whether you should build the software.

**Lukas:** Well, okay. So, so one thing is as part of the game, the things that we can submit to the organizers are mainly twofold which is one we can give them a piece of data and say if you feed this piece of data to this software to this specific entry point in the software it will crash right. And so what then happens on the organizer side is they run that piece of software feed the data in and check well did it crash right and if it does then they give you vulnerability scoring points. The second thing we can report as a system to the organizers is a patch where we say okay if you apply these additional changes to the software and then run that same crashing input that you gave me previously does it still crash. If the answer is no, then you patched the vulnerability to some extent and there's some additional tests that they make that they run to make sure you're not like trying to game the system. they check their own patches against and so there's some scoring logic there, but that's kind of like the two things that your system reports is bugs in the form of a crashing input and patches in the form of a change that needs to be applied to the system. And so obviously you might want to re replicate this locally in order to make sure that the thing you're about to submit is actually valid. And so generally the first step is like the building part of the pipeline. And our pipeline doesn't build the software just once, right? You you don't just build it one time. You build it a bunch of different times for different purposes. So fuzzers need specific customizations to the software to be done so that you can fuzz more effectively. When you are trying to look at like hey which parts of the code has my input reached has my analysis tools reached you use coverage instrumentation that comes with a specific set of changes to the compilation. And so we built the the software a bunch of times and then you can kind of that's that's like the first layer of the pipeline. Then you have a layer of static analysis and like almost like understanding the software. So splitting it into different functions trying to find out what functions are there. Running existing vulnerability scanners for example like Semgrep and CodeQL trying to find any known vulnerable patterns. Maybe this is a first analysis step of LLMs where you give them a bunch of functions and you just ask them hey are these vulnerable right like purely by looking at the code what can I determine of the software and then that's kind of the second layer then the third layer starts which is most of the dynamic analysis so this can be traditional fuzzers we generally have mostly three with some customizations Jazzer for Java, AFL for C and then libfuzzer for C. And as well as LLM components here we've now built a bunch of them where they try to actually like feed we we ask the LLM hey can you write me an input that will crash the software right like here here's a bug here's a program location where I think there's a bug write me an input that tries to get there write me a grammar that tries to reach there right like whatever you can come up with like anything that produces inputs that we can actually test against the target software and say like hey perfect this crashed go forward. And then after this stage you kind of come to the triaging part I would I would call it where now that you have a bunch of these results. You have a bunch of crashing inputs. You have crash reports of like hey these were the stack traces when it crashed. Here's what the state looked like. Now you have to understand what is the actual bug that we found. Is this the same one in four different ways? Are they different?


**Adam:** And this was important for kind of game reasons, but we won't get into too much depth. But it also, you know, I there's the game, but I also like to think of the real world impact of this stuff, right? So, it's like, okay, but as a developer, you want to know that there is a bug. You don't want to know that there are I found a thousand crashes and turns out they're actually all the same bug.

**Lukas:** Yeah. And that's something that is very real. Like people are very annoyed if you just report them the same bug 10 times, right? Because it's a waste of their time.

**Adam:** Exactly.

**Lukas:** The other part that this is important though is not just for the game reasons. It's not just for the real world part of it. It's also the better you can do this stage, the better you could understand what the actual bug that you've discovered is, the more information you can give to the last part of the pipeline, which is the actual patching and the actual patch generation. where we now use multiple different patching solutions all based on LLMs in some some way shape or form just with different strategies of hey I have found this bug

**Adam:** And very smartly I have to say named named patcher and then a letter it was absolutely insane

**Wil:** yeah yeah no it makes all the sense in the world that we have patcher Y patcher Q and patcher G which isn't a patcher by the way Yes. So insanity and smart you were thinking and delta and dumb and whatever. Yeah.

**Adam:** Amazing. Okay. So then the patching component is at the end or there are other components.

**Lukas:** So it's near the end. So because once you get a patch there is one more thing which is A similar to the first step you need to understand is is this patch the same or similar to one I already have. But also you need to do a bunch of cross-checking of like did it make the crash go away, right? This is part of the patches generally, but it's kind of this idea of like you want to be sure that your patch is correct. So, the last part I would say is like a separate step of the pipeline is we have some fuzzing for example on the patches where we just try a little bit to try to get around the patches and make sure that they're not easily bypassable. And that's kind of like the linear progression of the pipeline. And then there's one layer above which is the gameplay axis of the pipeline, right? Where you now have all of these results. Now you need to decide, okay, which ones of them do I submit in what order? And do I want to submit them? Am I confident? that kind of

**Wil:** and deciding this strategy took I think 10 of binary and program analysis top scientists four or five days.

**Adam:** Hey, we also had some game theory people. At least two

**Wil:** At least two game theory people. Yeah. Yeah. But we made a strategy in the end.

**Lukas:** And even after that it's still the scariest part of the system.

**Adam:** Yeah. Which makes sense, right? you're talking about. I like that notion of like it at the top layer or the bottom, right? Because the system is doing all this analysis, but you need to communicate those results and actually play the game in some sense because it's not just your you're not just creating this stuff. So, you have to play the game. And so, if you end up not being able to play the game or you hit the wrong button or you keep, you know, doing something over and over again, that would be a problem. That would be

**Lukas:** or that change you made an hour before the deadline turns out to be to be not so good.

**Adam:** Exactly.

**Wil:** Yeah. I think that was the that was the the scariest part for sure which is we made all this cool stuff and and to us obviously this is this we did something really awesome but if in the strategy or in the game we can't actually show we don't submit anything for whatever reason or there's some failure and just even if we make it internally but it doesn't make it out externally then it doesn't count for anything.

**Adam:** Exactly. Which is great. Okay.

## Wildest Components: SARIF and Grammar Guy [55:28](https://youtu.be/ozp7fBoOsIQ?t=3328)

**Adam:** So Wil then so we know the scariest component or the scariest phase. What is the craziest wildest component in your opinion that exists in the system? And describe to us like what it does and why it's crazy.

**Wil:** Okay. I may have to I may have to give you two.

**Adam:** I only said one.

**Wil:** Yeah, I understand what you said. I don't follow instructions very well. Yeah. So one I think is our is our SARIF component. And I think it's crazy. One thing Lukas had mentioned that maybe we can get three inputs from the orgs. This extra third input can sometimes be this SARIF report which for those who don't know is just a way of representing like static static tool findings of hey there's a vulnerability here and our job is to say whether or not there's a vulnerability and instead of making impressive tooling or maybe some really cool information analysis.

**Yan:** You just said the organizers tell you there's a vulnerability. Why would they need you to tell them if there's a vulnerability?

**Wil:** Now, you're getting to the to the crux of the crux of the problem. The organizers say a lot of things. But in in this in this instance, they want us to verify what they had said. They give us an assessment that says, "Hey, there's a vulnerability here." And our job is to say, "Yes, that's a correct assessment," or "No, that's an incorrect assessment." And then

**Yan:** Why do you think they they they do this? Why would anyone care about this capability in the real world?

**Wil:** So the the best guess there's a there's a whole meta component to to all of this, but essentially the the things that you need to understand at the core is there's a vulnerability that exists. We want to patch this vulnerability and maybe there's a report of this vulnerability. And if you combine all of these three features, all of a sudden you start to kind of think a little bit of, hey, this maybe actually sounds like a like an issue that maybe somebody could open on a on a GitHub repo that maybe somebody's found a bug or maybe somebody's found a vulnerability or maybe there's some CWE that comes in that says, "Hey, there's a bug here"

**Lukas:** Or maybe they just found code that looks suspicious, right?" Like they they they might not understand entirely.

**Yan:** So these SARIF Reports might be mistakes made by an analysis tool.

**Lukas:** Yes.

**Adam:** Exactly. Because it comes into if that's a static analysis report fundamentally it hasn't executed the code. We don't actually know that there is a bug there. It's the tool says there I think there's a bug here but we know false positives exist in static analysis tools and so it may be lying or maybe incorrect or I think the proper way is thinking about it is it's over approximating the program's behavior and it's envisioned a potential vulnerability that doesn't actually exist.

**Yan:** So, Wil, go ahead. Sorry. I know.

**Wil:** So, back to back to the the the the crazy this component is crazy just because we decided to go with it, which is just ask the LLM. Just don't don't do anything complicated. Don't burden your brain. Don't don't use any CPU cores. Just ask the LLM, is there a bug here? And it turns out that it's it works quite well at least given given the format that we've seen from the organizers and stuff we've generated ourselves is you have a relatively high true positive rate of whatever of of assessing correctly or incorrectly.

**Adam:** So 65 components or 64 components are all devoted to finding vulnerabilities and patches. But you have just one component that just says yo is this report accurate?

**Wil:** I just need a yes or a no, man. Just trust me. Just trust him. Just trust him. That's all. But the the the real answer to the craziest component has to be Lukas's grammar guy. I don't think I've seen anything eat money faster. I've never physically felt myself get lighter as my pockets empty when when when grammar guy is active.

**Adam:** Great. So what is grammar guy? So this is this is great. So you can tell us like what are the inputs of grammar guy? What are the outputs and and what did that component do?

**Wil:** Yeah. So of course the underlying challenge to AIxCC is where is the bug? You can have the best patching in the world, you can have the best SARIF detection in the world. If you don't have a bug to prove that these things exist, then you really don't have much. So we developed essentially all of our or much of our bug finding capabilities on fuzzing. And on top of this fuzzing, we can't just have plain old AFL or libfuzzer because although these things do work in practice, OSS fuzz has been using libfuzzer for years and years and the bugs that it finds maybe occasionally and maybe every couple months. It it doesn't progress very much very fast. So Lukas had a had a brilliant idea which is let's mutate the input the input seeds that we can give to AFL. What if we could make these seeds inputs smarter, right? So we have the source code, we have great information like CodeQL queries, we have great information if there's a diff of hey this is code that's changed. So let's try and generate grammars that drill deeper and deeper into the program as we find more and more coverage. And come up with these as fast and as broad as we can. And that's really the the the money eater issue there is as fast and as broad as you can because although it's been incredibly effective. It's found bug without it our bug finding capability's maybe halved maybe 75 or 25% of what it could be. But it uses like 90% of our budget.

**Lukas:** 55, excuse you.

**Wil:** Well, 55

**Adam:** Of the LLM budget, you're saying?

**Lukas:** Yes.

**Wil:** But, of the soul it uses 90%. Anyways.

**Adam:** And is this because it's it's not good or the LLMs aren't good or because you need something different? Like why what's the core root cause of why it takes so much LLM time or budget?

**Lukas:** I think there's Yeah. So, I think I think there's two parts just just be beforehand. I think there's a I can't take all the credit for spending all of our money, right? Grammar fuzzing is an idea that has been around for a long time and it was kind of a natural one to try to apply LLMs to because it has been traditionally something that has required humans, right? Humans would go in and say, "Okay, here's the application. Let me understand how the format looks. Let me understand what inputs it expects." And then they would write a specification of like okay the first thing is a integer number from 0 to 10 and then it is followed by a string blah blah blah blah blah right and so this was this is traditionally very human task of like writing these grammars in order to make the fuzzer better at exploring the state space because it no longer has to consider the first thing being a number 11 right like it very much prunes the search space and so this is a pretty old idea But the LLMs kind of allow us to take that human part and replicate it with something that might not be as good as a human, but can do it a lot longer, a lot more often, a lot faster than humans can. And we actually had this already in semi-finals. One of the interns at UCB Sebastian has been, working on that for a long time. And built the initial idea of like, okay, we don't trust these LLMs that much. we don't know how good they are. Let's break down the task and make it simple. And that is something that kind of you can see in all of our pipeline. A lot of the older components had a lot less trust in the LLM, right? They trusted a lot less in the abilities of the LLM to decide itself what to do and instead really tried to railroad the LLM into like here's your task. You have one job. just do that one thing and then the rest of the system would be built into the components. And we had that initial grammar guy. But one thing that we tried after that was, you know, in between semifinals and finals, as these models got better and as they acquired more ability to, for example, call out to external tools and retrieve additional information. One of the things that I think the initial version of the grammar agent that ended up spending so much money initially was written in a day or two. That really is just a couple tool calls allowing the LLM to collect coverage and then trying out this grammar, producing a bunch of inputs, seeing what coverage they hit, and then asking it, okay, now do better, right? Build a better grammar. And as part of this, as the LLM explores the code, it has the ability to look at functions, it can look at files, it can rep through the source code, whatever tool calls you make available to it. As it does so, it accumulates context and it accumulates knowledge within the interaction of like here's stuff I've already tried. Here is grammars that have worked. Here's mistakes I made. And in that version, it just accumulates context infinitely. Obviously there is a boundary imposed by the LLM at which point we have to you know prune it and truncate it but really the idea was just let it have everything it's ever seen and see what it does.

**Wil:** Yeah. After after about 10 10 calls you hit that context window pretty goddamn fast. But I I mean something something else here. Grammar guy could well one of one of the reasons it's insane is that we had to base our budgets for this final allocation based on the fact that we are physically limited by the rate limit in which we can send Anthropic tokens for which grammar guy is is sending them. And so we had to literally split off less and and allocate more money to to OpenAI because we physically would not have been able to spend the money in the time frame.

# AI Model Preferences [1:05:30](https://youtu.be/ozp7fBoOsIQ?t=3930)

**Yan:** So may maybe we can kind of pull on this thread a bit with this question. Favorite AI.

**Adam:** Oh, I like it. Yeah.

**Wil:** I I think Anthropic for for both of us.

**Adam:** Yeah, daily driver usage or or coding or for coding? For sure.

**Wil:** Well, so there's an interesting thing here, which is I actually think OpenAI is great for maybe like more nebulous tasks or things that require decision or critique. But if you're asking to generate code, if you're asking for decisions to be made on code that are that are minute or specific, then I think Anthropic takes the cake for pretty much any any use case that we have.

**Adam:** Yeah, great.

**Lukas:** I think one more one more thing is like I think this is again kind of that shift but I think Anthropic was the first ones to get there. I think now some of the other models have caught up. So I think like Gemini for example

**Adam:** Claude up.

**Lukas:** They've claude up. Exactly. Gemini is now pretty decent at it. We weren't able due to rate limiting issues to use it to the extent that we wanted to. but also some of the newer OpenAI models. I think they've also realized that this paradigm of like tool calling and being able to write code to do more things is just so much more powerful because it allows the LLM to think about less and it just has to write some code that does the work for it. Right? The same way that people were always harping on these LLMs about, oh, they can't do math. Well, just give it a calculator, right? It doesn't have to be able to do math. It just needs to be able to say what it wants to be solved. As long as it can do that, the the machinery that you build around it can do that hard work for it.

**Adam:** Yeah, that's cool. And it goes with what I observed when using Claude Code to try to implement some tests, which was my kind of contribution to the AIxCC push. And it would actually I watched it. It would I told it to like either generate a test case to hit here or fix a test case or whatever. it would add debugging code into the the this the system, run the test case, look at the debugging code, and then be like, "Oh, yeah, I see the problem. It's this." And then it would go back and delete it. That's like what was the crazy thing to me.

**Wil:** I mean, it's been very interesting to see these tools like progress over time from where we started in in 2023. We've mentioned a couple times about how how our whole paradigm has shifted, but like the I tool calling didn't exist, right? Tool calling was kind of like a a fresh thing there. We built our own tool calling capabilities initially like I remember making our own like Python execution sandbox where we say hey can you generate some arbitrary code for us and then we execute it and feed that back into the system. Now there's entire frameworks that allow you to build up the the agents and tool calling is is almost a given with any model you know minus a few. But it's it's been really interesting to see like the the industry and everything mirror us in a way or the things that like we've noticed lacks or or wants that we had and made it and created them for ourselves and then you know other people obviously had also wanted these or or needed these and then they developed it kind of side by side which which was interesting.

**Adam:** Great. That's awesome.

## Competition Results and Predictions [1:08:56](https://youtu.be/ozp7fBoOsIQ?t=4136)

**Adam:** Okay. And so yeah, I think kind of we're running towards the end, so we'll kind of close it out. So what's happening now? So we sub all of the team submitted at what was it? June 26th. Was that the...

**Wil:** Yeah, that was the morning of June 26th. 8am.

**Adam:** A date that will live in some people's memories, but not ours. And so we submitted, every team submitted on 26th, and the organizers are running all of the all of the CRS's on all of the challenge problems. and we'll find out. Yeah, right now as we are recording this they are running that. And so okay maybe final or couple final questions predictions predict how do you think ARTIPHISHELL is going to do in this competition.

**Wil:** So PR response we're first place right obviously real response I think we're probably I would say second or third.

**Yan:** What do you think will be the the differentiator?

**Wil:** I think that all the all the gaming all the the theory crafting gaming dedup stuff if you did deduplication correctly is is what makes you number one. I think that if you're able to accurately identify, hey, I found, you know, these bugs and they're different out of a thousand crashes, that puts you on on number one. I think it's very easy to go all in of I only found one bug or it's very easy to go all in in the sense of I found a thousand different bugs, but if you're able to differentiate even like two or three bugs, I think that's what actually puts you at at number one.

**Lukas:** Yeah, I agree with that. I think the and this is not to sound, you know, deluded or like grandiose or anything, but I think we've built an incredibly good system at solving the task. I think the only question remains of like how well does that system play the game. And I'm sure there's some team that will find new bugs that we haven't and I'm also pretty sure we'll find bugs that other teams don't have. I think there's always wiggle room in the results. But I think what it comes down to, and I think the thing that I'm most scared of is that, you know, something happens and our system melts down or hopefully not. Or we have bugs and we don't submit them, right? That would suck. But I think that notwithstanding, I think we have a pretty pretty good system that we've built and I'm pretty confident that we'll do well.

**Adam:** Awesome. So, based on that prediction, what is in very short your secret sauce? What's like the Shellphish ARTIPHISHELL secret sauce?

**Lukas:** I wanna wait for Wil's answers.

**Wil:** Well, yeah, I think we've said this in actually a couple different places, but the the number one is...

**Adam:** Oh, please tell us again. We would really appreciate to hear from you.

**Wil:** Yes, of course. Use LLMs, but they have to be grounded, give you great great output, very usable, but a lot of times it's not 100% correct or 100% the truth. make sure that you have some way of verifying that what it gives you matches with reality. Whether this is test cases or maybe you're able to gather constraints from somewhere or actually just run it. I I think that being able to trust but verify is the is the number one key to success here.

**Yan:** The term that I came up with I think in in the end for this is you have to baby proof your code from the... Yeah. as as the parent of young children, I love that terminology.

**Adam:** And because you came up with it, so obviously...

**Yan:** Oh, well, no, no, no. I think I think it was it it

**Lukas:** Quick Yan, come up with some 80s video game that had the term in it.

**Yan:** That's right.

**Adam:** Incredible. Okay.

**Lukas:** And actually, can I...

**Adam:** Yeah, go ahead, please, Lukas.

**Lukas:** So, I wanted to follow up real quick because I I have a little bit of a more concrete answer that I think might be might be cool, which is I think one thing that I really like is I think it's very easy in quotation marks obviously in terms of a two-year research project, but I think building LLM components is the easy part in a sense, right? Like you have to make them work well and that's what Wil was trying to hint at. But one thing that I really like that our current system has is we've kind of approached it from two angles. We've approached it from the angles of making the LLM be able to better use the tools that we give it and make sure that it really is good at that. But the other thing that I think is really cool is we've tried to build traditional analysis systems that are based around what the LLMs are able to give us. So Wil mentioned grammar guy as like this tool that writes grammars. Well, we've also then taken that idea and built a lot of software around the idea of okay is this tool is able to give us grammars. Let's try to use them in additional ways. So let's feed those grammars back to the original fuzzers to fuzz with those grammars instead of just let the LLM do stuff with them. let's try to find ways of augmenting these grammars with additional information where we are able to distill some of that idea of what the LLM was trying to do. Right? So maybe the LLM maybe we can detect the LLM was trying to create audio files. We might not know exactly what the LLM was trying to do, but we can use that pattern recognition ability and say like, hey, this looks like an audio file. Let me try to automatically use these existing grammars that I have for audio files. And so I think this interplay back of like this LLM produces information and we use that to make our traditional analysis better is something that I think is very cool in our system that we didn't have before.

**Yan:** So so this is super cool because basically we started you say you you started with the traditional program analysis for the first couple of months and then you started splashing in more and more and more AI. You can imagine a different approach from researchers that have more of an AI background that start with AI and maybe later on start splashing in more more program analysis. Do you think that there will be these two competing approaches like over in an overarching way in the AIxCC maybe three teams do one thing and four teams do another or do you think everyone is going to kind of end up with the same place regardless?

**Lukas:** I don't think everyone's going to end up in the same place. I think there's a lot of difference in the shift in focus, right? I think there's almost certainly teams that invested more into these ideas of like let's just make the LLM really good. Right? Like I think there's I think it's probably fair to say that that might other teams have done more in that direction of like trying to build different versions of these systems. I think the other direction of teams that have done more maybe only rely on fuzzing is possible, right? Like maybe someone decided to not use LLMs except for patching at all. I don't know. I would imagine not because it's easy enough to at least do the minimum to get a little bit of an advantage. So I think it's there's room for that space to to shrink. But I think everyone will end up with some mix of the two. I can't imagine why you wouldn't, right?

**Yan:** Yeah. Yeah. Of course.

**Wil:** It's easy enough to mix these things together. I think I think there will be some two kind of groups, but there's not going to be as much disparity between them as these people went all in on one and these people went all in on the other. It's like these people just were more comfortable with with doing this type of work rather than than the other

**Adam:** Which makes sense, I know there's a selection or a a forcing function of quals, right?

**Yan:** Yeah. And the the prediction basically people probably will have started on maybe different parts of a sides of that spectrum but we'll meet somewhere toward the middle.

**Adam:** We'll see.

**Yan:** The CGC...

**Adam:**  Go ahead.

**Yan:** For the CGC. I was shocked at how similar all of the final designs were of the cyber reasoning systems. Everyone had a fuzzer, a way to help the fuzzer get unstuck when it reached the you know parts it couldn't fuzz through and a general patching engine. That was for the most part what what which was really interesting. All the minutia differed but the high-level approaches were similar. I'd be really interested, maybe we should do another episode afterwards with all of the teams.

**Lukas:** Yeah. Yeah. One thing I'd be curious to see is if one thing where I can see a little bit of a gap in the spectrum is how much did teams try to do very vulnerability specific or target software specific things. Right? So did teams try to build agents that are just really good at only buffer overflows but nothing else. that kind of an idea where I think we fall on the end of we try to treat everything the same and we try to explore the code as evenly as possible and we don't have we have some components that are specific to specific types of bugs but I think that I'm more curious to see if like is did anyone go full in like we have 30 different LLM agents each one doing just one thing really well

**Wil:** I really really hope somebody went with the Skynet approach We talked about doing this ourselves but of having like like our our orchestration is very like input output driven but I really think there's something to be said for an approach where you give the LLM control of oh I think this problem is better solved with static analysis. I think this problem is better solved if we slap on some fuzzing for a little bit. Oh, I found this interesting thing. Let's actually use this other tool that I can I can do. If there's some LLM or some team that's super heavy into LLM, I really hope they took some some approach like that. That would be that'd be awesome to see.

**Yan:** What about a single prompt? Develop a cyber reasoning system. Go.

**Wil:** Need more be said?

**Yan:** And it just like bootstraps.

## Final Thoughts and What's Next

**Adam:** Okay, final question and then we'll let everyone go. Lukas and Wil, if you knowing what you know now, if you could change one thing about your approach to AIxCC, could be team-based, technical, whatever, what would you change? And you can also say, I would never have done this in the first place.

**Wil:** I definitely would have done it still.

**Wil:** Yeah. Wil, you want to go first or should I go first?

**Wil:** You go first, man, if you got an idea.

**Lukas:** So, I'm going to give you a little bit of a copout answer because I think at the end of the day, I wouldn't do anything different. Like, realistically, from the place we started at, this was the natural version for our team to go. And I think we kind of ended up where I expected we would go like not not necessarily with the same system, not with the same complexity, not with the same component, but I think it was always trending in that direction. I think if I had to start over now in order to try something different, I would do the second thing that I just mentioned. I would try to go LLMs first, right? Try to just just because I want to know what it would look like. So, I really hope someone did it. Is like do LLMs first, build LLM agents for everything. and build custom LLM agents that are really good at maybe even something that I'd heard a couple times was this idea of like really infusing the LLM with as much personal information of how would I solve the task and trying to follow the LLM make the LLM follow what a human would do. I think that would be really cool to see and I think I'd be very curious to see how much how far you can take that. I hope someone did. Because everything is going to be open sourced at the end. So, I can't wait to read the code.

**Adam:** Yeah, that's gonna be great. So, you would have rather you would have just done AIxCC like four times is what I heard and just done different strategies.

**Wil:** He just wants to be every team himself.

**Yan:** Cool. The system feels very Shellphish. It it was very cool with it's... Yeah. Anyways, yeah,

**Wil:** I I I think I I imagine it would be difficult for us to really do anything differently given like how technology kind of ramped up over time. I think maybe increased adoption of like LLM as time goes went on because I think we really had kind of like a sticking point of pre pre-quals after quals of like oh we're only using LLMs a little bit to oh let's use LLMs for everything that we actually like think is good. But beyond that there's one singular thing I would change and it is use a monorepo from the beginning. I think submodules are a curse. They are the spawn of Satan. They have bitten us in every which way that is possible to be bitten by submodules. If we had a re a monorepo from the very beginning then I think we could have legitimately saved like 10% of dead dev time in the in in quals.

**Adam:** Vindicated. When Yan was saying keep things simple, I said use a monorepo.

**Lukas:** Yeah, I think [unintelligible..]

**Adam:** Kids need to learn their own mistakes.

**Yan:** I know Adam said last question, but like one more question. You said second place for guaranteed. Boom. Maybe first. So, second place. What are you going to do with those three million?

**Wil:** Three million. I first take a break. It's been a long two years. And then make some make some more cool stuff, man.

**Yan:** Team vacation to the moon. Can we go do that for 3 mil.

**Wil:** We could probably send a couple of us for 3 mil.

**Yan:** Nice. Let's do it.

**Adam:** That would cost you way more money than that I think.

**Lukas:** I think we just pay for the LLM to write all of our papers going into the next 20 years. You just buy LLM credits to do all of our research so we don't have to do anything because...

**Adam:** Hey, that'll save me a lot of money on PhD students.

**Lukas:** Exactly.

**Wil:** In this economy?

## Closing

**Adam:** Awesome. All right. Well, thank you, Lukas and Wil, for joining us. We're super happy to have you today. I'm Adam D. You can find me online, Adam Dupe. He's Zardus. You can find him online at Zardus. Together, we are CTF radio. And you can find us online on YouTube or Twitter or X @ctfradiooo. You can send us questions through email at CTFradioooo@gmail.com. And you know what? We may just use your questions on a future episode of CTF radio. I think from what I've I've seen here, we have we didn't even get into there's like so much craziness we could have got into about the stuff that Yan got up to during the final push. The the almost lack of actually submitting anything. So there was so much stuff we could have got into that we didn't that maybe we'll have to have another episode. But that'll either be a happy or sad one depending on what place we get. But anyways, if you have a questions for Lukas and Wil, feel free to send them to us. We'll be happy to do that. So, take care everyone and happy hacking.