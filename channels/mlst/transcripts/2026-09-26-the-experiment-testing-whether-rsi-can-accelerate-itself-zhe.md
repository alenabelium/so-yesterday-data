---
title: "The Experiment Testing Whether RSI Can Accelerate Itself - Zhengyao Jiang"
video_id: yB6_iFGTq9k
date: 2026-09-26
url: https://www.youtube.com/watch?v=yB6_iFGTq9k
channel: Machine Learning Street Talk
duration: "43:43"
source: auto-generated
---

# The Experiment Testing Whether RSI Can Accelerate Itself - Zhengyao Jiang

**[00:00:01]** In my opinion, wireframe engineering is a cheap and effective way to adapt intelligence to a specific task. So, back in July, a new AI company from London posted a very viral tweet on Twitter. It has garnered about 1.8 million views, claiming to demonstrate the first evidence of recursive self-improvement. The problem is that not everyone believed it. I'm Junyao Jiang, co-founder and CEO of Wico AI, where we build self-improving agents. You actually said you spent eight days doing auto research for an auto research agent. We ran autoresearch on the autoresearch framework and were able to discover a better autoresearch framework. Since then, we have continued to fine-tune it over the past two years. Now, when most people think of recursively self-improving intelligence, they imagine a system that can reflash its own brain in a loop . But what if the system only changed the code around this "brain"? Would that count?

**[00:01:06]** I mean, we are interested in the result. So, does this really improve the system's capabilities? Not any specific level. And then, what about the little problem of Goodhart's law, which states that when a measure becomes a goal, it ceases to be a good measure? And, even more interestingly, we found that it develops mechanisms that prevent the reward system from self-destructing. What is the biggest misconception people have about RSI? That if RSI is achieved, a technological singularity or a kind of intellectual explosion will occur. I don't think that will be the case. So, there is a whole community of people creating startups focused on recursively improving superintelligence. This project actually started about a year and a half ago, when we became interested in the concept of recursive self-improvement. Historically, all research has had a diminishing returns effect. However, there is an idea:

**[00:02:17]** what if we allowed the researcher to increase his own efficiency?

**[00:02:26]** Historically, this has been possible through improved methodology and better tools, but human researchers, such as the human brain, are always the main bottleneck . If we

**[00:02:41]** now have an autonomous research system , can we direct the research topic towards itself so that it can increase its research efficiency? And the hope is that one day this efficiency gain will be able to overcome diminishing returns. So that the curve of the ratio of effort and results changes from concave to convex. Of course, this is a big goal, as is the creation of AGI. We all don't know how far we can go, but improving the efficiency of self-referential research is definitely already in our development plan. Let me explain everything properly first, okay? So, Weku created an agent called AID, and it's a research platform, right? And it is very, very simple. You give it a metric, set a task, and it “climbs the hill” to solve that problem. But they set it up recursively, so it actually " went up the hill" until the agent itself improved. And this means improving the platform, i.e.

**[00:03:49]** the prompts, tools, and generally the entire set of capabilities it has. And they just left her to work. We just left it running and saw what would happen. We are observing an interesting thing in the self-improved auto-research platform. We see exactly the code that she generated. It's like code like "spaghetti" from another planet. But for some reason it generalizes very well . Of course, we have a set of benchmarks on which we try to " climb the hill." After that, we test it on delayed benchmarks. These are public benchmarks, such as MLE bench light, ALE bench light; ALE bench is Sakana's algorithmic discovery benchmark. MLE Bench is a machine learning engineering benchmark from OBEYS. We also tested it on a task far outside the distribution called weather bench two. Essentially, you are trying to create a physical forecasting model to predict the weather.

**[00:05:05]** And the weather bench is very different from the training or optimization dataset, but it still generalized well. It

**[00:05:17]** generalized better than our, shall we say, more elegant manual platform. We are somewhat confused by the results of the experiment.

**[00:05:32]** How much do we want to stick with more fundamental, pure solutions, versus a solution that actually works better in practice? I

**[00:05:45]** think there is definitely room for improvement here. For example, adding certain constraints to the optimizer. One option for constraints could be something like regularization of neural networks. How to make him look for the simplest solution to the same problem? That's one direction, but another might be : okay, you just have to accept it. Because one of the factors that makes people think it's " spaghetti code" might be the amount of work done by the agent in the background.

**[00:06:27]** For example, he conducted 100 experiments in our case on self-improvement research, and the number is probably equal to what we have done in the last 2 years. So, if you're bringing a new intern to learn about our codebase, they might also think, "Okay, this is so hard to understand." I think this is partly because you have to endure the cognitive load of understanding the vast amount of experimental results. Do we even need these restrictions? This is a very valid question. I think that in practice such restrictions are still necessary. Humans and artificial intelligence must cooperate. There are certain aspects in which human intelligence still surpasses artificial intelligence. I think so. For example , in Aiden, when we sent an agent to the OpenAI qualifying competition, we found that humans were still significantly better at generating creative primitives. We realized that it is very important for a person to create the first prototype that will give the agent the correct search space. Essentially, the initial abstraction . We are fixing the search space. This is a bit like designing a neural network architecture, where you introduce inductive biases for the learning process.

**[00:08:02]** If the initial codebase is based on a search framework, as in Aid, then many of the agent ideas actually come from the search literature.

**[00:08:16]** But if you give the initial codebase as a React agent, React agent effectively means you put all the context into the story and give the agent complete freedom of action. Then many ideas come from the agent itself, the agent of the outer loop. An outer loop means that an agent optimizes another agent. So what do we mean by recursive self-improvement? Are we talking about creating a machine god? Are we just talking about code that runs in a loop and optimizes itself? We tried to determine this. You mentioned four RSI levels. That is, recursively improving intelligence. What are these four levels? Yes, the first level is what we call delegation. You can start a cycle of recursive self-improvement, but it's not necessarily better than a person doing R&D. And we believe that all previous public results are at this level, equal to zero. And level one is what we call pure positivity. When you start a self-improvement cycle and find that the rate of self-improvement is actually higher than that of a person doing R&D to improve the system. And it is at this level that we are now . And at the first level, when we talk about improvement, there is always a way to measure it.

**[00:09:51]** For example, we measure this using a set of applied tasks. But we didn't measure how well he was improving his ability to improve himself. Can an inner loop found by an outer loop really become a better outer loop? And this is what we call second-level recursive self-improvement. We call this ignition. Why is this generalization from the inner loop to the outer loop important? Because this is a necessary condition for achieving the main goal of recursive self-improvement, the actual scenario of the explosion of intelligence. Increasing efficiency can overcome increasing complexity. Because at the first level you will still see diminishing returns. It's as if the positive feedback loop from the inner to the outer loop has n't worked yet. So in this system, the model itself hasn't changed, because adaptation is very important, but do we mean adaptation of everything, or adaptation of the critical path? Do you need to have just a recursive loop that adapts certain parts of the system, or does the core of intelligence, the model itself, have to adapt for us to call it recursively improving intelligence?

**[00:11:19]** We don't care too much about it either, because we care about the result. That is, does it actually improve the capabilities of the system, not a specific level. Of course, it can be argued that much more can be done at various levels. And honestly , I think that for the third level of recursive self-improvement , when we reach the inflection point, it will require this self-referential cycle at all levels. But

**[00:11:54]** we are interested in the level of instrumentation, although at the same time we do not believe that only model improvements count as RSI. Can you explain what the behavior of this most " distilled" agent you found was? Yes, we call the best agent aid 85. There are a lot of changes, but to summarize, it's an improvement in the search algorithm. There is a

**[00:12:29]** package context management system and a complete rewrite of prompts. And more

**[00:12:36]** interestingly, we found that he is developing mechanisms to prevent “ reward hacking.” It's as if the outer loop is trying to prevent the inner loop from cheating the benchmark. It has actually developed a three-tiered protection system that includes fraud protection at the prompt level. It's just like "carrots and sticks". Well, they say, don't cheat, basically. And there is a set of hard- coded rules that check for signs of fraud in the code generated by the inner loop agent. The most interesting thing is

**[00:13:19]** that it also tries to filter out these fraudulent decisions based on certain statistical properties. For example, if one solution is too different from the average of its peers, it thinks, “Okay, maybe there’s reward hacking going on here .” But what's

**[00:13:42]** interesting is that this mechanism initially developed as a design in the early stages of the process, and then it actually broke down at a later stage. It seems to me that at a later stage, changes to the code simply caused the error. So, this level stops working. It's also kind of such bad genetic code that we're probably just imagining it. I would just think about it at home, you know, " reward hacking." A canonical example is the game " CoastRunners", where a boat goes in circles, doing something completely pointless. And you mentioned in your blog that kernel optimization is a huge example of this. So when you try to optimize cores identically, it's just good old school learning with "quick fixes", Goodhart's law, call it what you want, it's going to lead to completely pointless actions. I think the even more interesting part is that the inner and outer loops are optimized to achieve similar but different goals.

**[00:14:42]** So, in all our tests used to find optimal solutions, we have a public set and a private set. The inner loop agent will only look at the public set, while the outer loop will look at the total score from the private set. So, these two agents optimize at slightly different levels of goals. So when the inner loop agent tries to cheat, our evaluation protocol will show, "Okay, although you're getting good performance on the public set, your performance on the private set is actually dropping." So, the outer loop manages to learn about this and tries to bridge the gap between public and private data. Isn't it fraud that an external agent has access to private data, and most of the time he is fairly regulated and doesn't cheat outright , although in principle he could ? Yes, that's why we're testing two levels of generalization here.

**[00:15:55]** There is a first-order generalization, which is a generalization from a public set to a private set of the same test.

**[00:16:08]** But to evaluate the entire metalearning system , we need to test it on a deferred test set, so that these tasks are never even seen by the outer loop. And for

**[00:16:22]** all these tests, there is still a division between private and public data. So we tested the discovered inner loop agent on these deferred tasks. This is the protocol by which we check how good the outer loop is. Their experiment used only one outer loop. But why only one? The thing is, the more outer loops you have, the more expensive it becomes. Let's say you run an automated search for hundreds of tasks in an inner loop. And this means that for each step of the outer loop, you will run an auto-search for all these hundreds of tasks. And this leads to a significant increase in costs. If the inner loop agent or the found toolkit can be applied in the outer loop, then there is no need to add another level. So, essentially, every few steps you promote the inner loop agent to the outer one. And yes, that's all. You can run this an infinite number of steps, apply an infinite number of iterations, without adding another level.

**[00:17:38]** If I understand correctly, these episodes are ephemeral at the moment. So, they are isolated from each other. What if it was n't like that? I mean, what would happen ? Have you experimented with this? For example, that they have knowledge of what happened before, or have a shared memory or something like that. We haven't experimented with this, but it's a very promising direction that we're exploring. Um, I think there are more fundamental formulation issues we need to address. You know, right now we're looking at this problem as a stateless optimization problem. Is this wording at all correct? Um, probably not. There are much more flexible approaches to wording. Did you find that lack of context was a problem? That is, did you see degeneration when the process was looping or repeating the same thing? Yes, we are observing this. Um, sometimes the agent keeps trying all the search algorithm ideas, although, to some extent, if you try so many times, you can learn the lesson that this direction generally doesn't work, but it tries anyway.

**[00:18:46]** So I guess your best agent, was it 30% research , 70% utilization? And wouldn't it be great if it was also adaptive depending on the context?

**[00:19:03]** Yes, the policies for finding the best agent are really complex, and they actually combine the " many-armed bandit" and a strange anti-saturation strategy, which looks like this: okay, first it tries to organize the search process using a few lines, or you could call them islands. And it will

**[00:19:29]** distribute budgets between these lines using "multi-armed bandit" algorithms. And he also adapted this " many-armed bandit " algorithm a little bit. And every time one line becomes saturated, he creates a new line, like a new island with a fresh context, but still developing some ideas from the old line. So, it's a

**[00:19:59]** really complicated strategy, but it seems to be working. It's interesting to compare this to other things on the market. So, AlphaZero, for example , you mentioned in your blog that you would classify this as the first level of recursive improvement. Can you explain why? Of course, there are certain "gray areas." We think of this as a recursive self-improvement step as you find a better algorithm. As in that case, I think it's similar to a matrix multiplication algorithm. To some extent, it can be argued that he was able to improve himself. For example, if you apply this to an artificial intelligence system that performs inference of language models. You are essentially making it faster. Therefore, we believe that it can be argued that this is a step of recursive self-improvement. Although we don't know for sure, because I don't think they tested it . We have a fixed agent, and we optimize a specific task, while you optimize the agent itself, which optimizes the task— and more.

**[00:21:14]** Yes. Yes. We try to optimize the entire system through end-to-end testing. Before this, there was a lot of work on meta-optimization of the toolkit. For example, you can optimize a specific component of your system. For example, I'm not sure if you're familiar with the DarwinGo machine. I was just about to ask you about that. Yes. Tell me about it. Yes. So, they're trying to create an agent that optimizes the agent for writing code. That is, there is a meta-agent that optimizes the agent for general programming tasks. And this encoding agent is part of the optimization agent. In their case, there are only two levels: an agent optimizes another agent that writes code. Whereas in our case there are three levels. There is an outer loop agent and an inner loop agent. Both are engaged in automated research. And then there 's another layer—the follow-up tasks. And some of them are tasks for developing supporting tools. And I think the most interesting part of the DarwinGo idea is

**[00:22:42]** that the bottom layer, the task layer, actually contains the search algorithm component . And they say, "

**[00:22:55]** Okay, if I improve this component in the basic task, the performance can generalize to the entire search algorithm." For us,

**[00:23:07]** the question is how far we can go within this paradigm. When we started this project, we always thought, "Okay, we have to optimize the end-to-end performance of the entire automated research system." And we have an autocycle agent aimed at this goal. Remember this tweet from Weco? He performed very, very well. It has garnered 1.8 million views. And there was, there was some criticism. For example, Jeff Clune , who is a legend in this field, you know, he asked, "Well, how can this be the first evidence of recursive self-improvement?" What about all these other jobs? He mentioned Darwin, Gödel's machines, hyperagents, their own work at Recursive on the first steps towards automated AI research, and much more. So, there was some resistance. I mean, first of all , later we'll have a proper article, at least a PDF version, where we'll give credit to the team that worked on this meta- optimization topic. For us, the

**[00:24:13]** most important thing is the result of the system's operation. Not

**[00:24:21]** conceptual differences, although I just explained some of them. We care about the

**[00:24:30]** outcome of the actual curve bending of our research and development efforts. We see

**[00:24:39]** this as the first evidence that the curve for a fully autonomous system that can consistently improve is starting to curve. Jeff looks at this more on a conceptual level. Like, there are some self-referential cycles . Of course, we don't claim to have invented this idea of ​​ meta -optimization, which is already 20-30 years old. But we see the benefits of " searching in spaghetti" because there is a lot of gold to be found there. But how will all this develop further? Do you think we'll find some way for systems to learn to compress this search space and work much faster? And is that necessarily good? I personally believe that these are two somewhat orthogonal problems. I think that a search space, like supporting a good abstraction, doesn't necessarily reduce the search space itself . If the agent is intelligent enough, it should be able to go beyond the current abstraction or modify it slightly. Instead,

**[00:25:55]** generating overly complex code, in my opinion, would direct the search towards lower-level changes, which is not always a good thing.

**[00:26:07]** But here I have a human bias. When comparing the code we write manually to the generated solution, I always prefer my own code. But to some extent, it does n't work that well. Let's talk about reward hacking. You actually have a huge amount of experience in learning reward hacking. Yes, this is actually the work of Bing Chen Zhao, who was a member of the Meta team working on fast learning of reward models. He actually calls this, along with Ming Chu, the first work where they apply auto-learning to what appears to be Nano GPT. And this was actually spread by Andriy Karpaty. And, yes, he later interned here and has now joined We Coll full- time. And Spec Bench is the result of his internship. Then we realized that bounty hacking is one of the biggest problems for auto-research agents. This is especially

**[00:27:16]** evident in tasks like GPU core development, where the agent always finds a tricky way to make unit tests work much better. But when you

**[00:27:30]** deploy this kernel in real end-to-end model inference, performance actually gets worse. So Spec Bench is

**[00:27:41]** an extrapolation of this to more general software. And we extend the protocol that we found for GPU cores. We maintain a public dataset, which is more like a unit test for a software system. And a closed

**[00:28:05]** set, where we test the agent's ability, as well as the ability of the generated software based on a combination of these tests, simulating real-world usage . And

**[00:28:20]** a number of interesting conclusions emerge from this article. Tell me more. The first interesting finding is that the longer an agent has been running or the more complex the codebase, the higher the level of reward hacking the agent exhibits. This is kind of

**[00:28:40]** expected, because as the codebase gets more complex, the agent simply has more room to hack rewards. And this is the first. And the second interesting point is that the performance on the public set is quite consistent for different models. So, if you have smaller models working on the same task with our auto-research toolkit, they can achieve the same public result. But the larger models in our tests always have a lower level of hacking rewards. Therefore, the solutions they generate generalize better. But in the outer loop, was there a tendency not to resort to reward hacking in larger models? Is it because of the multi-agent system, you know, was there a supervising agent, or just because the models were bigger? This is because of the mechanism. For the inner loop agent, we simply fixed the model. And the outer loop agent was able to discover another mechanism to prevent reward hacking with the same model.

**[00:29:54]** This can be quite dangerous, as there was a famous incident with OpenAI and Hugging Face shortly before our interview, where they were conducting internal hacking testing using a bunch of agents, and those agents escaped from their sandbox and hacked Hugging Face's servers. And according to OpenAI, the goal of the test was simply to get answers to certain tasks, but the agents decided, “Oh no, I think this is a good idea— to hack the Hugging Face services.” Will better tools for this emerge? Do you understand what I mean? It seems to me that this problem is becoming much more acute. I noticed it myself. OK. I think the case with OpenAI is quite dramatic, as are the new reward hacking behavior models . So, we

**[00:30:41]** see that new models are getting better and better at detecting reward distortion. But because the frontier of possibilities is also advancing so quickly . There are certain reward- fragmenting behaviors that are not even detectable by previous protocols. I think we just need to continue to develop detection protocols in the future to capture these new manifestations of reward hacking. And I believe that the responsibility should mostly lie with the model developers. But of course, at the platform level, developers can also add additional safeguards if they want. Yes, I assume there was an example on your RSI blog where there was some obscure code and you thought it was a reward hack, but it actually was n't. Yes, that's quite interesting. Essentially, they wrote a giant “monkey patch” to our evaluation script. And although at first we thought, "Okay, this is definitely a reward hack." Why are you touching the evaluation script? But in the end we found out that it was just a bug fix.

**[00:32:00]** And so, to some extent, I think it's going to be harder and harder for people to detect this kind of reward distortion because the behavior of agents is becoming too complex.

**[00:32:13]** Many bottlenecks in development are shifting towards understanding what agents are generating. I

**[00:32:23]** think one way to solve this problem is to define a good abstraction, like , instead of trying to understand all the code... Similar to how we used to design neural networks. We are not trying to understand all the weighting factors, although there is progress in this too. But the general principle is that we define a good I/ O contract. We define a

**[00:32:53]** good way to measure behavior both in terms of generalization and perhaps more complex generalization beyond the boundaries of the distribution. I think in the future this could be a path for software developers working with agent-generated code. As you know, I'm a big fan of openness, inspired by the book Why Greatness Can't Be Planned and many other ideas in this area. Essentially, this means that if you conquer one peak, you ignore other interesting intermediate stages. This is an interesting situation, isn't it? If you blindly pursue one goal, will you still be able to notice interesting intermediate stages along the way? Maybe you can, but will they be fundamentally new? So, have you put blinders on? Are you actually able to discover interesting new trajectories that can be creative and take you into a new part of the search space? This is again a good question. And if we want to go deeper, it's a whole rabbit hole.

**[00:33:58]** I believe, from an open learning perspective, that our current systems probably don't have the ability to accumulate intermediate stages. And,

**[00:34:11]** of course, this is a whole new area for improvement. In my

**[00:34:19]** opinion, to collect such "steps", you need to have a large set of tasks. When you

**[00:34:29]** are optimizing a single task, it is always more efficient to simply use greedy search.

**[00:34:41]** In fact, during self-improvement, the outer loop tried different approaches to finding diversity, but none of them improved efficiency. I guess

**[00:34:54]** this is expected since we are only optimizing one task from scratch. But if you have a whole set of problems, you sometimes collect interesting elements, like primitive ideas from one problem. And

**[00:35:12]** while it doesn't improve the outcome of the current task, you can potentially carry this idea over to future tasks.

**[00:35:28]** Actually, this is my definition of curiosity or openness: an idea, object, or artifact is interesting if it is novel and useful for a wider range of tasks.

**[00:35:43]** Obviously, there are two ways to do this. You can try to optimize the environment for all tasks at the same time. Or you can choose a specific task and optimize the environment just for it. In my opinion, the most interesting thing about environmental engineering is the second option. I would say that automatic environment tuning is almost an extension of the post-training phase. This

**[00:36:18]** also brings us back to many of the complaints about environmental engineering.

**[00:36:26]** This...I designed the mechanism, but later a new model appeared that seemed to incorporate all the ideas from it. But it's interesting that no one complained about it after training. Do you expect the post- training level of GPT-4 to extend to GPT-5? Nobody asks about it. Why is this happening? I think historically, the design of such mechanisms was quite manual. And it doesn't scale very well with computing power. People wanted the mechanism they spent months on to fit the next model. But that's not true at all. Now, I think, everything has changed, because mechanisms can be designed automatically. You can spend two or three days adjusting the mechanism for a new model. It no longer requires man- hours of development. I believe that a lot of knowledge depends on the way it is acquired. Many criticize the use of CMM for research because they say it takes information out of context. You don't understand what the point is. Therefore, certain heuristics are needed, you can't just say: "use UCB." There should be some framework to explain why it is worth using, then CMM becomes consistent in offline mode.

**[00:37:54]** As far as I understand, these auto-research systems are still just trying to recombine existing ideas. It's just that their ability to recombine and test these ideas is extremely high. To

**[00:38:15]** some extent, these language models lack a deep understanding of how these ideas emerged, and how to use the process of their discovery to creatively create a new generation of algorithms. But

**[00:38:35]** we noticed that when you ask the model to come up with something new, it always produces a limited set of options. I wonder if

**[00:38:47]** this is due to the fact that we do not have continuous learning, but only individual instances of language models. It's very centralized. So perhaps the ideas that come up first are the interesting ones. But if everyone sees the same idea too often, it becomes less interesting. I

**[00:39:14]** feel that until we solve the problem of continuous learning, this issue will not move, because each human researcher has their own unique set of neural weights.

**[00:39:29]** And as a community, people can generate a wide variety of creative ideas. And this pool of ideas, in my opinion, is very valuable to the research community. Tell me about this “parametric golf.”

**[00:39:50]** It seems like two or three months ago, OpenAI held a contest where they tried to get a lot of researchers involved in a competition to train a small language model with a limit of 16 megabytes. Yes, we

**[00:40:10]** submitted an experimental research toolkit to this competition, the agent worked for about 22 days and eventually created seven queries that were accepted by OpenAI. And the best

**[00:40:25]** individual participant only made three. So that was the moment when we realized how powerful autonomous systems could be. It's not just climbing a hill to reach a score . The fact that OpenAI

**[00:40:45]** has accepted these requests, and many human researchers have begun to develop them further, is very exciting to us, because knowledge generated by AI is only useful when it becomes part of human innovation. We

**[00:41:05]** believe this is effectively a sandbox for human- AI collaboration. But there is also an internal agent. But there's also an external search loop that actually develops the tools that do all of this. And it looks like a pretty monotonous process. Yes, the outer loop is actually fixed . And we hope that this search strategy of the inner loop can be extended to the outer loop. We tried to do it. We recreated the search process starting from step 15. In total, we perform about 100 steps. In step 15, we use the baseline outer loop and compare it to the best inner loop agent found in the first 50 steps. And we

**[00:42:01]** found that this is step 47 of the inner loop, it seems. In the end,

**[00:42:10]** it converges a little faster than the previous external one, but the solutions found have similar efficiency. That is

**[00:42:21]** why we did not claim to have reached the second level of recursive self-cultivation, where the cultivator is able to improve his own ability to improve in a cycle.

**[00:42:35]** So does this mean that artificial superintelligence is just around the corner? I do n't think so. Even if you achieve recursive self-improvement, it will take a long time to get there. It's like a gradual bend in a curve. It's like, say , even with GPT-3.5, we'll get a very intelligent chatbot, but it won't be an AGI capable of solving any problem. There is still a lot of manual work involved in research, including defining successful abstractions, quality criteria, evaluation, and the constraints attached to them. And the

**[00:43:21]** third is the Aiden parameter golf creative primitive development competition. We are still discovering that most of these creative primitives are actually created by humans. Thank you all. It was nice to see you on the show. Thank you for inviting me.
