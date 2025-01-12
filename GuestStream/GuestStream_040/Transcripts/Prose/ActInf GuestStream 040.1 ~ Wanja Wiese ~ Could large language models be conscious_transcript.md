00:07 _Daniel:_

Hello and welcome.
It's March 29, 2023.
We're here in ActInf 
GuestStream number 40.1 with Wanja Wiese.
We're going to be hearing a presentation in the first section and then having a discussion.

00:23 So thank you, Wanja, for joining.
Again, really looking forward to your presentation.

00:30 _Wanja:_

Thank you very much.
So this presentation is based on a preprint that can be found at Phil Archive.
And this is work in progress.
And I probably or hopefully upload a revised version of this preprint in a few weeks.
So if you're watching this or if you're reading the preprint and have any comments or questions, feedback is very much welcome.

01:02 And I'm also, again, grateful for having the opportunity to present here because I'm really looking forward to the discussion and any comments that people may have while watching this video.
So do contact me if you have questions or comments.

01:23 Now I want to start this presentation with an idea from this wonderful novella by Tet Qiang, The Lifecycle of Software Objects.
And if you're not familiar with the novella, it doesn't matter.
So there are some digital entities, or Digians as they are called in the novella, who at first live in a purely virtual environment.
So these are virtual entities like virtual pets, and human users can interact with them in a virtual environment.
Then in some passages of the novella, there are scenes in which some Digians are, as it were, downloaded from this purely virtual environment and are implemented in a physically embodied robot.

02:25 So the program that is running within this computer simulation and is controlling the purely virtual body is then downloaded into a physically embodied computer and is controlling a physical robot which can interact with its physical environment, non virtual environment, in the same way in which the virtual agent, the virtual digient, interacts with the virtual environment.
And I find this idea really fascinating and powerful.
So the novella suggests that these virtual entities are conscious and that they can switch back and forth, as it were, between this purely virtual environment and the physical non virtual environment.
And the idea is that these entities remain conscious when they're in the robot, but also when they return to the virtual environment.

03:36 And to some people it may be unintuitive or counterintuitive that a purely virtual entity in a simulated environment can be conscious, but maybe some of these people will find it less counterintuitive to imagine a conscious robot.

03:59 And so the the idea is is fascinating to me because it suggests that if you can switch back and forth from the virtual environment to the physical environment and in the other direction, it really doesn't matter where the software is implemented, the system remains conscious.
And I will come back to this idea at the end of my presentation and we will see what the account that I'm presenting here suggests with respect to this scenario.

04:40 So this is the overview of my presentation, which is based on the preprint.
I'm just omitting a lot of details.
I'll start by saying just a few things about the free energy principle.
Then I will ask what is the difference between an unconscious simulation of a conscious system and a conscious computational system?
Or in other words, what's the difference between what is called weak and strong artificial consciousness?

05:11 So strong artificial consciousness is an actually conscious artificial system and weak artificial consciousness is constituted by an visual system that maybe behaves as if it were conscious or that simulates a conscious being but is not actually conscious.
And I'm interested in the question what's the difference?
And a particular version of this question is whether a computer simulation in a computer with a Bonoman architecture can be conscious.

05:54 So I start with the free energy principle and I don't want to go into the details.
So we start with a description of a physical system.
So the X is the the physical system.
And the fundamental assumption is that the dynamics, the physical dynamics of this system can be decomposed into two components.
So we on the one hand have a deterministic flow term f and then some noise term, stochastic noise term.

06:32 So we end up with a stochastic differential equation which describes how the physical system evolves over time.
The further assumption is that we can decompose the states of the system into internal states mu, external states ETA, sensory states S and active states A, which together the sensory and active states together constitute the blanket states B.
And this then is a particular system system that can be partitioned into internal and external states, separated by blanket states.
And a further assumption is that the dynamics of this system can also be partitioned in the following sense that we can decompose this flow term into individual flow terms for the different states.

07:36 So we have a flow term for internal states mu and can also describe the dynamics of internal states in terms of such a differential equation here.

07:49 Okay, so these are just technical fundamental assumptions made by the free energy principle.
But then interesting thing starts here when we look at how else we can describe internal states and the dynamics of internal states.
So the idea is that we can map internal states mu to probability distributions.
So this is your formulation in terms of states.
And then the idea is that at every point in time the system will be in certain states, so there will be internal states relative to each time point and we can map each of these states to some probability distribution Q of external states given blanket states.

08:47 Okay, so we can do that, but then the question is why should we do that?
And the idea is that maybe we can redescribe the flow term, which is essential for characterizing the dynamics of internal states.
Can we redescribe this flow term in terms of the probability distribution encoded by internal states and the free energy principle?
Answers.
Yes, we can rewrite this term in terms of a variational free energy functional, which specifies how the probability distribution q, which is parametrized by mu, and thereby also how mu changes over time.

09:36 So we can reformulate the physical dynamics of internal states.
We can rewrite the flow term in terms of variational free energy or in terms of minimizing variational free energy with respect to a probability distribution encoded by internal states.
And this is then called Bayesian mechanics.
And it's called Bayesian mechanics because minimizing variation of the energy involves minimizing a divergence term between the internally encoded probability distribution q and a posterior over external states given blanket states.
Okay, so to sum this up, I will give these ideas some labels.

10:33 So, I've already talked about the physical dynamics, and these are the dynamics of a particular system described by a stochastic differential equation involving a flow term and a noise term.
And recall that a particular system is a system that can be partitioned into internal, external, and blanket states, and then, according to the free free energy principle, can redescribe these physical dynamics in terms of as computational dynamics.
We can reformulate them in terms of a description of the system's internal states, Mu, as performing approximative Bayesian inference by minimizing variation of free energy with respect to a probability density encoded by mu.
So, in short, we can reformulate the physical dynamics as a computational process that involves a form of Bayesian inference.

11:35 Now, a further assumption that I want to make here is that we can capture the computational correlates of consciousness in terms of the computational dynamics as described by the free energy principle.

11:52 So here the computational correlates of consciousness, or Cccs, are defined as the computational dynamics of a physical system, of a conscious physical system, as specified by the free energy principle.
So this is not just any physical system, it's a conscious physical system.
Forgot to add this on the slide.
All right, so given these initial assumptions and definitions, can we say something about the difference between weak and strong artificial consciousness?
And I think we can.

12:30 So let's start with the idea of a computational call it of consciousness.
Computations are medium independent, so it's plausible that a digital computer can implement computational correlates of consciousness.
But then the question if we want to distinguish weak from strong artificial consciousness is, is every system that implements Cccs conscious, or do systems have to implement these computations in the right way?
And what would that be?

13:10 To better understand this question, I find it useful to look at this diagram and see where we started.
So we have a description of a conscious system's physical dynamics in the bottom left.
And then according to the free energy principle, we can reformulate this, redescribe this as some computational dynamics.
And by assumption, these include the computational correlates of consciousness, and they must be implemented by the physical dynamics of the conscious system.
Now, given that these are medium independent properties.

13:58 They can also be instantiated by other systems.
And here I'm assuming that these computations can also be implemented by a digital computer.
And the digital computer, as a physical system, has some physical dynamics.
And if we can apply the drainage principle to it, we can reformulate these physical dynamics as computational dynamics.
And so then the question becomes, do these computational dynamics, do they include the computational correlates of consciousness, whatever they are?

14:37 So this is a crucial question that we have to answer if we want to know what the difference between weak and strong artificial consciousness is.
Maybe there is no difference.

14:53 So before I present an argument to the effect that in general, the computational dynamics of a digital computer will not entail the computational corals of consciousness, before I present this argument, I will present some observations on the free energy principle.
So note that systems that conform to the French principle sustain their existence by minimizing variation of free energy, but the reverse does not hold.
So you can run simulations of agents that minimize variation of free energy, and you can do that on a computer which does not thereby sustain its existence.
So it would continue to exist regardless of whether it runs these simulations or not.
Okay, just to illustrate this with a quotation which may be familiar to many so this is by Chris Mattel.

16:05 Many theories in the biological sciences are answers to the question, what must things do in order to exist?
The French principle turns this question on its head and asks, if things exist, what must they do?
More formally, if we can define what it means to be something, can we identify the physics or dynamics that a thing must possess?
And Jacob Howie puts a similar point as follows.
The free energy principle analyzes the concept of existence of particular self organizing systems.

16:42 So the idea is that continuing to exist, sustaining one's existence, means minimizing variational free energy.
And so any processes that contribute to minimizing variation of fringe thereby contribute to the sustained existence of the system.

17:08 But such processes can also be implemented in other ways by different systems which do not thereby sustain their existence.
And this, I want to suggest, is a crucial difference between systems that merely simulate conscious systems and systems that actually are conscious.
Okay, I will hopefully clarify this idea in a moment by presenting an argument.
But before that, I need a definition.
So I want to introduce a notion of intrinsic computation.

17:48 And these are just computations that contribute to the sustained existence of the systems.
So these are the computations that figure in the computational reformulation of the system's physical dynamics.
According to the free energy principle, an intrinsic here means these computations are observer independent.
So it's not the case that we as observers say, okay, we can interpret the system as performing these computations, or it's useful for us to use them as computational devices.
The idea is that these computations are processes that are intrinsic to the system, that only depend on properties of the system itself and not on relations that the system has to observers or to other beings.

18:47 Okay, so here's the argument, which in a way is already contained in the preprint.
But I did not formulate the argument in this explicit way.
So I'm grateful to Tommy corBack, who provided some comments on my preprint and who also suggested a reconstruction of the argument that I'm presenting in the preprint.
And this formulation here is based on Tomic's suggestions.
And I hope this clarifies the argument that I'm putting forward developing in the preprint.

19:38 Okay, so the first assumption, and the argument is a version of computationalism about consciousness.
So the idea is that causal roles that characterize phenomenal consciousness are medium independent and can be captured in terms of computation.
These are computational correlates of consciousness.
So the idea is that consciousness does not require a particular type of substrate.
It can be, in principle, can be realized by different types of system as long as these systems implement the right computations.

20:21 So this assumption, as I intended, does not entail that implementing the right computations is sufficient for being conscious.
It's here just meant as a necessary condition.
And the idea is that there are informative, interesting computational crawlers of consciousness and they can, in principle be performed implemented by different types of system.
Then comes the second assumption, according to which every conscious system and its computational correlates can be described by a mechanical theory that conforms to the free energy principle.
So this is an assumption about the scope of the free energy principle.

21:14 And it's at least clear that the free energy principle is intended to have a very wide scope that's not meant just to apply to the human brain.
It's not just meant to apply to living systems, but it's meant to apply to a very wide class of self organizing systems.
And this idea or this intention that the free energy principle has a very wide scope is also evidenced by the fact that recent formulations and recent developments in research on the free energy principle seek to relax certain assumptions.
That were made in previous version so as to make the free energy principle applicable to a very wide class of systems and not, for instance, just to systems in non equilibrium steady state.

22:22 For instance, just as one example.

22:26 All right, so the idea is that we can apply the free energy principle to conscious systems.
And that means we can move from a description of physical dynamics to a description of computational dynamics.
And these will include computational correlates of consciousness.
The third assumption makes a connection between intrinsic computation and consciousness.
A system is conscious only if it sustains its existence by virtue of the computational correlates.

22:59 It realizes such computational correlates of consciousness are intrinsic computations, computations that contribute to the sustained existence of the system.
So if a system follows certain or implements certain physical dynamics, which under the Fep can be described as computational dynamics that entail computational correlates of consciousness, whatever they are, then the system is conscious.
But it's only conscious if it's in this direction.
So, in principle, it's possible to implement the same computational processes without being conscious.
And this becomes clear in conclusion or described by conclusion one, it's possible to instantiate computational calls of consciousness in a physical system without instantiating consciousness, namely, if realizing the computational correlates of consciousness does not contribute to the sustained existence of the system.

24:11 So assuming that a digital computer can perform the computations that characterize consciousness in conscious systems, it's likely, according to this proposal, it's likely that the computer will not thereby be conscious because it could implement different computations.
It really doesn't matter what computations it performs.
It will continue to exist as a physical system regardless of the computational processes that it implements.
So it does not sustain its existence by virtue of the computations it performs.

24:58 All right?
And a condition that is entailed by this is that from the point of view of the free energy principle, computation of the physical system is intrinsic if it matches the system's physical dynamics.

25:19 And this will be important also for the question about consciousness in computer simulations.
So the second conclusion that I want to draw here is that computers with a von Neumann architecture cannot implement intrinsic computations because their physical dynamics induces a causal flow that is different from the causal flow entailed by the computational dynamics.
So there's no match between the physical and the computational dynamics or between the physical dynamics and the computations that are performed within the computer simulation.
I will unpack this in the third part of my presentation.
So could there be consciousness in a computer simulation, in a computer with a classical architecture?

26:17 So this is an idea that I already presented in previous works.
So in a system that conforms to the free energy principle, there's a basic flow from internal states via active states to external states and from external states via sensory states to internal states.
So we have these circular dynamics.
And in a computer with a von Neumann architecture, the basic causal flow is a bit different.
So we have memory and we have a separate processing unit and units that store the values of the different variables of internal that stand for internal, external and blanket states.

27:10 They are in the memory unit, and there's no direct causal interaction between these units, but it's always mediated by the CPU.
So that's a basic idea.
And therefore, there's difference in a causal flow.
And this means that the physical dynamics of the computer does not have a or the if we want to reformulate the physical dynamics of the computer in terms of minimizing variation of the energy, we end up with something that cannot match.

27:54 We end up with computational processes that cannot be identical to the computations that are simulated by the computer because then there would have to be a match between the states that represent the probability distributions encoded by internal states and the internal states themselves.
Okay?
So from this, I suggest we can derive two necessary conditions for consciousness.
One is the flow condition.
The causal flow of a physical system's computational dynamics, which may realize computational correlates of consciousness must match the causal flow of the system's physical dynamics.

28:48 And then there's a second condition which I call the existential condition.
A physical system sustains existence by virtue of realizing computational correlates of consciousness.
So if it's a conscious physical system, then this is the case.
All right, just a few observations or notes about this.
So a system can satisfy the first the flow condition without thereby satisfying the existential condition.

29:20 So the existential condition is stronger than the flow condition.
But if a system satisfies the existential condition, then it also satisfies the flow conditions.
And not all systems that satisfy both of these conditions are conscious.
In other words, neither of them are sufficient for consciousness.
These are really just strictly necessary conditions for consciousness.

29:52 All right, let me return to the idea that I presented in the beginning from Pat Xiang's novella.
So from the point of view of the account that I presented here, is it possible to download virtual entity to a robot?
And will it be conscious, or can it be conscious in the simulation?
So I should just assume here that these systems satisfy the flow condition first condition.
So assuming that this is a very special computer simulation in which the physical states that represent internal, external and blanket states, that these physical states also directly causally interact with each other and according to the account proposed here, the computer simulation.

31:01 There would still not be consciousness in the computer simulation because the computer does not sustain its existence by virtue of performing these computations.
It could also run different simulations which do not involve these digital entities, and it would continue to exist.
So according to the account presented here, there would not be consciousness in this system.

31:32 And if we download the part of the program that controls the virtual agent and download it to a physically inverted robot, could that robot be conscious?
Well, in principle it could if the robot sustains its existence by virtue of performing the computations that are also performed by the computer simulation.
And now this result might be a bit strange because contrary to what the novella suggests, it would suggest that the system cannot switch back and forth between the virtual and the physical non virtual environment without losing consciousness.
And I admit that that is a kind of counterintuitive implication.
But maybe it only seems counterintuitive.

32:36 Maybe it's not technically possible to download a virtual entity which was trained in a purely virtual environment and download it to implement it in a physical robot and thereby allowing the physical robot to interact with its environment in the same way as a virtual entity can interact with a virtual environment.
So I know that in robotics there's a certain strategy to train robots or to develop the controller of the physical robot, naming that you first train it in a virtual and a simulated environment, and then you use that to control the robot.
Maybe this only works for robots that kind of have certain limitations in their sensory motor abilities.

33:42 Maybe it doesn't work for highly sophisticated robots that are more like conscious organisms which can react adaptively and very flexible in a flexible way, can interact flexibly with the environment on the basis, maybe, of effectively guided, effectively shaped representations.
So this would be maybe an empirical hypothesis derived from my account that this strategy, this symptom real strategy of simulating an entity in a virtual environment and then applying that to a physical entity, the prediction would be that this has at some point reach limits and will not be successful.

34:36 If, on the other hand, this hypothesis or this prediction will turn out to be false, I think we should reconsider the account that I'm presenting here.
Okay, let me conclude.
I've asked what is the difference between weak and strong artificial consciousness?
And the suggestion is that it's about intrinsic computation.
That's the difference.

35:06 Actually.
Conscious systems sustain their existence, at least in part by virtue of performing certain computations.
And a mere simulation of a conscious system does not thereby sustain its existence.
It could also perform different computations and still continue to exist.
This condition entails the flow condition, which is important for the second question.

35:31 Could a computer simulation in a computer with a Van Neumann architecture be conscious?
No, because it violates the flow condition.
Okay, here's an ad for the journal Philosophy and the Mind Sciences, which I'm running together with Sasha Fing, Jennifer Wind, and Regina Farpri, and I thank you for your attention.

36:05 _Daniel:_

Awesome.
Thank you.
I'm just getting my video back in the game while I'm getting everything back on the stream.
First, just thank you for the presentation and wanted to pick up with that robotics intro and conclusion.
To what extent does the embodiment in the robot matter beyond the ability of the virtual simulation to do things like eject.

36:52 The CD drive or ultimately do physical things, just not the kinds of physical things that we see human children do, like play with toys?
When you were thinking about the virtualized simulation, were you thinking about one that had no access to sensors and actuators?
Or what happens when the digital simulation also has access in some limited way to the ability to sense and act on the outside world?

37:35 If you have any thoughts sorry about that.
On the stream, it was audible, but not to you.
But now I've resolved the zoom.
So we can, from your consciousness perspective, consider it a new question.
So I just wanted to pick up with that robotics example, a digital simulation may still have sensors engaging with the world and may still be able to undertake actuation if only something like flipping a switch on a processor.

38:11 So what exactly about the embodiment do you think matters for it to have that kind of adaptivity and maybe even open endedness and learning that you pointed to as an important property?

38:29 _Wanja:_

Yeah, good question.

38:34 I think there are many different aspects that you're touching upon.
Let me start with this one.
So I mentioned my correspondence with Atomic corBack and one thing that he suggested was that couldn't we regard a language model as a system that has certain sensory motor abilities so it can interact with physical environment via a linguistic interface?
So it receives text as input and it outputs text as outputs text.
And can't we regard this as sensing and acting?

39:32 I think it's similar to one of the aspects that your question touches upon.
So what is it about the embodiment?
And can there be different forms of embodiment that might still lead to consciousness?
And I don't have a full reply to this, just two things that I would mention here.
The first is that there are certainly some analogies between what a language model does when it interacts with a user and a system that maybe an organism that interacts with its environment via perception and action.

40:18 But there are also some dis analogies.
So when it comes to interacting with the environment, when an organism interacts with its environment, their temporal constraints, it's really important that it does the right thing at the right time and reacts fast enough and so on.
And for a language model, that does not play a big role.
So there's one difference.
And then there's also a difference in the format of the representations.

40:58 And in principle you could say, okay, why does this matter?
And maybe in the end it doesn't.
But I just want to mention that there's some crucial dis analogies that I think would be important to take into consideration and evaluate.
Then there's a question, okay, is there something about these more low level sensory motor skills that is crucial when it comes to consciousness?
Now, on the one hand, we know that an organism can be conscious without having any language skills, without being able to speak or understand language.

41:50 So this is why when it comes to functions of consciousness, for instance, people don't look for or usually don't look for linguistic abilities, but more for sensory motor abilities or forms of learning that enable or improve interaction with the world.

42:14 This is one thing, but of course, in principle it could still be that a system that lacks these low level, low level skills is conscious.
But then I would say if it's possible to be conscious without having these sensory remote skills, then it's not really about any ability for interaction with an environment that a system is conscious.
But then it's merely because of some internal computations that the system performs.
So if you're thinking about systems that might be islands of awareness, systems that don't receive any sensory input and don't produce any motor output, then I wouldn't want to rule out that such systems are conscious and these such systems don't have any ways of interacting with their environment.

43:17 So I'm happy to accept that interaction with the environment is not required for consciousness.

43:29 But coming back to language models this would mean that being able to interact with users using language is similarly not required for consciousness.
So I would say if such a system is conscious then it's not because of its ability to interact with the environment, but because of the internal processes.
And what may be crucial is not the actual interaction with the environment but just the potential for interaction with the physical alignment.
And then it might in principle it might very well be that a language model can facilitate interaction with the physical environment, for instance if it's connected to a physically embodied robot.
And I mean, there's research going on on such things.

44:33 Researchers who try to improve the abilities of their robots by connecting them or interfacing them with a language model which can then help translate commands into motor sequences.

44:53 What this suggests is that maybe there are some crucial types of representation or computational processes that are actually already implemented in language models or in other systems that don't really not directly interact with the physical environment.
And I'm happy to accept that.
But I would add that at least according to the proposal that I've presented here, you need something more for that.
And you need really it's not sufficient to just implement these computations, but they must have a meaning for the system itself, in the sense that the system will sustain its existence by virtue of these processes if it is connected to the real physical environment.

45:59 Now maybe that I've not addressed every aspect of your question so feel free to restate your question.

46:10 _Daniel:_

It's great.
It got to a great place because I wanted to follow up with this intrinsic computation concept.
So you mentioned that they're observer independent to the extent that anything or any process can be and that these are the kinds of processes that actually enable the persistence of that thing according to the Fep.
And so I was thinking about this first in a bottom up way.
Like this is the firmware, this is the Linux kernel.

46:49 This is the kind of enabling software that is supporting potentially extraneous higher order functions and that is allowing some kind of separation or delineation between what we can say are like the vital and intrinsic like almost the homeostatic functions and then second order functions.
But then I thought about the ecology that the computation is deployed in and so let's just say that the software is being the software simulation is being used in a scientific context.
Or to run photoshop and another cognitive agent keeps that simulation alive because it's performing some function.
And so from that bottom up sense the Photoshop program is not the Linux kernel so it's not like the Photoshop.

47:50 Like the Photoshop in principle is not sustaining the persistence of the entity in a bottom up fashion.

47:59 However, in deployment it actually becomes a necessary condition imposed externally and that will also be extremely observer dependent or subjective.
So how do we think about in standard modern computers or in Wetware?
What are these intrinsic computations?

48:32 _Wanja:_

Thank you.
That's a great question.

48:39 I can say more about intrinsic computation in a moment but just one comment before that.
So I think you're touching on a very important issue and that's a question by what is a system in the first place.
So if we want to consider the question what kinds of entities can be conscious?
And we have to first say okay, what are the entities that we're looking in at in the first place?
What are these things?

49:15 And why can't we look at a piece of software or some process that is running an app that a user is using?
What was the example that you gave?
Photoshop or something?
So why can't we regard Photoshop and a particular instance of this software as a system which exists for some time and it will continue to exist if it's useful for a human being and it's useful by virtue of the computation computations that are realized by it.
And so can't we say that the system sustains its existence by virtue of the computations that it performs?

50:14 That's I think a very crucial question because it's so fundamental what is a system?
And currently I think that the free energy principle is sufficient to answer this question but it may be that it's still too general.
So I dean the free energy principle gives us an answer to the question if something exists, what must it do?
And so it analyzes this notion of the continued existence of self organizing systems and maybe it does apply to the processes that implement photoshop in the computer of a human being who uses this software.
And if that's the case, then I think we have to add some further constraints it may be necessary to add some further constraints on the kinds of systems that we want to regard as potentially conscious or that we want to consider when it comes to the question what kinds of systems can be conscious?

51:42 And one suggestion or idea that I think would be worthwhile to explore here is to investigate to what extent something like the free energy integrated information theory may complement the free energy principle in this regard.
Because integrated information theory has a very strong emphasis on the notion of existence, of what it means to exist, what it means to be what it means to intrinsically exist, as it were, and not just in the eye of a beholder.
And maybe we need to add constraints from something like integrated information theory, which would then tell us what types of systems really exist.

52:42 And then maybe it would say, okay, the processes that are implementing Photoshop in this computer don't really exist in an intrinsic sense.
Yeah.

52:58 So this would then be my suggestion to add some constraints.
But of course, you could say, well, no, such constraints are completely unnecessary.
We don't need to exclude certain systems, and we can regard the processes that implement Photoshop as a real system that sustains its existence.
But my intuition would be, at least currently, that such processes would, at least in a classical system with a classical hardware, would be too scattered, and there would be so many physical processes interfering, as it were, that you can regard this as a separate thing which is distinct from other things that are happening in the computer.

54:06 But I would say this is more an observer dependent property.

54:13 Those processes, they're so entangled with other processes in the physical system that they are not particular systems in the sense of the free energy principle.

54:31 _Daniel:_

Awesome.
And again, kind of journeys us to another question about the topological or geometric concordances between physical and computational dynamics.
And it made me think of a few different kinds of systems.
The von Neumann architecture described with the CPU and the Ram regular desktop computer situation.

55:00 Of course, we have unconventional computing paradigms, quantum and analog computers.
We have the brain and the SPM package in which statistical inferences help us model how brain regions that aren't connected through, for example, axons can still have an edge in a Bayesian graph.
They could still have a causal effective or functional connectivity without being structurally connected and vice versa.
And then to kind of bring it back to the computer and what you brought up about whether or not those processes would be too scattered, what about a computer, either a distributed computing cluster or a strict virtualization scheme on the computer such that certain variables were isolated?
Would it be enough for the system to have some kind of constraint, again through a physical networked layout or through a virtualized system so that the computational flow and the causal flow could be played with in a different way?

56:18 And then how would we know?
What would we be looking for?
Surely not simply test retest accuracy or efficiency in some way.
That's not what consciousness is.
So, I mean, it really comes down to what are we looking for or talking about if we did have the ability to design different systems that did have different overlap with their computational and structural aspects.

56:49 _Wanja:_

Yeah, great question.

56:54 I think it's very important to look at different types of computer architecture, different types of hardware, and you mentioned some.
So there's actually something that was pointed out to me by Johannes Kleiner.
So he pointed me to the notion of computation and memory or something similar, and if I understand that correctly, it is a slight departure from the Van Norman architecture because you actually do computations within the memory unit.
So it's not that you have additional memory units within the CPU, but you perform computations in the memory unit itself, which would be a way of satisfying the Axel constant, the flow condition that I mentioned.

57:57 And similarly, there may be other architecture, maybe neuromorphic hardware that also could implement simulations in a way that satisfies the flow condition.

58:14 And as I pointed out in the presentation, the flow condition is just one necessary condition which is weaker than the existential condition.
So all of these systems, even if they satisfy the flow condition, would not thereby also satisfy the stronger existential condition.
But as may have become clear, I am not completely certain about this existential condition.
Or rather, there may be some ways in which one can describe what's going on in such systems that you can actually say, okay, the processes that implement these computations, they are systems, particular systems to which the free energy principle can be applied, even if maybe the material on which these processes run is not directly affected by these computational processes.

59:26 So maybe if we think about maybe neuromorphic computer chips, maybe the chips themselves, they will continue to exist no matter what computations they perform.

59:40 But if what's going on, if the activity that implements the computations within such a chip is sophisticated enough or has certain properties, maybe this activity can be regarded as an instance of a particular system to which the free energy principle can be applied.
So I'm not completely certain about this and I think this is something that has to be clarified.

1:00:16 Maybe it will be useful also to see what people are actually working on the free energy principle would say about this.
That's very important point.

1:00:28 _Daniel:_

Yeah, a few things that makes me think of first is kind of like the hard problem of virtualization or something in that some modification of a hard or an easy question.
And then also about the difference between a case where the material substrate of computation is its own self referent sustainer and another case in which the material basis of a computation is projecting, let's just say a non equilibrium steady state like a holograph or it's creating robots, it's spinning out robots or it's doing 3D printing.
So in that situation, depending on how the system boundaries are modeled, the viability of one part, maybe even like its kind of semantic germline is required for the continued propagation of some other part of this persistent system.

1:01:28 But Thomas Parr is actually disposable even though it's the embodiment.

1:01:35 I'll go to a question in the live chat and also I think it was a mem computing was the memory based computing architecture.
Yeah.
And agree, there's a lot of interesting threads there.
So Ali asks a question in the chat he wrote, what about understanding?
If we define understanding as a kind of correlation or mapping between spaces of semantic possibilities?

1:02:01 Can we say that large language models do indeed understand their prompts and outputs?
And does understanding in this sense require or entail consciousness or vice versa?
So with understanding as a map among semantic spaces, what can we say about Llms and understanding?
And what is the relationship between understanding and consciousness?

1:02:24 _Wanja:_

Thank you.

1:02:25 That's a very good or these are very good questions.
And of course, it depends on the notion of understanding.
And if we conceive of understanding as a way of grasping inferential relations or associative relations between different notions, there certainly is some form of understanding that large language models have.
They can relate concepts to one another.
And their representations of concepts in a vector space preserves some important parts of the structure of conceptual spaces of our language.

1:03:27 So in this sense, they do understand some things.
Then there are other forms of understanding and about which I will say is something in a moment, but because that's a bit more complicated and I cannot say as much about it, I think.
But the question whether understanding entails consciousness or understanding in the sense you mentioned, I would say, does not entail, does not require consciousness.
So you can have that without consciousness.
And another question is well, does consciousness require some other form of understanding?

1:04:14 Maybe.

1:04:17 Or at least my proposal here would suggest that yes, there is some form of understanding that is required by consciousness.
And this is an understanding which is related to knowing what things in the world some words or representations refer to.
So this requires that you actually have a concept of there being a world of which you are part.
And I don't think that large Lagrange models understand that they are things in the world.
They don't know that there is something out there of which they are a part.

1:05:03 And I think that's crucial for a certain form of understanding.
And in order for certain things to be meaningful for you, you must somehow have a concept of the world and a sense of that you are part of this world and how you relate to things in the world and so on.
Now, this, I think, is required for some form of understanding and I think it's also required for consciousness, at least according to the proposal that I presented here.
And the idea is that if a system not only has some internal representations that it manipulates, but if by virtue of doing so it sustains its existence, then this puts some very strong constraints on what the system will do with these representations.

1:06:15 So if you if you think about a self driving car, then in principle it may compute all sorts of things and it will not have a meaning for the system, for the car itself.

1:06:35 But if these processes are realized in a way that the system's continued existence depends on these computations and this puts some more constraints on what it can do with these internal representations which will give such a system maybe some form of common sense and allowing it to draw certain inferences and avoiding other inferences and so on.
So that would be my hypothesis that there's a certain form of understanding that requires these, that also requires the conditions that I think are necessary for consciousness.

1:07:35 _Daniel:_

In that I hear a shift from semantics and semantic embeddings to true semiosis and the abductive process of generation of embedded meanings.
That's very interesting.
Okay, a few more questions.
One, you've been writing excellent and diverse papers on different mathematical formalisms of consciousness for some years now.
So how have you seen the empirical side and the theoretical side of scientific study of consciousness developing in the last several years?

1:08:18 And how do you believe that the current inflection points in artificial intelligence are like recontextualizing or modifying your agenda or bringing different relevance to your work?

1:08:33 _Wanja:_

Yeah, that's a good question.
And in general, I would say that since the 90s there's been an explosion of empirical work on consciousness, partly also due to certain methods that were and paradigms that were developed and then imaging technology that improved and so on.
So we have better ways of empirically studying consciousness.
And so in the past years, there's been or decades, a lot of empirical data on consciousness has been gathered and many things have been found out.

1:09:20 And I think there are two reasons for which many people are now driven to theoretical approaches again or looking more closely at theoretical approaches.
The first is that data alone doesn't give you understanding, so you need ways of interpreting data and constraining experiments and so on.
And I think some evidence for this is are these recent adversarial collaborations in which proponents of different theories of consciousness team up design experiments that would lead to, or could lead to evidence which more strongly favors one but not the other theory.
And part of why such adversarial collaborations are needed or are perceived as necessary by some is that in previous years people working with certain theoretical assumptions in mind or with their pet theory, maybe global workspace theory, they've been or other theories.

1:10:51 Of course they've then been looking for evidence that would confirm their theoretical assumptions and maybe designing experiments in a way that is more likely to yield certain kinds of evidence or confirming evidence, supporting evidence for their own theoretical assumptions.

1:11:12 So realizing that in order to make progress and constrain also the class of theories that you have, realizing that it's important to do more rigorous experiments and explore ways in which you can actually find also find evidence that disconfirms certain theoretical assumptions.
That I think is one of the motivations behind these adversarial collaborations and also makes people a bit more self conscious of the theoretical assumptions that they're making.
Yeah, then another big issue is, of course, that the scope of empirical and theoretical approaches has to be expanded.
We now have good evidence that many animals that were previously thought to be unconscious actually are conscious.

1:12:16 Animals such as octopuses.

1:12:19 And there's at least reason to take the hypothesis seriously that some insects may also be conscious, maybe bees are conscious.
And in order to make progress here theoretical approaches are needed to help structure debates and determine what kind of evidence would be supportive for certain hypotheses or which type of kinds of evidence would be relevant.
To answer the distribution question which entities, which animals are conscious.
So that's one thing.
And then, of course, you mentioned progress in AI and people are now seriously considering what artificial systems might be conscious and whether some existing systems might actually already be conscious.

1:13:23 And we need theories to make progress on this or maybe not necessarily theories, but theoretical work.
And what I and also, there's a very difficult problem here that artificial systems are in many ways not only unlike human beings, but also unlike other animals.
So whereas in research on animal consciousness you can try and draw some analogies between human beings and other animals, it's less straightforward when it comes to artificial systems and this means that empirical research alone will be less helpful.
We also need very sophisticated theoretical approaches to deal with these issues.

1:14:26 And there will always remain some uncertainty just because artificial systems can be so can be physically or physiologically so different from conscious organisms.

1:14:41 And it's not clear how best to deal with these uncertainties.
We need theoretical approaches to make sense of all this.
And I would say we might face the reality at some point.
So maybe it will turn out that we won't ever know whether certain systems are conscious or not.
I'm very skeptical that we'll someday find a theory of consciousness that will tell us exactly which entities are conscious and which are not.

1:15:24 I mean, integrated information theory is a proposal for such a theory and it's for this reason very important that theories like IIT are being developed.
On the other hand, it makes very ActInf prediction about what kinds of systems can be conscious and which can't.
So it would agree with the proposal I presented here that a computer simulation in a classical hardware will not be conscious and many artificial systems will not be conscious even if they have all the abilities that we that are associated with consciousness, even if they can interact with the environment, have sophisticated cognitive abilities and so on.
So it's very important that such theories are developed.

1:16:30 But I think it's also very hard to gain certainty.

1:16:35 And maybe so.
This is one strategy that I'm pursuing is to try and find necessary conditions for consciousness which would allow us to rule out that certain systems are conscious.
So maybe we will never have a theory of consciousness that says with certainty if a system, an artificial system has x or X-Y-Z and so on, then it is conscious.
But maybe we will have some theoretical approaches that are empirically informed and which strongly suggests that if a system does not have X, then it is not conscious.
So maybe this will be all that we can hope to achieve when it comes to understanding artificial consciousness.

1:17:32 And I see the account that I'm presenting here as contributing to this project by proposing some necessary conditions for consciousness.
And as I already indicated, I'm not completely certain about either of these conditions.
But maybe something like the weaker condition, the flow condition, maybe that would something like that could be a useful, necessary condition for consciousness, which would rule out consciousness in a wide class of systems, but which would, for example, not rule out the possibility of consciousness in a computer simulation.
Not in all computer simulations.

1:18:25 _Daniel:_

Awesome.
The via negativa of consciousness studies.

1:18:31 So one question on measurement and then a closing question on ethics.
So you mentioned the distribution question.
What is the distribution of consciousness in our scenario?
What kind of distribution is that?
Is it a z axis?

1:18:51 There's a scalar quantity that is going to summarize the density of some distribution in space like we were doing some kind of topographical map?
Or is that distribution multidimensional?
Are there different dimensions to consciousness?
So to what extent do we even aim for a unidimensional scalar representation, potentially using IIT or other measures?
Or to what extent will we have a plurality of consciousness measures without necessarily like a higher or lower.

1:19:35 _Wanja:_

Thanks.
Yeah, that's a very tough question as you already alluded to.
According to some theories, such as IIT, consciousness does come in degrees, but it varies along a single scale, a degree of consciousness.
And classically, there's also this distinction between the level of consciousness and the contents of consciousness.
Or the level would be defined in terms of wakefulness or vigilance and the contents in terms of that which is experienced.

1:20:21 And the idea would be that you can distinguish between levels of consciousness in a unidimensional way.
But then more recent proposals according to which consciousness is multidimensional and as you already mentioned, which means that it may be impossible to define a unidimensional degree of consciousness, maybe you can only order conscious experiences along these different dimensions individually, but not have a total order on conscious states.

1:21:15 Yeah, so I think these are, to a large extent unresolved questions and I don't have a strong opinion on this, but I do think that consciousness, there are at least some crucial dimensions of consciousness that come in degrees.
And I'm open to the idea that there will be borderline cases between systems that are clearly conscious and systems that are clearly unconscious.
So I'm open to the idea, to the possibility that there will be some systems for which it's indeterminate whether they're conscious or not.
And apart from I, Dean IIT would not imply this, of course, but there some computational approaches to consciousness would specify some properties.

1:22:16 I mean, if you think about the counterfactual depth action, action oriented representation instance, that's something that comes in degrees, and it's not clear at what point a system will be conscious and cease to be unconscious.

1:22:34 What degree of counterfactual depth is necessary for consciousness.

1:22:45 I'm open to the possibility of borderline cases of consciousness.
And similarly, if we try to apply theories of consciousness to other animals, then there may be cases in which it's not clear whether what a theory of consciousness would say.
So Jonathan Birch has a wonderful paper about the problem of trying to determine of finding out which non human animals are consciousness.
And the idea is that if you try to use a theory of consciousness that was developed on the basis of what we know about consciousness in human beings, then there may be many cases in which it's not clear whether the theory applies or not, or whether the conditions for consciousness are fulfilled or not.

1:23:46 So if you think about global workspace theory, what is a global workspace?

1:23:52 We can, for human beings, distinguish between different consuming systems, local processes that have access to the global workspace and which receive the contents that are represented in the workspace and which are thereby consciously processed.
But there are animals that don't have as many cognitive sub processes, that don't have such sophisticated cognitive abilities, that may maybe have something like a global workspace, but with fewer consuming systems.
So when does it cease to be a global workspace in the sense that will be required for consciousness?
And because of such indeterminacy, it may be more useful than to look for other markers of consciousness, evidence for consciousness, such as learning abilities.

1:24:55 That's what Birch proposes, and in part, I think, inspired by work by Yvonne Jablanca and Simona Ginsburg, who suggests that certain forms of learning are transition markers for consciousness, which provides strong evidence for the presence of consciousness.

1:25:19 And yeah, what about the distribution question?
So this is more about evidence for consciousness in different types of systems and what will the distribution look like in the end?
I don't know.
But what I'm mainly interested is in trying to find out how we can determine whether a system is conscious or how we can rule out that a system is conscious and what, in the end, this will tell us about the distribution of consciousness, I think is a great open question.

1:25:58 _Daniel:_

Awesome.
Well, as we say in the ant colony, the whole nest is our workspace.
So different systems will do it differently.
And in closing, I know that you're teaching a course on this, so to compress it will be a challenge.
But could you conclude with a statement, or actually a pair of statements on AI ethics, one addressed to natural humans, one addressed to the machines?

1:26:29 _Wanja:_

Yeah.
So AI ethics so I don't want to say anything about AI ethics in general, but just about consciousness.
So when it comes to human beings what I find interesting is a question what is required for being a moral agent?
So most people would agree that consciousness gives people or gives entities gives organisms at least some moral status even if it's maybe not required for having a moral standing but it's at least sufficient for some form of moral status.
And then maybe some organisms matter more than other organisms even if they are similarly conscious.

1:27:27 But maybe some animals matter more than other animals because of their cognitive abilities and so on.
And then the question is what do we have to add in order to turn a moral patient, as it were, into a moral agent?
A being that can act in ways that are not just in accordance with certain moral principles or not in accordance with them but that can act because of certain moral considerations?
And is it necessary to be conscious in order to be a moral agent?
And what I find interesting here is to explore to what extent accounts that look for necessary conditions for consciousness may also yield some necessary conditions for being a moral agent.

1:28:32 So even if consciousness may not be required for being a moral agent maybe there are certain necessary conditions for consciousness that are also necessary for moral agency.
And this can then also be applied to artificial systems in principle.
But of course, when it comes to artificial systems the interesting question is should we even create artificial systems that might be conscious or do we have a duty to create conscious artificial systems?
And my own position would be that in the case of animals it's already happened.
We may not know with certainty which animals are conscious and which are not.

1:29:32 But regardless of our epistemic situation regardless of what we know about these animals they are conscious or are not conscious.
They feel pain or don't feel pain.
They suffer or they do not suffer.
So the most we can do is to try and minimize the suffering in existing animals.
But when it comes to artificial systems we can at least at the moment say that most artificial systems are very unlikely to be conscious.

1:30:05 And we have the unique opportunity now to really think hard about whether we want to risk creating conscious artificial systems.
And I think we learned at least two things two interesting things in the past weeks or months about artificial systems artificial intelligence and consciousness.
And one is that AGI may not require consciousness.
I think most people believe that anyway.
But there was at least a possibility that AGI artificial general intelligence might require consciousness.

1:30:53 And what we've seen with the latest generations of language models is that they at least come very close to some form of artificial general intelligence and it's very unlikely that they're conscious.
And so this gives me at least some confidence that future, more sophisticated systems that will have a general form of intelligence will also not be conscious or unlikely to be conscious.
And I think that's good because it will not there will be no further incentive to create artificial conscious systems in order to achieve AGI, because it seems that you can achieve that without creating conscious systems.
Another thing which is a bit more concerning, maybe, is that we've also seen that it's very difficult to regulate developments in AI, and big companies can just decide to put systems on the market and make them available for everyone, and they will use them for whatever purposes without any regulation.

1:32:21 And so if it will, in the maybe not too far future, be feasible to create conscious systems, if we do gain a better understanding of what it would mean for an artificial system to be conscious or maybe how to create one, people will do it and it will be very difficult to regulate this.

1:32:49 So this may be a problem for the not too far future.

1:32:59 _Daniel:_

A problem for guest stream number 40.2.

1:33:03 _Wanja:_

Yes.

1:33:05 _Daniel:_

Thank you, Wanja.
Very insightful.
Best of luck with your works and hope to talk to you later.

1:33:12 _Wanja:_

Thank you, Daniel.
It's been a pleasure.

1:33:15 _Daniel:_

Very well.

1:33:17 _Wanja:_

Bye, you.
