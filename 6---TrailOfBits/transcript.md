# AIxCC Trail of Bits Team Interview

**Hosts:** Adam (adamd) and Yan (Zardus)  
**Guests:** Michael Brown and Evan Downing from Trail of Bits

---

## Introduction

**Adam:** Hello everyone, welcome to CTF radio. We're here in our six out of seven AIxCC team interviews. So Yan, it's been quite a long road. How are you feeling?

**Yan:** I am feeling great. One, because I am running on zero sleep, which means I'm on a complete exhaustion high with a lot of coffee. And two, because it is super cool hearing from every team over and over how hard they went for the competition, right? It's one thing to have millions and millions of dollars on the line and someone at some point swoops in and grabs the whole bag, but hearing how hard people have been pushing has been super cool and also helps frame our own efforts and put them into perspective too. 

We've been pushing forward for years and it's really interesting to think that this whole time we've been going it, it felt like everyone's going it alone but there are six other teams for sure suffering in parallel - you just couldn't see them.

**Adam:** And actually on that note, a bit of backstory that I probably wouldn't mention, but I think it's relevant here - our next guests, they were one of the first people to respond. "Yes, we're super happy to do the interviews, but we're taking vacation, so let's do it later." And that I think perfectly ties in with the effort that it's clear that teams put into this event. After the submission, people need time to recharge. And it's actually really brilliant after the submission, but before the results come out. So you don't even have to be over the moon or completely dead. You're just like, you don't have to care.

**Yan:** Exactly. Yeah, for the vacation time.

## Team Introductions

**Adam:** Cool. So we have with us today Trail of Bits and we have Michael and Evan here. So Michael, you want to go first and introduce yourselves to the great people out there?

**Michael:** Yeah, sure. So I'll start with our company. If you're not familiar with us, Trail of Bits is a cyber security services company. We do a lot of commercial work, but I'm part of our research and engineering practice and we do a lot of work for DARPA. So we do a lot of research for government clients, including ARPA, which is now kind of a co-sponsor/co-runner of the AI cyber challenge. We also do some work for big tech and commercial clients in other parts. So we're about 120 people. 

I personally am a principal security engineer - that's my title. I lead up our company's AI/ML security research team. So kind of two flavors of that. One flavor is applying AI/ML to security problems which is right down the alley for AIxCC, and then we also do a little bit of work on securing AI/ML pipelines mostly with supply chain type stuff. So I've been with the company for three or four years now.

**Adam:** Wow. Cool. That's awesome. Evan, what about you?

**Evan:** Yeah, hey, I'm Evan Downing. I'm a senior security engineer at Trail of Bits. I joined last year as part of the R&D group under Michael and I've been part of the AICC team since I entered in the semi-finals. So, it's been fun to work with them and grow with them. And particularly I was in charge of one component of the CRS, but also we had our hands in other areas of it too. And yeah, just enjoying working and contributing as I can.

**Adam:** Awesome. Wait, so you joined last year - did you join right before the qualification and did you know that you'd be doing this?

**Evan:** I did. Yeah. So I joined April of 2024. So we already knew we were going to go into it. So it was right when we were set up to actually get all the semi-finals rules and start hitting the ground sprinting. So that was part of that.

**Adam:** Great. So they didn't just pop that on you. They didn't like you started and then the next day after orientation they're like, "Oh, by the way, you're going to help out with this giant AIxCC."

**Evan:** No, I mean it was planned. It was introduced to me that I might help out with that when I was doing my interviews. But yeah, so it wasn't any surprises necessarily, but it was definitely right up my alley and right up my experience level, so I was comfortable getting in that position.

## Team Structure and Background

**Adam:** Awesome. Very cool. Well, yeah, thank you both for being here today. We're really excited to hear from all the teams and specifically to dig into your team. So, can you give us maybe some background on the team about roughly how many people, what's the size of the team? I think Michael gave us a great overview of Trail of Bits as a company, but inside of there, how much were dedicated to AIxCC?

**Michael:** Yeah, sure. So our AICC team is entirely composed of people who work at Trail of Bits and also people who worked at Trail of Bits before the competition got started. I think at one point we briefly entertained the idea of bringing somebody on to assist, but we ended up staffing it entirely internally. So from the beginning all the way to the end we've had about 10 people - between eight and 10 people working on the project at any given time on a meaningful basis. 

We had a large number of people who helped out in the beginning with ideation and running some stuff to ground and helping us out with various rubber-meets-the-road type things, but this was all before we actually knew really even how the competition was going to be structured. So that was back when there's this huge wide open possibility of what this actually could be. And then when it came down to what it actually became, we really had a team of about 10 people. 

Of those 10, we typically had about eight at any given time actually working on the CRS. And we maintained throughout the entire project a two-person, I call them our red team, whose job was to basically make challenges that would try to make our CRS, for lack of a better term, puke, and try to challenge us that way. Yeah, big shout out to Brad Swain and Alexandre Gario on our team who did the hard part of making us work extra hard to try and live up to a standard that was a little bit beyond the exemplar programs we got from DARPA.

**Adam:** Yeah, that's great. I mean, I think that gets into a lot of AI - one of the main focuses that I see is on benchmarking, right? How do we create good representative benchmarks?

**Yan:** Reading between the lines, this means that to support a red team, you would have had to have a runnable CRS pretty early on and continuously.

**Michael:** Yeah. And the way we do things at Trail of Bits, this is really for all of our research projects - we do like an MVP style development. So we make the absolute barest bones possible minimum viable product that does end to end whatever this impossible-to-do thing that we proposed is. So even if it means it really only supports one exemplar program or a very tight narrow definition of that, we started off with that and then we started adding support for all the various aspects of it. 

So now admittedly there was some lead time. We knew what exemplar programs were going to look like but DARPA didn't give us very many. So we sent Brad and Alexandre out with this mission of "go find hard stuff that's going to make us break" so that we don't train to specifically the test that DARPA has given us and then find out the test is a lot harder and we stumble. 

So yeah, and then as we learned more about what the actual system was going to look like, how long the cyber reasoning systems were going to run, what kind of resources we had, we would adjust fire on what kind of challenges we were trying to create. But yeah, absolutely Adam, to your point, it was a data set problem. We got an N equals two or three when it comes to data set size for example programs from DARPA in the semis. We got more in the finals, but it was still, you could count them on two hands. 

So unless you want to stretch the capabilities of your subs, you can't just go with two or three examples and hope that you do okay. Actually honestly we stumbled quite a bit in the semi-finals when it came to Java challenges because we only got one Java challenge ahead of time and we could process it. Everything looked good on our side but we didn't have time to make a lot of Java challenges on our own. And then when we get to the semi-finals our cyber reasoning system really struggled. I don't think we got any points on any of the Java stuff. 

And we really think it was probably more due to the fact that - it wasn't due to the fact that the CRS was incapable because it really performed quite well on the C and C++ challenges, but we think something went wrong with the Java class path or the types of CWEs that were being examined there were things that we didn't really tune our system for. So we actually never really found out what actually happened with it because we didn't get a lot of information back. So we do better on the Java challenges now and we had Ryan and Alexandre find a lot more Java challenges the second time around, that's for sure.

## Company Background and Open Source Approach

**Adam:** That's great. Okay. So, yeah, before we dig too much into the system, I want to roll back a little bit. And so, you guys were one of the small business prize winners. So, the AIxCC must have been on your company radar for a while, right?

**Michael:** Oh, yeah. That's for sure. Like I said, so as a company about 30% of our company's revenue comes from long-term research contracts with the US government. So DARPA, ARPA, sometimes ARPA-E, I-ARPA, some of those other star-ARPAs that are out there. But for the large part, we do a lot of our research - about 30% of our revenue comes from research programs. And within the research and engineering division of Trail of Bits, it's basically flipped. About 70% within that division comes from DARPA. So they're our primary sponsor. 

So we're hyper aware of the things they put out. This has been something - a research area of mine that was a big part of a PhD that never got finished and then also a big part of what I've been interested in researching for the last five years. So personally, I was pretty hyper aware of this, but also, more largely before my time at the company, Trail of Bits competed in the CGC, didn't make it to the semi-finals due to an unknown element of the scoring at the time that ended up costing them a spot in the top seven. But they teamed up and went to the finals with another team. They ended up not placing there. 

So, Trail of Bits was heavily involved in the Cyber Grand Challenge and this being a spiritual successor to that. It was something that, the minute it got announced, we were all on the DRO list, so to speak.

**Adam:** Very cool. Yeah. That's awesome. So then I'm curious if you can - and of course if you like, we all understand your company, you may not be able to say things - but I'm curious how the requirement to open source the systems either altered your approach to participating or was it not a barrier at all? When especially with the - because I think that was from the jump - as part of the small business prize you needed to guarantee that you'd open source it and all of that.

**Michael:** Yeah, it really was no problem for us at all. To the maximum degree possible. And this is companywide. This isn't just with research projects. Trail of Bits tries to open source everything we create. That's one of the really great things about working for a services company, not a product company. Trail of Bits has made successful products in the past, but they get spun out as separate entities and we remain a services company. So we don't have any financial incentives to engage in this heavy productization. 

Now that's not to say that our CRS might not get productized after this, but realistically I mean a part of the reason why Trail of Bits is well known in the community is because we open source our tools. Tools like Manticore have been really popular. A half dozen tools that Evan and I have created over the years either at Georgia Tech or at Trail of Bits have been made open source. So, we really try to put everything out there. So, this was really no factor for us at all. 

I think it was a consideration in the finals when it came to open sourcing AI models, in our decision about whether or not we were going to try and fine-tune or create our own model.

**Adam:** Interesting.

**Michael:** So I think that was a consideration there. But realistically when it came to open sourcing the CRS, I mean, we were going to do it anyway.

**Adam:** That's great. Okay. Awesome. Yeah. It makes sense. It's like a selection function, right? I'm sure we never would talk to the teams that would have submitted except for that open-source requirement. So, that's great.

## Buttercup System Overview

**Adam:** Cool. So, maybe now can you - you mentioned Buttercup. So, can you give us the high-level overview of how the CRS works? The 10,000 foot view.

**Michael:** Yeah, sure. So our CRS is called Buttercup. And based on how the competition ended up being structured, it really heavily influenced our design. So Buttercup's basically a large distributed system that works and functions basically in a pipeline. So early on when we first saw the original structure of the competition, we saw there's basically three things that you have to do to win the competition. You have to discover vulnerabilities. You have to characterize or contextualize vulnerabilities. You have to patch them and then kind of item three and a half is you just have to manage the competition or the gamesmanship of this, but it's not really a major task. 

So as most people know, and I'm not going to get deep into the rules here, but the competition requires us to find a proof of vulnerability. So we've got to find a crashing test case and you have to do that before you can patch. That constraint was loosened a little bit for the finals but more or less you have to find a vulnerability then you have to patch it. So A precedes B, B precedes submission. So we have everything set up in that way. 

So we scaled different aspects of our system or different components of the system and replicated more nodes for certain tasks than others based on how that pipeline worked. For example, we have lots and lots of fuzzing nodes, a relatively or comparatively fewer but still a lot of patching nodes. That's because you got to find the vulnerabilities first and then patch them. 

So at a high level view, the CRS receives or communicates with the competition infrastructure with an orchestrator. The orchestrator is where all of our scoring strategy and gamesmanship lives. That's component 3.5 there. Then the orchestrator sends or coordinates the actions of the other groups of nodes. One of which is vulnerability discovery which more broadly contains two subcomponents that fuzz the target - fuzz the available fuzzing harnesses. We use large language models to help us generate seed inputs that are either likely to trigger certain types of vulnerabilities, help us explore more of the code base, or otherwise just generate interesting behavior. So that vulnerability discovery component is the first step of the pipeline. 

The second step of the pipeline is this contextualization process. Which this is what Evan was in charge of. At the high level it is a collection of static analysis and other automation type tools to feed information to both the CWE generation and the patching system which is where we also use a lot of large language model support. So this provides additional context that is necessary for solving these problems with large language models. 

So once we get a vulnerability from the vulnerability discovery component and once we've contextualized it, it goes off to the patcher. The patcher generates candidate patches, figures out which ones work, which ones don't clobber existing functionality. And then once it validates one of those, it submits or it sends that back to the orchestrator to submit that. There's a little bit more in there with the idea of the SARIF broadcast that I didn't mention. Most of that logic actually lives within the orchestration component. We actually didn't handle the SARIF broadcast very much if at all in our CRS.

**Adam:** Nice. Okay, great. But then so this orchestrator is - I guess a little bit more detail. What kind of languages are the components written in different languages or does everything kind of standardized? Maybe we can dive in a little bit deeper.

**Michael:** Yeah, sure. So, our original CRS that we made for the semi-finals, it had a little bit of Rust in it. Our vulnerability discovery component was written in Rust. But for the most part, I'm sure you've heard this before, everything's in Python for the most part. So, that was a common language, easy to implement, easy to test, a lot of that kind of stuff. So, yeah, it's mostly written in Python. In the finals, it's entirely written in Python. At least the code that we wrote, anything that we've vendored or included as a dependency, it's in whatever language it was in, but anything we wrote was more or less in Python. 

So the orchestrator is probably the only part of the system that is - I mean there's probably some other random node somewhere like a task server or something. But for more or less the orchestrator is the only single choke point in the system. Every other portion of the pipeline is highly replicated. This is mainly for uptime and for throughput when some of these later rounds have quite the scale that you have to handle when it comes to target programs. 

So yeah the orchestrator is probably the only place where we only have one of them. And it mostly just communicates with message queues to the other components, but it does also house all of our strategy for how we're scoring, how we're deciding which POVs to submit, which patches to submit, whether or not to attach a SARIF to them, bundling, all of that stuff happens there, which is great because we really practice a lot of separation of concerns to try and make this problem tractable.

**Adam:** And did that help with the testability as well? You mentioned making sure testing with red teaming and stuff. Did that allow you to then test each component separately while also testing the whole system?

**Michael:** Yeah, absolutely. That design was intentional. One of the great things about Trail of Bits and the wide variety of work we do here is that we didn't really have to look outside of our tent to find talented software engineers who've worked on systems that need a lot of uptime and need to be reliable. We didn't have to look anywhere else to find researchers who were good with AI or researchers who were good with machine learning, researchers who were good with software analysis. We had everybody under one roof. 

So one of the things we knew would be an advantage for us going into this was as an established company with personnel to actually do this. We knew that we could always put more work than I think a lot of our competitors could into maintaining reliability, robustness, uptime and all these engineering aspects. So even though this is a competition to drive forward the state of research, we did an embarrassingly large amount of engineering into the system which included we had basically some version of CI/CD that was running one of the - I think it was libxml2 - one of the targets that basically every time somebody pushed a commit to GitHub that we ran from end to end, fired up the entire CRS. Towards the end we had to turn that off because we were running out of credits. But for a long time, even if you just changed comments or updated a configuration file, it ran everything. 

So, we kept a close eye on whether or not we were breaking things as we go because like I said, everybody was working on different components. We're working at a rapid pace. Everything's got to get plugged in. And the integration, we didn't want that to be an event or to be a headache on its own. So, we largely automated that.

**Adam:** That's great. How much did each run cost?

**Michael:** It didn't cost a whole lot. So we actually got a shout out from Andrew Carney in the semi-finals. He said we were the most judicious use of the large language model among all the teams. I think he told - I don't know if it wasn't him. Somebody one of the organizers told us that for one of the challenge projects that we use $14 in LLM credits for processing.

**Adam:** Wow.

**Michael:** And your final submission and your call submission were similar on this?

**Michael:** Yeah, we were - so we eventually tuned and scaled the system to use more resources because they were available. But in the first exhibition round when we got our report back on how much we used, I think we had a budget that was like $5,000 or $3,000. It was several thousand. We used $162 and we found and patched all four vulnerabilities that they put out. 

So, yeah, we were quite efficient and also the compute was more or less in the same boat. So, we actually didn't really use a ton of resources. We started getting to the point at the end we're like, okay, we actually have to use these things otherwise we're leaving stuff on the table. So we actually had these weird problems in the last couple of weeks where we're like, can we increase the number of fuzzing nodes by four times and this thing will all fall apart or not? And yeah, we had to answer that question. So yeah, most of our CI runs, they didn't actually cost us all that much because we were always really resource conscious when it came to how we designed and how we built the CRS and how we used AI, how we used compute.

**Adam:** That's great. We were actually talking I think Lacrosse and SIFT had a similar usage of LLMs and they were advocating for a - they're hoping that maybe DARPA will do some kind of award for most efficient CRS in terms of bugs found versus money spent, right? I think there actually is an interesting decision space in there of finding the different CRSs and what resources they can use.

**Yan:** So, I was talking to someone today. I mentioned early on, I think throwing around strategies and various approaches, we calculated how much it would cost to just put every line of the Linux kernel through GPT, right? And it was like $10,000 or something at the time. And I was talking to someone about this today and they said, "Well, depending on what kind of bug you get, $10,000, that's not a bad investment." So, maybe you've been thinking about this all wrong. Maybe it's about throwing the maximum money in. But I think that there's this reduced returns that happens eventually.

**Michael:** Yeah, for sure. The point of diminishing returns is really real with applied AI particularly now that applied AI to security problems looks very much like you're paying a third party for the AI. The AI is incredibly compute intensive. It's one of the things we considered at the end of this which was we are going to open source this, we are going to try and share this with people. It doesn't really do anyone a lot of good if we make a system that requires $50,000 in compute and $20,000 in LLM credits to find you a couple of bugs. 

It probably exceeds most of the bug bounties you would get if it was that kind of situation. Value and risk to the business is not always that high. So really we wanted something that people could use because I mean if you think about it, a good portion of AICC's infrastructure is based on OSS Fuzz. So if you require big tech level organization to run this system at the end of this, the only people that are going to benefit are the big tech organizations because they will just take Buttercup's patching component and slap it onto OSS Fuzz and then now OSS Fuzz Plus or whatever they want to call it does a great job of submitting patches. 

Through Google or through whoever, substitute whatever organization, through them we've now helped the open source ecosystem but that doesn't help when you want to port this to other places that also need security services like embedded systems, hospital infrastructure. They don't have the money to go stand up their own Google and data centers and all this stuff to run this stuff. It was a big goal and a big design decision for us to say like yeah we're going to use a lot of resources now to try and win this competition, but wouldn't it be great afterward if we could tune this down, run some experiments and say, yeah, we spent 100% of the budget in the competition, but we got similar results by tuning everything down and spending maybe 20% of the cost. So, that's an interesting research question for us.

**Adam:** Almost like distilling a model down in some sense, right? It's like distilling a CRS down into something that's more tractable.

**Yan:** Do you have any preliminary ideas based on your testing? It sounds like you've definitely done an above average amount of testing compared to the typical competitor in this.

**Adam:** I don't know about that. We had a button that anyone on our team could press to run a full run on any target and they were like, "Yeah, I click this button. I spent $250 to run this."

**Yan:** Definitely true. Considering how much I've complained about the testability of ARTIPHISHELL in our podcast, it was shocking.

**Adam:** Not saying that was the most efficient way of doing that, but when the money's not coming out of their pocket, they were very happy to click that button.

**Michael:** Yeah. Yeah. The people had the button. I mean that was certainly a factor for us too. We ran a bunch of - almost every week for the last two months of the competition we were running an exhibition round scale version of Buttercup mainly to shake loose reliability type bugs that you can't get when you know like it was great that we had CI/CD that was running every time you push a commit and would make sure that the toy example would run. That would cost us a couple hundred bucks at absolute most. But we would spend our LLM credits and when we spend our compute credits, it was like $10,000/12,000 at a time. 

We got to the point where our very last run right before we submitted, I was actually watching our Azure update as at whatever cadence it updates. I was like, "Turn it off. Turn it off. We hit 100K." So,

**Adam:** yeah, we maxed out credit card at one point. We hit the max and I had to keep an eye on it and just feeding money into that card because the Claude credit and the Azure hold were just going way over. It was pretty wild. But yeah, that's the - there's definitely an interesting trade-off there between playing the game and creating a system that lives beyond that's usable by a non-tech giant. I think that's kind of a great point. 

**Yan:** And I also love that concept also with integrated CI. It all goes into this life beyond AIxCC, right? If you have a CRS that's impossible to deploy and untested and has unclear components and connections, it's much trickier. Now you mentioned you had your custom written orchestrator. Were the glue pieces between that and the components - are those off the shelf, were those custom written?

**Michael:** We use Redis queues and Redis databases to handle most of our persistence. So we relied on Kubernetes to do most of the uptime management. So it was set really aggressively that if anything went down it would just kill it and restart it. So we persisted everything to disk that was a meaningful artifact. And then so basically all of our individual components when they would wake up whether it's the first time they were started or they'd been restarted, they knew just to go look in a particular queue for a task to be completed and we really relied on that for scaling the system up to large number of nodes are all performing the same task to different nodes that are performing different stages of the task. And then really when it came to the functions of the orchestrator it basically did the same thing. It's just there was only one of them because we needed one central place to decide what we were going to submit and this worked out great.

**Adam:** Yeah. Yeah. For the most part. I mean, we had our problems. I mean, so I don't think we told anybody this, but for the second exhibition round, we found eight vulnerabilities and patched six things and we all thought that we were cooked. We're like, "Oh my gosh, we're just stumbling. This is awful." We found out six hours in that the way we were creating file names for POVs was putting too much information into the file name. We were exceeding the size of the maximum length available for file names and that was crashing nodes hard. 

So we went from basically we did the best in the first exhibition round and it was only two challenges, four vulnerabilities, a very small scale but we did the best. You don't want to do the worst. If you got to pick a place to be after the test run you want to pick first. And the second one it was like way down the roller coaster like oh man we're going to get yelled at so hard, this is going to be awful. And then we figured out it was a bug. We're like oh cool we can fix this. And then we ran it and then performed much better in our own run of exhibition round two. 

So I mean yeah we had our fair share of broke stuff that's for sure. But generally speaking it doesn't sound like you regret those decisions. No, I mean when it came to - I mean I think you could have certainly for the semi-finals and certainly through the first exhibition round you could afford to keep things pretty small scale and not really write with any scalability in mind. But the second you got to exhibition round two, three in the final scored round, if you didn't have anything built in for scalability. You were going to spend the last two months of the competition instead of trying to improve your score, you were going to spend it fixing scalability issues. 

So, we built this thing to scale in the first place. Which meant it took longer for us to get to a place where we had something runnable and testable. So we were like I said, for the last two months of the competition, we were doing a lot of these full scale runs. It's because we had a lot of our credit saved up. We didn't really spend a lot January through March. But once we hit April, we were spending a lot, but it was also because we were testing at scale almost immediately.

**Yan:** You might be the first team we've talked to that has no qualms about the plumbing of their CRS.

**Michael:** I mean yeah. Our issue log that thankfully got stuck - you don't have to look at or think about anymore - that thing was full of a bunch of stuff that we didn't like or that we wish we could have fixed. But yeah, for the most part I mean we had to test it a lot and we had to fix a lot of issues with it. But for the most part, we really didn't have issues with dealing with scalability, but like I said, we also like every question when we made our diagram for Buttercup version 2.0, it was like is this going to scale? 

And that's part of the reason why we were really constrained with our resource usage. We didn't know what the final round, what the budgets were going to be. I mean, the budgets in the semi-finals were astronomically small. I got $100 in LLM credits and like $500 in compute. You only had to run for four hours. So, I mean, it's probably commensurate with that, but we had no idea going into the finals like is it going to be more of that or is it going to be what it actually turned out to be, which is six figure budgets, five figure budgets. 

So, we knew from the beginning that if we're going to have to run this a lot, we need to use very few resources per vulnerability. We might have to process a lot of targets. So we can't - we need to be able to rely on replication to scale and not just throwing hardware at it because the processes are only so fast. They've been killed by diminishing returns and you can only - you have to parallelize if you want to scale.

## System Name Origin

**Adam:** Wow. Okay. Cool. Great. So maybe then we can dig a little deeper into the CRS. So can you walk us through what are the steps that happens with the orchestrator and all the components when a new repo arrives in buttercup? Wait, first sorry before that - what does buttercup stand for? Is it just a name or is it an acronym?

**Michael:** I've been asked this five times and I promise you I wish there was a good story for why we named it Buttercup. We actually - it was just made up.

**Adam:** Human made up or AI made up?

**Michael:** No, human made up. So here's the best I can give you for a story as to how the buttercup name came around. When I along with Ian Smith, who's no longer with us - I say that at Trail of Bits, he's not dead, but he's dead to us because he went to a competitor.

**Adam:** I was like, "Wow, this is getting really dark."

**Michael:** No, no, he's not dead, but he's dead to us because he left the company and went to a competitor. But he and I we wrote the original concept for the original concept white paper. And back then, my kids were really into the movie Wall-E, so I named it Patchy. So, if you look back at our original concept white paper, if it ever gets published or whatever, it says the name of our CRS is Patchy. 

But as time went on, it wasn't terribly marketable as a name. And we also wanted to avoid names that anthropomorphized the AI because that was becoming one of these ethical questions in the AI community is like should we give these things human names because it makes them - it sets a weird set of expectations. Move away from that. So we talked about it internally to the company and our CEO Dan I think came up with the name or was the one to suggest it. 

And I mean it helped me when it came to titling some blog posts and some talks I could use the "buckle up buttercup" idiom but beyond that it didn't really come from anywhere. We just wanted something that was simple, easy to remember, wasn't an explicitly human thing. I wish I could say we were all big fans of the Princess Bride - we are - but that had nothing to do with naming it Buttercup.

**Adam:** It's like a good horse. Like maybe a CRS and a horse is a good metaphor. Like it's intelligent, but it's maybe not as intelligent as a human. It can run faster than a human.

**Michael:** Yeah. Honestly, I was just thrilled that we didn't follow the other well-roded tech naming schemes like calling it Trail of Bits Plus or Patchify or something like that. So yeah, I was pretty happy with the name. It is pretty easy to remember.

## System Workflow

**Adam:** No, it's great. I really like it. Cool. Okay, so then back to Buttercup's details. So what are the steps that happen when a new repo arrives at Buttercup?

**Michael:** Yeah, I mean I imagine this will probably be pretty similar to our other competitors. Mainly just because it's how the competition is structured, but when the competition infrastructure sends us a task, the orchestrator is the endpoint that receives it. It's where the API is implemented that lives. So, we pull down the competition repository. We build it and then basically we start fuzzing it. 

So we build it with a couple of different sanitizers, all the ones that were basically in scope for the competition for libFuzzer and then also for Jazzer. So we build different versions of it. Each equipped with the sanitizers. And then we start fuzzing it in parallel. Our LLM driven CWE generation process is also running. It's adding to the corpus new inputs that will, like I said before, either help it explore and get better code coverage for the code reachable from the particular harness that that fuzzer is responsible for fuzzing. 

And it also generates inputs that are likely to trigger certain classes of vulnerabilities that mutational fuzzing isn't necessarily great at generating. So, think of these as grammar-based type vulnerabilities. Like a good example is SQL injection. It's very rare that a mutational fuzzer, given just a random seed of a clump of bytes is going to stumble upon what is mostly valid SQL with a correct terminating character and then the correct grammar to start some other query that's malicious. So, we asked the large language model to help us generate inputs that were likely to trigger SQL injection, path traversal, other types of specific vulnerabilities.

**Adam:** And is that given the target? So, what are you giving to the LLMs to make that? And is the LLM just spitting out a seed or is it spitting out Python code that generates a seed?

**Michael:** It's the latter. It's Python code that generates a seed. It's actually quite bad at path reachability and code reachability problems. It just requires a lot of reasoning about the dynamic nature of a program that large language models just - they aren't architected to do and are never going to be good at. But they can generate code. So we asked it to generate small Python programs we can run in a sandbox that generate these inputs. And it was surprisingly good at doing that. This one area I was - my expectations were exceeded by a lot in terms of how effective that strategy was. 

So yeah the CWE gen bots, they are busy generating seed inputs to help the fuzzers be more effective. We do this for two reasons. One, we tried to convince the people who ran AIxCC to extend the processing windows because one of the qualms we had with the semi-finals is that if you want a POV you pretty much have to fuzz some way shape or form. You might not call it fuzzing but really what you're doing is fuzzing.

**Adam:** Can you elaborate on that? Like what might you be not calling?

**Michael:** So let's say I get rid of all the mutational fuzzing piece and I say LLM generate inputs that are going to trigger a vulnerability. For it to be a POV and for you to be reasonably assured that you should submit it, you have to validate it which means you have to run it. So really what you've done is you've replaced the mutational fuzzing engine with a large language model that generates the inputs. So you've made a less efficient fuzzer. So no matter what because you have to - because you need a POV and because you have to validate it before you submit it, you are doing fuzzing. There's just no way around it. 

So, that's my philosophical stance. I'm sure someone out there would love to debate me on it.

**Adam:** It's interesting. Yeah, I like that there's even this bit of randomness involved as the temperature or whatnot, like there it is essentially a custom mutation engine.

**Michael:** I mean, it really is. Yeah. So, I guess getting back to the original question. So, yeah, the CWE gen bots, they're trying to improve fuzzing and it's for a couple of reasons. One is to find vulnerabilities that are harder to reach, stumble upon by mutational fuzzing. I covered that, but two, it's also to meet the time horizon. We tried to convince them in the semi-finals to give us a lot more time to run these things because anytime you talk about doing something with fuzzing, you're usually talking on the amount of time you're allowing the fuzzer to run on a given harness usually in orders of days. 24 to 48 hours is what you'll see in the literature and we're talking 0.4 hours and it's like okay I built this system and you're going to rate it against other systems and you're going to tell me I wasn't in the top seven or I was. It's a coin flip game on how good the mutational fuzzing engine happened to stumble upon the vulnerability and it's not really a true measure of the system. 

So in some of the earlier exhibition rounds they had longer windows but I think that pushed them back down. So in order to meet the time horizons for doing this we had to fuzz or we needed to get higher coverage on the fuzzing harnesses faster. So that's why we also include a portion of our CWE generation which Ronald Chen was the member of our team that was in charge and owned that tool and did an absolutely spectacular job with it. Yeah, it really helped us find those vulnerabilities within that time frame and then also helped us find vulnerabilities that are harder to stumble upon with mutational fuzzing.

**Adam:** Awesome thing. And so this generated synthesizer seed synthesizer programs but it didn't - it implicitly built in grammars just in by virtue of how it built the program. It didn't like for example shellfish generated grammars and then had all of this combination of grammars and generational fuzzer from there. But you basically had the CRS do or the LLM doing that implicitly in its head and then generating the grammar based generation program basically.

**Michael:** Yeah, we didn't want to constrain the large language model and how it would go about doing that. We really relied on it pulling something out of its training data which is probably some input generator for SQL injection vulnerabilities. So we wanted to keep it as broad as possible because the more information we gave it, the more likely it was to hone in on just one solution. And we're running these CWE generator bots many times with different configurations asking them to focus on different CWEs. So we wanted them to be - and sometimes the same CWE has two or three CWE generator bots for the same challenge. We wanted them to come up with different possible solutions. 

So with the temperature setting on the large language model, it's possible that it hones in on one implementation that it found in its training data from one person who made this tool and then some other person who made a similar tool and another person made a similar tool. All of those would eventually be brought to bear through code synthesis and seed synthesis.

**Adam:** Very cool. All right. So then you get a POV, right? And then what happens after that?

**Michael:** Yeah. So the actual fuzzing part was more interesting in the semi-finals but is very uninteresting in the finals and I suspect this is probably the same with most everybody where people just used OSS Fuzz or ClusterFuzz and the OSS Fuzz infrastructure that was provided. So yeah when we get the POV, our orchestrator gets it back and it starts looking at it and it decides whether or not to submit it. 

There's a little bit of deduplication that goes with this because for the most part the competition really didn't disincentivize you from submitting duplicate POVs. There was no penalty for it and also you might be able to clobber some other teams' patch if you submitted a lot of POVs. But we had an interest in our own system to keep the number of POVs down because it meant there was less time spent patching. 

So we used basically the same infrastructure that the competition organizers were using to deduplicate vulnerabilities. This is based on the stack trace, based on instrumentation traces and we also deduplicated across sanitizers because the same bug will trigger multiple sanitizers. So we deduplicated there. So ultimately we kept the number of vulnerabilities down that were going to process but we were pretty liberal with if something did come out but look similar we were pretty liberal with submitting it. 

So from there the vulnerabilities now go to a patcher. The patcher is supported by our contextualizer. The contextualizer also supports the CWE generation mechanism but it was really conceived to support the patcher. So for that I'm going to hand it over to Evan to talk in detail about some of the stuff that we did there. Evan was the owner for this component throughout the entire competition semi-finals and finals. So we had a couple people on the team not able to continue with us and some that came on new for the finals. Evan has been subjecting himself to this abuse for the entire two years and deserves full credit for this, good or bad, but I'll let him take it from here.

## Contextualization Component

**Adam:** Awesome. And just the contextualizer component is what you worked on or the patching component?

**Evan:** Contextualizer component.

**Adam:** Okay. Very cool. Awesome.

**Evan:** Yeah. So, as Michael said, after you get a POV, what do you do with it? You give it to a patcher. So the idea is that the patcher would take some information from the POV, the stack trace, some artifacts from the crash itself, maybe the byte input, and try to figure out, okay, where in the code does this issue manifest, where's the root cause, and then how do I patch it? 

So in order to get this type of information, we decided to create a contextualization component that could be queried. So the high level overview of the contextualization component is just a query mechanism, a library that an LLM can use as a tool to query various information about the software structure of the program's information. So things like if it finds that in the stack trace it calls a certain function or crosses a certain line in a certain function, it can query the contextualizer and say okay what is the code in that function body, what functions call that function, and what kind of types are in there, what are those type definitions, what else calls that type elsewhere to try to reason about and figure out what the root cause of the crash is, of the discovered vulnerability. 

So initially what we had in the semi-finals competition is we had something that was a bit more fixed. So we tried to prescribe a context. We tried to reason okay well the LLM is going to need the stack trace information. It's going to need the function code, caller/callee to a certain degree, a certain number of parents or grandparents or children or grandchildren of functions, information about data structures and etc. It worked just fine for the semi-finals obviously but we started...

**Adam:** Sorry just as a - so this would just get shoved as part of the context and then you'd have the prompt of like use all this context but then make a patch for this thing.

**Evan:** That's correct. And it's a tall order to ask for an LLM, but we were very measured in how we did this and through lots of testing as Michael had mentioned through the semi-finals. We were like, okay, well, we are getting good enough results that we will perform what we expect to perform well in the semi-finals. Obviously, we did. So, we were pretty confident going from there. But, as Michael said, immediately after we found that we were in the top seven in the semi-finals, we went back and regrouped and said, "Okay, what if this scales? What if we get a bunch more money? What if we get orders of magnitude more repos, more complex code? We have to prepare for the finals." 

So, we went back and figured out, well, giving an LLM everything is not, or at least to the degree that I was doing, maybe not the best decision. Maybe like the LLM guide itself. So, this is kind of a precursor. You can make an illustration to what MCPs are nowadays. Kind of a big thing.

**Adam:** Waiting for the more details to get there.

**Evan:** Yeah. Yeah. Of course. So MCP - so to be clear we are not using MCP in our CRS but this is kind of a precursor to that. So basically you can think of this as a tool that the LLM can attach to and use. So in the prompt we'll say here's the stack trace and give it the information that we have from the POV and then we say hey you have these tools available to you. You can query for functions. You can query for certain lines of the code. You can query for specific data structures and what is involved in those data structures and where those are used and you get these tools to the LLM and the LLM goes through this discovery process and it's less of a prompt to give to the LLM. So the LLM can be more targeted towards where it thinks it should go and discover as opposed to trying just to shove the entire Linux kernel all in there and say hey go figure out where the bugs are and patch them. 

So, again, it's a bit more of a judicious use of the LLMs and as Michael was saying, this obviously gets us to the point where we're not overly using the LLMs, but using the LLMs where appropriate. And again, in all of our testing, we were still seeing the same efficacy through the semi-finals challenges, but once we started running it on the newer challenges, we were seeing a better, more effective solution through this. 

So yeah, so back behind where the program model or the contextualizer exists is just static analysis tools running. So the static analysis tools running are going to be the ones that actually are performing the program analysis. It'll figure out where the callers, callees, etc., etc. are and then that's just provided as a function call to the patcher and the CWE generator.

**Adam:** And you're talking about stuff like clang indexer, code-these guys.

**Evan:** Yeah, something like that. Yes. So we were using code query, tree sitter etc those types of things. We tried to use - so the dream was to use something graph-based and was working, it was working well until Java came up and then Java didn't work really well for some of the things we were trying to - I was trying to use graph and all this stuff and it just didn't - it just didn't work out for the program analysis tools that we were trying to use so we ditched it and we went back to the just your general static based code analysis as opposed to...

**Adam:** It sounds like you chose the tooling specifically so that it would work on both C and Java.

**Evan:** That's correct. Yes components. That's correct. Yeah. Because we wanted - because as Michael said we underperformed on the Java side. So we wanted to make sure we're on a level playing field each way. So, when we were doing our tests, we made sure that obviously we were still doing well in all the semi-final challenges and the exemplar challenges we were being given for the finals, but we always had Java in our mind as equally weighted on C challenge because we just didn't really know what the percentage of those challenges were going to be. 

And honestly, we just wanted to make everything under the same umbrella, not get too specialized unless it was warranted. We wanted to make design decisions carefully and with evidence. So I did a lot of testing before the first exemplar to make sure that the design decisions that I was making actually did have an effect and were still effective enough to help the patcher and the CWE generator out to patch and find vulnerabilities or generate.

**Adam:** Yes, this is super cool. So I think one of the things that - sorry Yan - that you said very specifically this is not MCP but is that just because you built this system and started it before that was clear that that was becoming the standard.

**Evan:** That's correct. MCP I'm not going to advertise myself as an expert on the genesis of MCP but I'll say it wasn't readily available when we started it. So, to be specific, I'm not using the protocol at all. That's what I mean when I say MCP. I'm using the concept of it, but I am not using it itself.

**Adam:** That's a very clear like agentic style that you're allowing the LLM to use tools, which is essentially what MCP is supposed to, as I understand it, supposed to allow you to do. But yeah, I think what to me what's very interesting there is it just shows how quickly this field is evolving, right? When you started this even - I mean way before semis I don't think people were starting to talk about agentic AIs like before semis but it was just like now it's a big thing but you had to build this stuff over the last year, two years.

**Evan:** Yeah it was super vindicating doing this project for two years because everything that we put into the semis became commonplace by the time we got to the end of the semi-finals and then some of the stuff we're doing now is starting to really come about. So, for example, our patcher has always been a strong suit. I'll get to the design of the patcher here later, but a lot of what we put into the patcher has later become what was baked under the hood for OpenAI and Anthropic's reasoning models. This mixture of experts, this degree of prompting, separation of concerns, we did all that before it was cool. 

And then our first patcher was basically a multi-agent system. It now is like even more complex multi-agent system. We did that before it was cool. So all the stuff that you can do now in Langchain easily with stuff that we had to bastardize and wedge in. And yeah like the way we structured our prompt and the use of tools, a lot of that stuff that has become now commonplace for getting the best out of large language models I feel like we did all of it a year earlier than everybody else.

**Adam:** So even just the concept, sorry Yan, just real quick, even just the concept of contextualizer, like there's a push I'm seeing among AI people that we should not be thinking about prompt engineering, but context engineering. Like the important thing is what context you give the LLM, whether it's through tools or stuff that you pre-populate. And so that in itself, I think, is a very forward-looking thing. But go ahead, Yan.

**Yan:** I was wondering so - so it's very forward-looking but now as you said the field has evolved now there is the reasoning models and so on. Did you go back and adapt your multi-agent or your multi-step separation of concerns chain of thought stuff to just use o3 and be more straightforward or streamlined or whatever you might - not as good maybe - or did you stick with what you had?

**Michael:** Actually no. We actually stuck with models that were non-reasoning models. We eventually added them in I think as backups or fallback models and that was because through the semis and through the finals we built a lot of tuned to the problem of vulnerability discovery and patching. We built all of this problem breakdown, all of this chain of reasoning, chain of thought, step-by-step, multi-agent processes, all the stuff that we built. 

So OpenAI and Anthropic they've tried to generalize this and bake this into the model by essentially whatever query you provide to o3, there's a prior model that says here's what they've asked for, how are you going to break it down, how are you going to do it step by step and then figuring out which fine-tuned model under the hood, which expert model should handle this particular request or that particular request. So thinking this from a computer science perspective, best case scenario the o3 model is going to perfectly replicate what we've already done because we are experts trying to solve an unsolvable problem. No one's doing it. At worst case scenario there are six people doing it better or six teams doing it better than us. Worst case we're dead last in AICC but nobody else is really doing this. 

For we actually still use GPT I think 4.5 - we went with the later versions of the models but we went with the non-reasoning versions because they kept cost down.

**Adam:** Because four point five is expensive but because you are careful about your usage you can actually afford it. I think we've talked to a lot of teams that say yeah for this we use GPT 3.5 or something right because it's - we need it to be dirt cheap because we query so much.

**Michael:** Yeah. That's interesting because you're the 16th team we're talking to now. We have a lot of this context. Exactly. So for example, Theory - we were talking about a similar thing with Theory and they initially wrote their careful prompting strategy and if I remember correctly I think it was Theory they threw it out faced with the same decision. Which is an interesting...

**Adam:** I liked your reasoning about keeping - also two teams that said that they had some complicated patching where they broke like they had used two different models to do the patch and then verify the patch and then when the thinking models came out they reran their initial test and was like wait this can just do it without us doing this other part.

**Michael:** So, this is going to sound catty, but I say this mainly so I can pump up a member of my team. Ricardo Chirino was a member of our team who was responsible for the patch the entire way through and he's an incredibly diligent engineer. So, it was very easy for us to keep all of his patching components because they were well written and pretty reliable. 

So in other cases, especially when you have to put it together before the industry is ready to support it with standardized libraries and like it become like MCP and multi-agent are a thing. It's easy for that stuff to get complicated and become an albatross. In our case, it wasn't because we had an incredibly talented engineer who really owned that and honestly, it's probably one of the strongest points of Buttercup is how well the patcher performs. 

I think if you actually look at the semi-finals, every vulnerability we found, we also patched. We didn't have anything that we left points on the table after a vulnerability discovery. We had issues in finding vulnerabilities in the Java side, but had we found them, I'm confident we would have patched them. And going forward, I can say this now, going forward, part of this is just depending on when you find the vulnerabilities, and some of the vulnerabilities are more complex now. Going even now in the exhibition rounds, it's pretty routine for us to patch 80 to 90% of the vulnerabilities we find. So we are very strong on the patching side. 

So like I said, this is not to be and tell everybody else they make spaghetti code and it's all crap. I'm really just trying to say this is my way of saying thanks to Ricardo for making me look good for two straight years.

**Adam:** Well maybe we can then use that to transition into. So we have the contextualizer that the patching component can use. So then how does the patching component work? I mean we've basically been addressing it but let's do it head-on.

## Patching System

**Michael:** Yeah. So our patching system is probably the most complex part of the system. And this is largely because we didn't - least amount of compute, right? Because you said the fuzzing nodes used a ton of compute whereas patching was way less, right? Which I think is also super interesting to think about that this part is very complex. Fuzzers are actually kind of simple, right? Once you know you're not writing the code for that, using libraries. So anyways, yeah, please go ahead.

Yeah. Yeah, sure. So the yeah, like I said, the patcher is super complex and it's really cutting edge. So right as the semis were kicking off and we finally got an idea for what the CRS was actually going to have to do. This was when the first papers were hitting not even the actual literature like hitting archive talking about how to separate concerns and how to do these multi-agent systems. 

So I've been doing applied AI/ML for solving security problems for a long time back before LLM became the predominant form of technology and as we saw LLMs come out two years ago they were really trash at solving a lot of these problems mainly because these problems are trained on these huge generalized problems. So this was something that Ricardo and I when we discussed early on, we need to actually focus this problem down. 

The prevailing mindset at the time was just throw all the code in there. This new model X has a context window that's five times larger. So now you can fit all the code in, right? But that was presupposing that more context meant better results. And if you actually think about how large language models work, the more context you put in, the more you null down to the denominator. I call it the null weights of your token probabilities. So you're actually better off and our experience has borne this out with very highly contextualized, highly narrow requests to large language models. 

So this was a design decision that was based in from the very beginning. So our very first patcher had three distinct agents. One was a leader agent which was very thin. It basically just handled the work of the other two. It doesn't even use a large language model to do it. It's just code but it counts as an agent because it's in the agents folder of our source code. 

The other two agents are a quality assurance agent and a software engineering agent. So the software engineering agent gets the task of hey you broke this code or this code's broken, it's got this vulnerability, go fix it. So it tries to fix it. Then the quality assurance agent was actually tool enabled. This is long before tools became part of MCP and or just tool use in general around it would actually - we treated the competition infrastructure and the actual repository as tools. So the quality assurance agent would be tasked with, hey, you need to go run the test and make sure that the tests come back clean. You need to compile this and build this. You need to make sure that it builds. 

So it actually had built into the prompting and built into some of the automation this validation step that made sure that when we submitted things, we never submitted anything that was wrong because I mean it is possible to validate every POV and every patch that you submit. So, in our finals version of the CRS, we added a couple of other agents that do some small things, but for the most part, it's pretty much the same. Like, we have a persona that is a software engineer that is tasked with fixing the code, not just you're a general LLM or you're a security expert. 

It turns out if you ask software - the terminology for software engineering is much more associated with coming up with corrections than vulnerability researcher which actually - the more I think about it, most of the vulnerability researchers and software engineers I know, I actually probably would trust the software engineer to fix the code more. We're good at finding the bugs and pointing out everyone else's mistakes but thank god we don't actually have to write our own code at scale or that level. So we'd probably be shown to be just as bad as your anecdotal experience.

**Adam:** Did you run ablation experiments? This is super fascinating to me because people blob you're a cyber security expert and they don't really think about it.

**Michael:** It's anecdotal. We've done some work for the UK government on evaluating models for their ability to do certain tasks. And I think early on we said you're a cyber security expert and then we asked it to do things like find vulnerabilities and we didn't get great results. But then we found through just prompt engineering that separating a quality assurance engineer that was responsible for looking at the quality of the code and then a software engineer that actually was responsible for generating the patches like calling it a software engineer was better. 

So yeah, we had a couple of other agents that did other smaller tasks. We had one agent that was responsible for reflecting on a patch. Some of these smaller agents were created to fine-tune towards the end of our final submission. For the large part, we really only needed a three agent system with access to lots of tools. And when I say lots of tools, I don't mean custom stuff. I mean, just the ability for it to on its own run the test because otherwise you have to rely on these really complicated automation loops where you're relying on this thing to recognize that it gives you something. You have to test it. Okay, it's trash. Now you have to figure out what to provide it back. 

A lot of this infrastructure exists now and is actually easier to run and maintain a coherent context window when it's run as a tool versus being run completely separately and you're using manual Python code to pipe information around.

**Adam:** Awesome. Okay. So then that verified patch and probably POV and all that information goes back into the orchestrator. So then how does it know what things to submit and when?

**Michael:** Yeah. So this is where the gamesmanship comes in. So the patcher when it finds good patches it sends them up. And the orchestrator keeps track of the various patches that we have. We don't really wait on submitting patches. We submit them as fast as we can because of the time component and scoring. But then the presence of patches then informs future iterations of the CRS. 

So for example, if we have two POVs that don't show up as duplicates or don't register as duplicates based on our deduplication scripts that we largely source from the competition organizers, we actually test that POV to see if it's fixed by patches we already made. And if it is fixed, then we register as a duplicate that way. So we avoid processing it and potentially submitting a duplicate patch, which does actually cost you points in the form of accuracy. The competition organizers nerfed the accuracy multiplier with the last round, but still, we recognize that it could be a significant scoring detriment. 

So our scoring strategy was basically don't lose the points that we get and do a good job of getting points and then we probably do okay.

**Adam:** It's pretty interesting like when you think about it there's because you talked about the stochastic nature of fuzzing, right? So there's the key components I think in the scoring where this affects things is the speed at which you find things. So you're rewarded the faster you find things which went into your patching strategy like submit the patch as early as possible to get that speed bonus. And then there's the accuracy multiplier. So assuming - I think actually talking to the teams there's enough diversity in the systems themselves I think there will be pretty disjoint sets of POVs and patches found but among similar systems that are finding the same bugs those differences of speed and accuracy multipliers will probably be the differentiators right?

**Michael:** Yeah that's part of the reason why we do POV and patch cross comparison because We also test to see if a POV that we found that is registered as a duplicate. We test to see if it breaks a patch we already made. And if it does, we know we're not going to score anything with that patch. So at that point, it's now more advantageous for us to submit a new patch, which we get dinged on the accuracy multiplier, but we actually collect points and the patch is worth more than anything else in the system. 

So if we get to a situation where we know a priori that we found a vulnerability, we can be sneaky and not submit it and then not blow our own patch. But we figured with six other teams out there, someone's going to find this POV because we found it with fuzzing. It's not like we did anything super special. Everyone's using OSS Fuzz. So someone else is going to find it. So that then we have to go back to the drawing board, repatch, but now we're patching against multiple POVs instead of a single one.

**Adam:** And does the patcher use those additional POVs? If it's generating a patch and it knows the POVs are related, it will then use that. Does use that as part of context or just checking that the generated patch actually fixes all of those POVs?

**Michael:** It's both. So the patcher gets access to the different POVs and then also it goes into the quality assurance routine for making sure that all the vulnerabilities are patched before we submit before we go again. So, we never actually end up submitting that other offending POV. Actually, no, we do submit the offending POV. If we find one that clobbers our own patch, we submit it because we hope we're going to clobber somebody else's, too. So, we're kind of mean in that way. We chose to take everybody else down with us. If we're going to lose our accuracy multiplier, then we're going to be jerks about it.

**Adam:** No, it makes sense. Yeah, that's I think we did we go the other way, Yan, and hope that somebody else would submit that. I think there was one case where we if we knew we had a POV like a bypass for a patch that we were never able to fix that POV. I can't remember. Our strategy was very complex. I can look it up in our docs, but it's probably not too complicated. Who knows what the system did. Hopefully, it did what it was supposed to do.

**Michael:** It is super complicated. I described this functionality like it was always part of it. This was stuff that made it in a week before the competition was going. So we were scrambling and honestly most of the work we did in June after the third exhibition was focused on just adjusting to the changes in scoring that were published by DARPA. So that was the vast majority of what we changed in June. By the time we got to the end of the third exhibition round, we were basically pencils down on the actual core functions of the CRS, which was kind of interesting. It was a very different flavor work that last two or three weeks that we had before the final.

## Secret Sauce and Philosophy

**Adam:** Very cool. All right. Awesome. So, yeah. What would you consider to be your buttercup secret sauce?

**Michael:** Yeah. So the secret sauce I would say - I've said this quite a few times in various places but we started this off with we always had a best of both worlds approach. I personally had worked in applied AI for a while before this, had no delusions. I've seen firsthand how hard it is to make a machine learning model even remotely be good at vulnerability detection. I did it on a prior DARPA program and Evan and I like this - one of the papers that we published together while we were both at Georgia Tech. 

So we knew going into this that AI, machine learning, whatever you want to call it, it was going to be really bad at certain things. Then we also have been - my background is actually in compilers and Evan's is in malware analysis. We both have do a ton of work in conventional software analysis. So we know exactly where the halting problem is and how it wins every day. It wins every time. So we knew that program analysis was going to suck at certain things. So particularly on real world stuff, right? I think that's the other - not on toy small problems. This on real world software that is crazy.

**Adam:** Yeah, patching is that spot like there's all kinds of program synthesis approaches and all this stuff that people made to try and tackle software patches. They are all terrible when it comes to fully scaled programs. I'm not crapping on anyone's work. You got to solve Linux core utils before you solve Apache Tikica or before you solve the Linux kernel. But yeah there's a scalability problem there and that's one of the areas where AI was a good place. 

Yeah, really when I sat down to write our original concept white paper, like I said, I did this with the other person who wrote this with me, Ian Smith, we sat down and we said, "What tasks are you going to need to perform and what is good at each of these and what is good at each of these for certain types of problems?" So, if you look at our original concept white paper, it really wasn't a pipeline. It was more like a giant matrix where something would go in, we'd characterize it, we'd choose the right tool, we'd push it to the next stage, choose the right tool based on what tool we used previously. It ended up getting consolidated down to a single pipeline. Because we got a lot of constraints that were solved by the competition infrastructure. 

When we set this down, we said, okay, what is good - what does software analysis already do? Well, fuzzing is a good example. If you need to find a POV, people have been researching fuzzers since the 80s. I think it was when the first paper came out. There's a little bit of a gap between before it got serious, but it's almost like a right of passage getting a PhD. You have to write one fuzzer. You do not get a PhD in computer science or security without writing at least one fuzzer at some point somewhere. So people love to write fuzzers. There's a million of them and they're really really good at finding vulnerabilities. 

So, we didn't look at how are we going to make the LLM do this better or how is the LLM going to or how is AI even more generally before we knew that we were going to be mostly limited to using large language models. At least for the semis, we were looking at how we're going to try and like make AI do something it's bad at. And similarly, we weren't - we didn't have any - basically we went into this with no delusions about the capabilities of either set of tools, whether they are AI or whether they are conventional. and we chose to mix and match them basically where they go. 

I don't know, I use this analogy that I'll share here that I usually use is to try to explain to junior researchers when to use each. When we talk about conventional software analysis it is a prescriptive solution. You are prescribing a series of steps to the computer to go solve your problem. It works well when you know what to do and things flow from one step to the other. It's like any program. AI/ML is a descriptive solution. You're giving it lots of examples and you're saying I'm describing how the solution looks for a particular problem and I'm asking the model to infer what the solution will look like based on the descriptions I've given it. 

Certain problems are prescriptive. Certain problems are descriptive. And your ability to solve them should govern when you're going to use AI, when you're going to use conventional stuff. And we use that. We stuck to our guns on that. The AI hype machine went insane. Our company's embraced AI. We use it probably more than anybody else, but we have always stuck to our guns on we're not going to use it in a place where we're going to go off and go on some wild goose chase. We're going to waste a bunch of time. 

Just like when we try to solve computer science problems, every computer scientist that has a graduate degree knows how to reduce a problem to figure out if it's traveling salesman or the halting problem. Traveling salesman means NP complete. Okay, I can probably solve this, but it's going to suck doing it the whole time. And if it's halting, stay away. You're going to waste a year of your life doing this. AI/ML is kind of the same way. So it really comes down to problem formulation. We've stuck to that. That's the secret sauce of buttercup is we did a lot of just exhaustive problem formulation on what is the right tool to use for this particular job when the constraints are fully automated, you can't touch it.

**Adam:** So this is great. So then how - so during the competition right then how did your outlook change on AI like by participating in and as the models change. So looking back, did it kind of - the problems that you looked at where you're like, "Wow, the AI, you used to be bad at this, but now actually is good at it or better than I thought."

**Michael:** So the answer to this is that I am currently sitting in a bubble full of a tremendous amount of confirmation bias and that I went into this knowing what problems the AI was going to be good at. And I only used them or we only used them there and in both cases both for patching and for CWE seed input creation. My expectations were exceeded in both. Both of them really surprised me like okay these are actually doing a lot better. I was really pessimistic about it going in but they both performed much better than I thought they would. 

But the reason why I say I'm in this bubble of confirmation bias is it's entirely possible we go to this competition, we get absolutely smoked by somebody who used AI for a purpose that we thought was poorly fitted for it and it turns out it wasn't. So the element of surprise is potentially there to bite us in the ass. So, for now it looks great. In hindsight, I wouldn't have changed anything because the stuff I decided to use it for worked out great. But I also don't know if I missed anything out there where it's a really killer application of AI that I missed due to lack of imagination. But at the very least, we didn't go down any rabbit holes. We didn't waste a lot of time trying to make AI do something that it really wasn't suited for. Evan, what do you think? Do you have a different answer to this or what are your thoughts? I've been talking for a long time.

**Evan:** No, I'll pair what you said. But I think that yeah, I think again the - I think one of the best compliments we received in the ASC at the end of the semi-finals was that we had the most judicious use of LLMs. And I think I'm pretty proud of that. So no, I will just pair whatever Michael just said and I'll say I have we have seen a noticeable improvement in the different models abilities to patch. There were three different models we were using in sort of a round-robin type manner or some sort of - in the semi-finals in case one didn't do as well we switched to a different model and there's kind of like a convergence. Earlier this year there's a lot of new major models I mean obviously OpenAI GPT-4.1 came out and Anthropic had Claude 4 come out and so there's been some very noticeable changes and I think again because of our focused use of LLMs I think we did notice a difference at least from our own testing and infrastructure.

**Adam:** Were you very pro-AI at the beginning and now you're even more so or were you skeptical at the start starting this new job and being like wow I have to make these AIs work?

**Evan:** No. No. I mean so I'll again I have the same attitude Michael has. So in my research back when I was in grad school was ML applied to cyber security so specifically for malware analysis and malware detection. So I mean semester one I mean paper one the halting problem is ground into your head and understanding what these things can and cannot do. No I think I had and I still have the same attitude towards it. I think it's a useful tool. I think it has a place. But I think again it's a application needs to be measured. I think it needs to be - I think we need to be diligent with how we're using it and not just yoloing. Just give every get everything and hope everything works out. I don't like rolling the dice that much. But obviously there is a place for it. So no I don't think my attitude has really changed on AI since this competition. But it is interesting. It's been fun to see how well it has done and how it's performed to patch various software bugs we found.

**Adam:** Yeah, that's great. Yeah, I think that'll be that's one of the interesting things that are coming out of these interviews that we're doing. For instance, it was Theory, right, Yan that is actually submitting patches to which they don't have a POV for. So they found their confidence in the LLM's assessment of bugginess.

**Yan:** Yeah. So that'll be I mean just like you said Michael I think it'll be super interesting seeing the results how that shakes out how the different approaches to the problem will manifest.

**Michael:** Yeah it's I really appreciate that confidence of the depth of understanding of the approach. That's a very unique secret sauce. And it's also cool that, looking back, it sounds like you have no major regrets, major changes you'd make.

I mean, I might have some regrets on August 9th. Well, the good news is I'm going to be-

**Adam:** That's why I'm asking you now before you know the results.

**Michael:** Exactly. Yeah. You know, twice the pride, twice the fall, right? The good news is, we're going to be in Vegas to hear the results come out. So if we are indeed disappointed, we are in the perfect city to handle sorrow and deep existential regret. But no, yeah, I don't think we do anything differently. 

Admittedly our approach is conservative. We focus on doing a really good job at scoring points and doing a really good job at not losing them. So when it comes to SARIFs, this is a good example of this. We actually didn't do a whole lot with SARIF broadcasts because they're not worth very many points on their own and you only get points for bundling them if you also found a POV and/or a patch and you really only get the huge reward if you found both. 

So we actually wait to handle SARIF broadcasts until we've already patched a vulnerability and it's only if we see overlap between the reported code region and the SARIF with either the localized vulnerability or the region that we patched in code. That's the only time we actually handle those or bundle those. So, it's stark contrast to yeah, we don't submit any patches without a POV because the potential for your accuracy multiplier to get damaged there. And then also, if you bundle those well, I guess if you don't have a POV, they probably wouldn't bundle it. But yeah, the accuracy multiplier, I guess that being nerfed, it makes strategies like that possible to go out there on a lark and hope that the LLM is properly assessed everything or properly patched a vulnerability that you can't trigger. 

But yeah, we took a pretty conservative approach and that's mainly because I really wouldn't call it conservative. We're really aggressive with how we go out and find vulnerabilities. We're trying to use our resources to the absolute maximum. We did a lot of work actually just doing engineering tuning on how many replicas of each type can we get to spend almost the full $80,000 in the final and spend all the LLMs. Yeah I think our other secret sauce is probably engineering. We had really good talented engineers. So I think we probably worried the least among everybody about uptime, reliability, that kind of stuff. We tested for it pretty extensively.

**Adam:** From what I'm hearing, it makes sense your whole - I think maybe if I had to term a philosophy or something, it's around engineering focused, right? So, you started out at the beginning planning the system based on which components and which techniques you thought were best. You engineered the system, had it so that you had CI running like it was a well-tested system that did like all the components should have been doing what they were doing. And conservative - I don't - I guess with the use of LLMs and stuff like I see that as we're not going to invest time in crazy researchy stuff that may or may not pan out and may balloon our LLM usage or something but we don't quite know if it's actually going to help us win. Let's focus on solidifying the core is what I took away from it.

**Michael:** Yeah, I think that's a really fair description.

## Final Thoughts and Results Prediction

**Adam:** So then the $4 million question, where's all of this going to go? What place do you think you're getting?

**Michael:** You know, I think we're in the 51st percentiles, somewhere between one and four. I think we'd probably be pretty surprised if we ended up in the bottom half. A lot of this is just based on prior performance. We did really well in the semis. We found a lot of bugs first. We patched a lot of bugs first. We had some obvious issues with finding Java. The Linux kernel was a disaster. I'm not even counting that as a CPS. I kind of black out when I think that it was even involved in the first place, but fortunately it didn't show back up. 

But yeah, when it came to the Java examples, we had some engineering issues that prevented us. So maybe that was why we were hyperfocused on engineering in the second half to make sure we didn't leave stuff on the table. But yeah.

**Adam:** Were there any - I think you mentioned it before with the file names. Were there any other close call bugs that made it into the system that your testing caught and that you're now very happy that you found it and-

**Michael:** Yeah, that was the worst one that made it in that actually went to a round that we didn't find in advance. The file name one. Yeah. And that one was had a lot to do with just needing to see new examples. We needed a stack trace that was long enough that when you compute it into a file name that it exceeds the length. So yeah, we had a couple of other close calls here or there with stuff that we had to patch a day before we went in, but we were really good about being pencils down several days at least on the branch that we were going to submit. Pencils down a couple days before. 

So our typical approach to a deadline for an exhibition round was, the deadlines were usually on Wednesday or Thursday. We would be pencil down on Friday. We'd run a full-scale test over the weekend. We'd come back. Whatever issues that broke, we would fix on Monday, run another shorter full scale test on Tuesday, Wednesday, fixing only those small bugs that we had high confidence in and then push out. 

But that being said, we have a couple of bugs that - or a couple of Heisen bugs that they are absolutely in there. We over log everything. If you look at our logs, we look like a bunch of sloppy jerks who don't care about software engineering, but a lot of that stuff was just we don't have time to fix everything. We're on a tight deadline, so not everything got fixed. But they're all minor stuff that either doesn't affect the operation of the CRS or absolutely at the worst case after running for seven days it might make a node fail but the Kubernetes will just restart it and you're right back to being good.

**Evan:** I think the other superpower we had to lead up to that because we only experienced one major issue during one of the exhibitions is because each person owned a component of the system and we'd have regular meetings to discuss it. And I think one of the best parts of this is we were always still connected to each other and reviewing each other's code. One of the policies we had on the repository is that you couldn't merge your PR until someone else reviewed it. At least even if it's not their component. And I think what that led to was a lot of accountability and a lot of gut checking and cross-checking from other people that not they're not even in charge of your component. 

So even though I didn't do any work on let's say or a lot of heavy lifting on like let's say the fuzzing or the patching, I was asked to do different pull requests. So I it gave me a lot of opportunity to ask lots of questions and kind of gut check the design decisions and these things. So, I think a lot of having your own ownership and then also getting double checked by your teammates was also what led to us not experiencing that many issues leading up to the exhibition challenges.

**Adam:** Yeah, that's great. It was probably helpful even having eyes on and knowledge of other components. So, if they did hit issues, you have some redundancy built into the software engineering process in some sense. Very cool. Yeah. Any other...

## Favorite AI Models

**Adam:** Yeah, please go ahead. Yeah, the question the audience clamors for. Who's your favorite AI?

**Michael:** We just talked about anthropomorphizing AIs on this episode. I know. That's why I said, "What is your favorite AI?"

Okay, there you go. Man, I mean, I don't know. My favorite AI is whichever one happens to do the best job of solving the particular task because they all seem to be different. I don't know. I'd say generally right now I probably use Claude for more tasks than anything else. Really good at code generation. So I don't know. The great news is we have a super diplomatic answer if you're asking how does our CRS use it? We were split 50/50 between OpenAI and Anthropic. Anthropic is we use that primarily for CWE and it's the fall back for patching and OpenAI is the primary for patching and the fall back for CWE. 

So I think we have officially managed to by sheer luck avoid offending either of the major tech players. Google might be mad at us because we didn't use Gemini, but we did use Gemini 1.5 as a fallback in the semis. So they were helpful there. But yeah, honestly, I'd say I probably use Claude more than anything else. But, I admit I'm probably pretty sparing at AI use to be completely honest. And that's just mainly due to the nature of the work we're in. We're in the business of novelty. We find novel bugs, we find novel patches. Everything we do is new and hasn't been seen before. And that is not something LLMs are good at doing when it comes to the problem domain of cyber security because vulnerabilities, software bugs, they don't exist on this differentiable curve that you can match. They're all these fundamentally different concepts. 

So yeah, for my work I don't use it a ton, but I use Claude probably the most. Evan, what do you got?

**Evan:** I'd probably parrot what you said. I think because I think we're mostly - there's some co-pilots that we use as a part of our company and I think most of the time I'm probably using Claude and then if I just need to riff some thoughts out, I'll probably use - I've been using Gemini. If I need some free form, I have this concept of an idea, I got to flesh this out. I need some non-determinism in my thought process. I'll just throw it to Gemini and see what happens. 

I will say it was fun. I actually had to do - I had to give a talk in a couple months and I just recorded myself talking in just an audio clip of what I wanted to say in my presentation and uploaded that plus the report that I co-authored to I think it was Claude Sonnet and it spit out this - I was like hey I need 10 slides I need them to cover these specific key points and it gave me this cool just boilerplate outline of like hey on this slide talk about these three points because you mentioned this. So, it's kind of a nice thing to get started. I guess it's a good starter for that kind of stuff.

**Michael:** It's the professor trick. It's so hard to write a paper when it's blank. It is so much easier to shape and edit a student's paper that they have written. It's shocking how much that difference is like and there's also experience and all that, but Yan knows because he just very recently wrote co-wrote a first author paper and I don't know what I was thinking.

**Yan:** Yeah. Yeah, for the first time done with that over a decade. No, eight years.

**Adam:** Wow. Well, see you'll get there. I thought that was the whole point of getting a tenure track position is you never have to do that again. That's all your students.

**Yan:** I was thinking flip side of a tenure track position is you have the freedom to make stupid mistakes like writing a first paper.

**Michael:** It's so much work. We ask our students to do this all the time. It's so much work. You forget about it. You only the good memories like yeah we finished it was published. The actual track at 5 a.m. 4:47 a.m. 13 minutes before the deadline. Why did I do this to myself?

**Adam:** On the flip side, that's their full-time job. You also have are doing several things. So, that's right. A little bit of a difference there. I had a meeting today. I'm dead.

**Michael:** Yeah. So, I realize it's backtracking a bit, but I do want to give one AI pro tip for the fellow competitors who probably watch this. When you go to open source your CRS, Claude and Cursor are actually exceptionally good at helping you find all the comments that you don't want people to see and help you delete them. Took about 30 minutes to get through both of our versions of it, but there was definitely some stuff in there that was like, you know, "why the f does this work" or "who wrote this" or stuff like that. So, what you want in there?

**Adam:** I was just going to say I was pushing the team. The team wants to do a nice sanitized open source release and redact the history and I'm like show the people the guts of the sausage. I they want to see all the crazy comments where you're being like "why the f doesn't this work" and "magic hack to get this thing to work." And yeah, I was also pushing for that for CTF challenges, but nobody likes to show the history. They just want to see the finished product.

**Michael:** AICC is too high profile. I don't want to get all the nerd sniping after this.

**Adam:** And that's 100% correct. I think that's totally fair. And I wrote very little to none of the code, so it doesn't affect me at all.

**Yan:** Nice. One of the other benefits of being a tenure track professor, right?

**Adam:** Yes. Yes. We were Yan and I were in advisory roles, helping with helping out when when stuff needed helping out. But cool. Everyone went hands-on, but you know.

**Adam:** Yeah. Exactly. You got to. Yeah. All right. Well, thank you so much for Trail of Bits and specifically Michael and Evan for joining us today. I'm Adam D. You can find me online at Adam Dupe. He's Zardis. You can find him online at zardis. Together, we're CTF radio and you can find us online at CTFradio. You can send us questions through email at ctfradio@gmail.com. And your questions might end up on a future episode of CTF radio. Take care and happy hacking.
