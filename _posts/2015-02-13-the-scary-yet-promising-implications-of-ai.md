---
layout: post
title: The Scary yet Promising Implications of AI
---

This post was inspired by a long, thought provoking [post](http://waitbutwhy.com/2015/01/artificial-intelligence-revolution-1.html) about artificial intelligence (AI) from the very interesting blogging site [WaitButWhy.com](http://waitbutwhy.com/). A big part of my educational enlightenment has been figuring out just what it is that I can do to make an impact in the world, hopefully a good one, on hopefully a large scale. After spending the good part of an afternoon reading and mulling over the Wait But Why article, I had formulated the foggy idea that cognitive computing, machine learning, artificial intelligence, and other related subfields of computer science would provide ample opportunity and potential to make a huge impact by advancing the technology we have today into the superintelligent machines that will most likely be commonplace in the future. Instead of making you read the entire ~23,000 word two-part article, I’ll give you a super condensed version in italics below (note: I have no intention of taking credit for the hard work of the people at waitbutwhy.com – this summary is just a condensation of their really long article).

## A quick summary

> Basically, human progress is currently here:

![Just at the edge of an AI explosion. [Courtesy of waitbutwhy.com]][time]

> Artificial intelligence (AI) technology might be about to skyrocket thanks to the [Law of Accelerating Returns](http://www.kurzweilai.net/the-law-of-accelerating-returns). We don’t exactly know when (or if) it’ll happen, but experts predict it’ll be anywhere from 7 years to 100 years. And if it does reach the point of no return (known as the [singularity](http://en.wikipedia.org/wiki/Technological_singularity) – when AI explosively surpasses human intelligence), it’ll be a fun ride.
> Researchers have also classified AI into three calibers: ANI, AGI, and ASI, standing for Artificial Narrow Intelligence, Artificial General Intelligence, and Artificial Superintelligence. We’re currently at ANI, with things like Siri, Google Translate, or [Watson](http://www.ibm.com/smarterplanet/us/en/ibmwatson/) (the computer that won Jeopardy). AGI is as intelligent as a human, and ASI is anything past AGI, or past the level of human intelligence. Once we build an AI with human capabilities, it’ll likely go through recursive self-improvement (e.g. machine learning) and then become ASI really quickly.
> 
> The problem with ASI being smarter than is us that we wouldn’t know how to control it. It could do unbelievably good things or unbelievably bad things, like figure out how to make us an immortal species (see picture), invent technology for us, and solve all our problems, or it could destroy every living thing on the planet in a ~~plethora~~ [myriad](https://theartifexncsu.wordpress.com/2014/12/07/new-college-writing-paradigm-plethora-gives-way-to-myriad/) of different ways. This immense power is what scares many people (including me).

![The proverbial balance beam. [Courtest of waitbutwhy.com]][beam]

>  The article then goes on to describe a doomsday-type scenario where a robot is given the task of emulating handwriting by constantly improving, without regards to the human consequences of doing so, and the robot proceeds to kill the rest of the universe to gather the resources it needs to keep practicing its handwriting. 
> This doomsday robot isn’t necessarily evil – computers aren’t ‘friendly’ and ‘evil’, we just anthropomorphize them, e.g. think of them as human. Since human values weren’t initially hard coded into the robot, it didn’t consider the survival of humans to be an imperative goal, so it simply continued on to wipe out humans to gather resources for its task.

## So how do we control AI?

AI systems have the potential to drastically alter the current path of life as we know it, whether that path is good, bad, or both. The implications are pretty scary, but the scariest possibility is that we won’t understand how the AI systems we’ve created work, and therefore won’t know how to control them.

Figuring out how to gain control of artificial superintelligence and the self-improving decision making of AI *before* it actually surpasses us could be the difference between us controlling AI and our AI controlling us. And we need to do it fast, because we don’t really know how much longer we have.

In my mind, the key difference between a computer we can and cannot control long-term is whether or not it self-improves. If it self-improves, it could do so unpredictably in a way that creates undesirable behaviors. The intelligent decisions that a computer makes that affects humanity somehow must be moral decisions, in the best interest of human rights. But what’s moral? And how do we govern an AI’s morality?

<hr>

![Issac Asimov, author of Runaround and the Three Laws of Robotics [Courtesy of mentalfloss.com]][asimov]

You may have heard of **Isaac Asimov's** Three Laws of Robotics, originally published in [Runaround](http://en.wikipedia.org/wiki/Runaround), a short story from 1942. They are as follows:

 1. A robot may not injure a human being or, through inaction, allow a human being to come to harm
 2. A robot must obey the orders given it by human beings, except where such orders would conflict with the First Law.
 3. A robot must protect its own existence as long as such protection does not conflict with the First or Second Law.

The problem with these is that they were formed as the basis of a short story, and not from a well-formed scientific approach. They’re too ambiguous, and on top of that, there’s no scientific basis suggesting that they would suffice as valid parameters from which to construct ASI systems.

But is there really any scientific evidence that we can pull from that gives us insight into which ethical paradigms most successfully guide an AGI’s behavior in favor of humanity? **Not really**. We haven’t developed an AGI yet, and the only way to gather evidence about AGI behavior is to make them and study them. Our situation is paradoxical: in order to develop good ethical AGI/ASI laws before they’re developed, we *have* to have AGI to study and experiment on.

Effective technical design paradigms take time and experimentation to properly mature, and sometimes good paradigms haven’t matured until the technology has already undergone widespread mainstream implementation. Andrew Tanenbaum noted this in his [computer networking textbook](http://www.amazon.com/Computer-Networks-Edition-Andrew-Tanenbaum/dp/0132126958). The OSI model was developed, but **before the standards could mature** into a better networking paradigm, technology companies started heavily investing in TCP/IP products and the belatedly-developed OSI protocols were left by the wayside. This is known as the [apocalypse of two elephants](http://students.depaul.edu/~jabsher/apoc_eleph/apoc_eleph.html).

The same could happen with AGI. The rate of progress of AI is so volatile that we don’t know when we’ll achieve ASI, but when we do we should hope that solid fundamentals have been developed to ensure our control of their behavior. Fortunately, there’s been considerable development in the field of [machine ethics](http://en.wikipedia.org/wiki/Machine_ethics), which could provide the answer researchers have been looking for as an assuaging and sufficient response to Asimov’s Three Laws of Robotics.

## The successor to Asimov’s Three Laws

Machine ethics is a relatively new field, only recently coming into focus since the capabilities and sophistication of computers has made artificial intelligence a more realistic endeavor. Basically, it studies the moral behavior of artificially intelligent machines, the potential impact that morality could have on AI behavior, and the creation of '**ethical agents**', a term defined in James Moor’s paper, ["The Nature, Importance and Difficulty of Machine Ethics"](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=1667948).

Machine ethics considers a number of different strategies to control the morality of AI behavior. One such consideration is the domain of algorithms that can be considered safe to use in AI programming: algorithms such as neural networks and genetic algorithms are too indecipherable to be considered safe because of how difficult it is to see how they make decisions. An AI that runs on decision trees or Bayesian networks would be safer, because the implementation of those algorithms are easily inspected and transparent, according to researcher Nick Bostrom (see [this article](http://www.nickbostrom.com/ethics/artificial-intelligence.pdf)).

Another consideration on controlling AI behavior is whether or not we can use machine learning techniques to ‘learn’ morality. Some researchers suggest that AGI should be programmed to dynamically analyze the ethical consequences of its own actions, rather than rely on a predetermined list of rules to follow. It would be harder to implement, but would be more flexible and adaptable to different situations.

## Where are we now?

We ultimately don’t know when (or even if) artificial intelligence will reach a singularity, so there’s no telling what exactly is going to happen. However, the rate of progress of machine ethics and artificial intelligence ethics is definitely nonzero. Products like IBM’s Watson are getting at least within the ballpark of human decision making. Watson can answer impressively complex Jeopardy! questions (as it famously did to beat the two best human Jeopardy! players ever), by combining massive amounts of computing power and massively sophisticated combinations of algorithms in natural language processing and data retrieval to come up with *hypotheses* and their probabilities of correctness.

Watson is an impressive step forward in cognitive computing, and emulates human brain function on a primitive level: instead of *calculating* or *computing* an answer, it **searches** for an answer based on prior ‘experience’ in the form of indexed data. It’s very good at what it was designed to do, but it’s still far away from the general intelligence abilities of the human brain. The jump from ANI (*narrow* intelligence) to AGI is **huge**. It’ll take some pretty giant leap to get there. Still, Watson is a remarkably advanced product that pushed the capabilities of natural language processing and cognitive computing far beyond what had been done before.

In academic research, a great deal of progress is being made. Researchers have begun developing [automated tools](http://dijkstra.cs.virginia.edu/genprog/) (here's [another](http://qiyuhua.github.io/publications/icse2014-qi.pdf)) based on genetic algorithms that can fix bugs. It’ll be fascinating to watch and see what happens as the research continues to push further the extent of human knowledge already made in artificial intelligence and machine learning (and so many more…).

<hr>

Human morality is and always will be a field of deep divides. A quick Google search of [social issues](https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=social%20issues) gives plenty of varying and often extremist opinions. We, as humans, can’t and probably never will agree on the ethicality of certain decisions, and it would certainly be orders of magnitude more difficult to hard code ‘correct’ ethical behavior into an AGI or ASI. Nonetheless, the progress of academic research in both machine ethics and artificial intelligence (and other fields) will ultimately cause advancements in our understanding of the computing systems of the future, and it’ll be fascinating to watch.

[time]: /public/images/time.png
[beam]: /public/images/beam.jpg
[asimov]: /public/images/asimov.png
