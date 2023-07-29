00:07 _Daniel Friedman:_
Hello, it's July 28, 2023, and we're in active inference textbook group Slash Bookstream 2.02.
Thanks Ali, for joining.
So what we're going to do today is give a short overview of the chapters from the par at all 2022 book.
We're going to do chapters four, five, seven, and eight, and we're just going to pause between them because then we'll clip them into the shorter videos, append that to the playlist.
Just so there's a first video overview of each of the chapters and this is the second in that work.
All right, so we'll do chapter four.
We'll just wait a few seconds and then start chapter four.
Okay, chapter four is called Degenerative Models of Active Inference, and it begins with a quotation, everything should be made as simple as possible, but not simpler by Albert Einstein.
Ali, what is your overview, thought or warning for chapter four?

01:25 _Ali Rahmjoo:_
Okay, so after the preliminary materials in chapters two and three, which was basically largely based on providing some conceptual framework for developing the further theory, chapter four delves into much more detail in terms of mathematical formulation.
And it unpacks a lot more the way that the central equations of active inference is derived and how to construct the important elements of active inference models.
So say matrices A-B-C and D, and also how to put together generative models in different situations.
So it basically lays out the foundation constructing active inference models both for discrete time situations and continuous time ones, which will be used later in chapters seven and eight.
But this is probably one of the most challenging and at least mathematically dense chapters in the book.
So I would personally suggest reading through this chapter really slowly.
And even if we don't get to understand every single detail of the chapter, obviously we can return required as we go through the textbook.

03:14 _Daniel:_
Thank you, Ali.
Yes.
So let's look through the sections.
Just to add on, though, chapter four is one of the larger and more equation dense chapters because it is the common kernel or basis that's then going to get applied in chapter five.
In the Neurobiological case, there's a recipe for making chapter four in chapter six.
That's the recipe for active inference modeling.
Chapter seven and eight are about the discrete and the continuous time variant or subtype or motif of these kinds of things called generative models.
So this is the real common route and we'll just look at what the sections are.
This chapter complements the preceding chapter's conceptual treatment of active inference with a more formal treatment.
Section 4.2 from Bayesian inference to free energy.
What would you say about this section, Ali?

04:18 _Ali:_
Okay, so as we know, the free energy principle is inspired by previous work on Bayesian inference, I mean all the way back to Helmholt's theory about unconscious inference or something to that effect.
I can't remember the exact term, but here it provides in a bit more detail how we can derive free energy principle formalism using the established Bayesian inference formulation.
And particularly one of the key movements or at least one of the key decisions through the derivation of free energy principle formulation is using Jane's inequality principle to derive an upper bound instead of just using the exact values to compute or to achieve the required parameters.
So that's basically, in my opinion, the key premise of section 4.2 and to see in a bit more detail how we can achieve those upper bounds using Jane's inequality directly by using manipulations of Bayesian statistical formalism.

06:05 _Daniel:_
Thanks.
I'll just add one point from this section broadly.
These are the problems of inferring states of the world perception and inferring a course of action planning.
So this is again referring to the perception and everything that happens in between is the internal or the cognitive part of the inference.
But this is like the blanket state cybernetic input output.
And then let's look at the first equation or how much equations overall or what equations do you think we should highlight?

06:42 _Ali:_
Okay, just as a general comment about these different equations.
Well, each of these equations provide a distinct step toward deriving the ultimate whole picture.
So even if we don't quite understand how we can derive from each step to the other one, it's good to know that it's only required to understand how we get to that ultimate whole picture.
But ultimately what we would need in order to develop active inference models is the ultimate equation or ultimate whole picture.
So this is just a way to elucidate the steps toward developing that whole picture.
But again, it's not an essential requirement to understand the materials of the rest of the book.
But if we go from equations 4.1 toward the 4.4 or other words, a variational free energy, well, equation 4.1 is just a basic definition of some properties of probabilities in terms of conditional probability and so on.
So equation 4.2 provides the central Jane's inequality principle and how it relates to conditional probabilities and of course joint probabilities.
And then by using those two properties or those two equations, we ultimately get to 4.4, which is the definition of variation free energy parameter, which is the parameter of interest that needs to be optimized in order to inference to happen or at least perceptual inference to happen in active inference models.

09:13 _Daniel:_
Thanks.
Only thing I'll add is F is the letter used for variational free energy.
Think of it like a computer program and the arguments that it takes in or the variables that it takes in are q, which is the distribution that's under the statistician's control and Y, which are the data which are outside of the statistician's control.
And do you want to describe more about anything in this equation or carry on?

09:46 _Ali:_
Just one thing that can probably be helpful is to somehow compare these steps with the initial picture we had from chapter two because variation free energy was first introduced in chapter two.
So it can be helpful to go back and forth between chapters two and four and try to connect the dots between the related points there.

10:24 _Daniel:_
Section 4.3 generative Models all right, I'll read the first sentence, then you can give some thoughts.
To calculate the free energy, we need three things data, a family of variational distributions and a generative model comprising a prior and a likelihood.
In this section, we outlined two very general sorts of generative model used for active inference and the form the free energy takes in relation to each.

11:01 _Ali:_
Okay, so as mentioned earlier, this chapter deals both with discrete time and continuous time situations.
So clearly we would need two different types of generative models for each situation.
And obviously the generative models or the way to construct generative models for discrete time situations would vary quite a bit from the one for continuous time situations.
But the general principle underlying those generative models are basically the same, which is to somehow construct a model of the environment, either be it for the situation that is sequential in time or for the situations that need to be somehow each moment of the situation needs to be accommodated in terms of a continuous time situation.
So Figure 4.2 provides some examples of both.
Let me see.
Yes, so we have some examples of different kinds of generative models, some case studies if you like.
And it provides various ways to show how the dependencies between variables can be modeled using these kinds of graphical probabilistic models.
So one common way to represent generative models is to use these kinds of graphical probabilistic models in active inference literature, which is at least in this case, the circles would represent the random variables and the squares would represent the distributions, which would describe the dependencies between those random variables.
So we can see the clear relationships between those parameters here, which is basically what this whole graph, what constitutes the generative model that needs to be used for different situations.
And then in Figure 4.3, we can compare the two different types of generative models based on whether it's discrete time or continuous time situations.
So the upper picture is a generative model for the discrete time situation and the lower picture is the parallel continuous time version of it.
And as we can see, the general topology of these models are the same.
The only things that differ is the use of parameters for policies or I mean, discrete time policies or the continuous time ones.
And we can obviously compare the different elements for both priors states and external states, internal states and so on by comparing these two models here.

14:52 _Daniel:_
Yeah, we often return to Figure 4.3.
It's kind of the Rosetta Stone of generative modeling for the context of this book because it's then going to develop out into chapter seven and eight.
And it represents a really fundamental decision made in modeling and in the later chapters.
It's also shown how it can be made into a hierarchical model that combines aspects of both, but within each level of modeling still, these are the kinds of decisions that modelers are presented with when it comes to statistical modeling overall.
So Section 4.4 goes into essentially the top half of Figure 4.3 discrete time.
What would you say about discrete time?

15:43 _Ali:_
Okay, so the discrete time situation is obviously the archetype discrete time situation, which is the Palm DP models.
So at this point I would very much like to recommend following the material from step by step paper, because in that paper, the way to construct Palm DP models is described in a bit more detail.
So if anyone feels like they should learn a bit more about the gaps in the details, I would very much like to recommend that particular paper.
I don't know how much detail we should go into because although it's not maybe detailed enough for some tastes, but it goes in a quite extensive detail about how we can construct these models using the concepts we've learned in previous chapters.
So ultimately we reach equations 4.13 and 4.14, which are basically the culmination of Palm DP formulation using the vector notations and gradients and so on.
Then we go to continuous time situation.

17:30 _Daniel:_
Great.
A few things intervene in the continuous time chapter ones that we'll just mention here because they're kind of boxed or partitioned from the continuous time part, but they're following pages versus Markov blankets.
We won't go into it here, but kind of footnote that or look at some other places where we talk about it outside of this chapter.
Overview figure 4.4 Bayesian message passing.
Again, a big topic.
Let's kind of just go past it now back to the regularly scheduled continuous time generative model discussion.
And then another box to the generalized coordinates of motion.
So taking position plus derivatives of position.
And that has some beneficial properties that are described and unpacked also elsewhere.
Do you want to say anything about 4.5.2?

18:40 _Ali:_
Well, the only thing that comes to mind is although as I said before, all the formulations here may look more, I mean, a bit too dense to understand at the first pass.
But some of the key maybe components here could be obviously the material from box 4.2 and 4.3 I think are quite essential to understand the underlying principle behind deriving the continuous time situation because without LaPlace approximation, what we would have in terms of free energy minimization is it would look very much like the Gibbs free energy.
The key distinction between the free energy principle as described in active inference literature, as opposed to Gibbs free energy is this distinction, is the LaPlace approximation.
So this is what enables us to go from Gibbs free energy to the variation of free energy.
So yeah, that's quite essential to make this to be familiar with this essential approximation.
And obviously the concept of generalized coordinates of motion will come time and time again throughout the whole book, particularly in chapters eight and nine.
So, yeah, those two concepts, I believe, needs a bit more attention.

20:42 _Daniel:_
Yeah, sounds good.
Box 4.3 LaPlace approximation equations, another message passing, representation, and a summary.
The key message to take away is that approximate Bayesian inference may be framed as minimizing a quantity known as variational free energy.
This depends on a generative model that expresses our belief about how data are generated.
Anything else you want to add?

21:15 _Ali:_
Ah, nothing comes to mind at the moment because, as I said, we're still in the stage that we want to develop our essential tools to be used in the rest of the book.
So here, up until now, I believe by the end of chapter four, we have acquired all the essential, necessary mathematical tools.
And the next chapter, chapter five, kind of acts like an interlude, and I don't think it's the direct continuation of chapters one through four.
So I believe the first part of the book, conceptually and mathematically, ends here.
So, yeah, that's it.

22:14 _Daniel:_
Yes, it's a little bit like the Pragmatic modeling part gets foreshadowed or explored in five now that we're all built up with four.
All right, that's the end of the overview for 14.
Chapter five is called Message Passing and Neurobiology.
What is your overview thought on chapter five?

22:54 _Ali:_
Okay, I don't know.
I have mixed feelings about this chapter because on one hand, you see, as far as I understand active inference, although it originated as, quote unquote, a unified theory of the brain, I don't think it's a neurobiological theory per se.
Of course, there can be some correlations between neurobiological components or concepts with active inference concepts, but it's not an essential premise of active inference theory to provide a comprehensive theory about how the neurobiology of human brain or other organisms brain behave at detailed and neuroanatomical anatomical level.
But then again, it's nice to have these kinds of empirical correlations between the findings of neurobiology and the active inference theory.
But I don't think it's one of active inference central assertions, at least to my understanding.

24:29 _Daniel:_
Well said.
Very interesting framing.
Well, chapter five definitely takes a very specific system of interest approach by highlighting one of the most studied areas, also one of the most relevant areas, which is mammalian neuroscience.
And the chapter is going to introduce a few different motifs in the nervous system and essentially build up towards figure 5.5, which is at the end of the chapter, and 5.5 wires together three specific neural systems that the chapter is going to focus on work in that area from.
So Ali said it very well, active inference was built up to in chapter four.
Here is another level or type of science with assertions or with representations or mappings to any specific system.
But this is the kind of modeling that has been built up and done by Friston Parr Pazulo and others over the decades, with a focus coming from a human neuroimaging laboratory setting a lot of focus and study and attention and funding and everything on the mammalian nervous system.
But claims about the nervous system are not the basis of what active inference claims or how it's derived.
But this is like an example case study in neurobiology connecting back to some of the formalisms that we've just seen introduced in chapter four.

26:24 _Ali:_
Yeah, and to add a minor point to what you just said, I think it's important to draw attention to the last sentence of the last paragraph of the first page.
It is important to draw a distinction between a principle I, e.
The minimization of free energy, and a process theory about how this principle may be implemented in a certain kind of system.
So I think this sentence here frames this chapter in relation to all the other technical chapters of this book.
So if every other chapter is about developing, or at least up to now, was about developing the principled formalism of active inference, now, chapter five provides a kind of preliminary sketch for the process theory of active inference, which is obviously far from an extensive theory.
It's just a single chapter.
But then again, it can provide some important signposts for anyone who wants to further investigate this area awesome free energy.

27:41 _Daniel:_
Principle, Bayesian mechanics, all things in that area are, on this principle, not responsive to empirical data.
And then the process theory is about how the principle is implemented.
So the specific generative models that are made and how well they map or how well they do in a portfolio of models that can have very different goals and assumptions and all of this.
But the process theory implementation lets us develop hypotheses that are answerable to empirical data, like what is the kind of information or relationship between photons hitting the retina and changes in activity in neural systems?
And that's an informational question or can be abstracted in a way to an informational question that, it turns out, does have empirical support and results in unique explanations and predictions.
That doesn't mean that it always results in unique explanations and predictions, but a lot of citations are provided here.
That's what we can explore in chapter five.
The last paragraph of the first section describes that they're going to look at the three different neural systems.
Okay, section 5.2, microcircuits and messages.
What do you think, Ali?

29:18 _Ali:_
All right.
This chapter begins from how message passing happens in neurobiological terms and compare it to the way active inference frames this message passing mechanism.
And specifically, if we look at Figure 5.1 and compare this figure to the ones we've seen before in chapters one through four I think it was in chapter four, we can see some clear parallels between how this kind of cortical message passaging happens in the brain versus how it is framed in active inference literature.
And as we can see it's clearly inspired by the neurobiology of the brain.
But then it's important to keep in mind that it's not a direct one to one mapping between these two models.
This is just a kind of, I don't know, an interesting or illuminating, if you like, parallel to keep in mind to somehow be a bit more confident about the viability of the theory we want to use for message passing and active inference.
Which is to say, it's not some haphazard theory that's just been developed for practical reasons.
It has some basis in neurobiology, although it's not necessarily fully congruent with every detail of neurobiology.

31:19 _Daniel:_
Great.
The specific example is going to involve this one region of mammalian cortex tissue that has these six layers, and there's a ton of neurobiology.
The big takeaway for Figure 5.1 is that it's possible to graphically lay out nodes and variables and find some empirical correspondences, again, some unique explanations and predictions in certain cases.
And that's one kind of modeling where it's really trying to understand and improve the ability to do correlation and intervention and counterfactual causal type analysis with the real system of interest.
Or in a more pedagogical setting or in a research setting or an industrial setting, you might sweep across large families of structures of models and there's no need to be grounded to any biological structure at all.
So this is just describing the specific neuroanatomical research that really arose out of the imaging work at UCL and the SPM package.
That's where a lot of this comes from.
5.2.
Yeah, go ahead.

32:36 _Ali:_
Sorry.
Just as a side note, I think watching one of Thomas Parr's lectures on neurobiology of active inference, which is available on YouTube, would really help to understand the materials of this chapter better.
So I highly recommend watching that one.

32:55 _Daniel:_
Thanks.
Figure 5.2 gives a rerendering of a kind of classical view of a hierarchical predictive coding system works.
So here abstracting a layer from the tissue six layer to just two layers.
Here computational layers now and then showing how there's hierarchical communication within a layer, but also there's signaling within a layer.
And there's a hierarchy in Bayesian modeling with variables that are higher order predictions about other variables.
And that's the basis of the predictive coding architecture.
So 5.2 looks at some ways that something that resonates with the cerebral cortical architecture enables what might computationally look like or have some really strong and explanatory values in actually relating to computationally a hierarchical Bayesian model which could do various general tasks.
All right, 5.3 is motor commands leaving the prefrontal cortex, going down to the butterfly looking cross section here.
What is 5.3?

34:30 _Ali:_
Okay, so 5.3 moves to the other half of active inference framework, which is how it can model the decision making and ultimately the movement of the agent in order to minimize the expected free energy as opposed to variational free energy that we saw in perceptual half of active inference.
So it again provides a kind of correlation or analogy between the structural neuroanatomy particularly related to the motor commands and how it can relates to active inference, particularly the continuous time active inference.
So we can see that for the external event or, I'm sorry, for the external state, we can take, for example, the proprioceptive afferent.
And then this proprioceptive afferent acts as a kind of y for the continuous time active inference which needs to be processed in a way to optimize the expected free energy and how it relates to both attention and precision.
We will see a bit more detail about those terms and the relation between them in chapter eight.
But I think here Section 5.3 provides a good summary about the general paths through the motor command systems of neurobiology.

36:34 _Daniel:_
Great.
I'd say.
While the previous case study focused on how the connectivity within and between the Cortical columns could have a computational relationship with a Bayesian hierarchical predictive coding architecture.
The argument of the second case study is that a continuous input, continuous output kind of set point seeking, reflexive motor behavior with a moving set point with a descending moving set point enabling motion by changing ultimately the set point and enabling variation in the strategies to reach that set point through different mechanisms.
This is also describable in a compatible way that's a shorter section.
Now, section 5.4 subcortical structures.
What would you say about this section?

37:41 _Ali:_
Okay, so subcortical structures are very important in the decision making and the planning of the agents.
So obviously here we need another kind of analogy between the way that these plannings and decision making happen neuroanatomically with the way that it's framed in active inference.
But again, we can see it's clearly based on at least some of the important elements we've seen from the previous chapters.
So for example, we saw how policy is described or how it relates to outcomes and preference and so on.
We can see those elements are directly inspired by neuroanatomical structures.
So I guess that's at least in my opinion, this section here 5.4 seems a bit more sketchy in the meaning that it doesn't go into quite the extensive details about how those structures can be compared.
But for anyone who wants to further investigate these topics, there are some useful references put on here on pages 93 and 94.

39:39 _Daniel:_
Thanks.
Yeah, it's really abbreviated and overviewed but we get an interlude from Table 5.1 with putative roles of neurotransmitters.
So same perspective that we took before on neuroanatomical functionalism here directly translates to neurotransmitters reductionism or essentialism or something like that.
So certainly all neurotransmitters and molecules, they play variable roles in different settings and this is the neat and Scruffy manifold all over again.
One person might say well, we need a theory for every acetylcholine molecule in the world.
They're all in a unique context.
And someone else says all neurotransmitters are described by one parameter.
In this model I'm getting value from it.
So to me, that's an account.
And somewhere in between is the work in this space, which is making an attempt to have a principled and falsifiable approach to model the computational aspects of specific regions and contexts and settings.
And so Acetylcholine, Noradrenaline, Dopamine, and Serotonin are given a little mini review here.
And so it's not an exhaustive or an exclusive claim.
It's kind of a provocation from computational and molecular neuroscience, and people can look into the papers and also ones that probably have been published since.
5.6 goes to Continuous and Discrete Hierarchies, which is graphically overviewed in Figure 5.5.
So what would you say about this?

41:31 _Ali:_
Yeah, one interesting thing about this section is the observation that our lower level engagement with the environment can be most successfully characterized with continuous time formulations.
But as we go up on the level of cognitive concepts or at the level of cognitive hierarchies and we come to concepts such as, I don't know, decisions or even beliefs and so on, we can reach the area that the discrete time situation would probably be more efficient to characterize the behavior of the agent.
So this multiscale structure of active inference modeling is quite evident in the way that our message passing happens in our brain in terms of our lower level data processing up into consolidating the higher level cognitive concepts and ontologies awesome.

42:52 _Daniel:_
Thank you.
To me, Figure 5.5 demonstrates the kind of whole of body approach that you could imagine.
There's so many organs and systems and phenomena for which there aren't specific generative models.
So little can be said about situations where no generative model has been articulated, and here's one where it has.
So it gives you also it's kind of like reading a Drosophila.
Melanogaster review paper relatively.
It's like, this is how much work it takes to get to this state of knowledge in an insect.
So then in another insect, do we know less about that insect empirically and genetically?
So consider this to be what's known to be a lot, however, also about one of the most sophisticated or specific cognitive systems at least we know.
So there's that additional kind of like, self reflexive aspect to this chapter that is not a cornerstone of active inference, but here it's just presented in a synthetic case study.
Anything else you want to say about five?

44:02 _Ali:_
Nothing particular comes to mind.

44:05 _Daniel:_
All right.
Okay.
Chapter seven is called Active Inference and Discrete Time.
Chapter seven is the first in a pair of chapters with chapter eight on Discrete and Continuous Time.
So they're kind of like two forks of a river that we discussed in chapter four and before and described the recipe in chapter six.
Now, seven and eight are kind of like one level deeper, going from the kind of all of this group of animals to one level deeper into its classification scheme on the way to the specific generative model for which it's actually given in its totality.
But everything prior to that is about the learning about its principles.
And this is kind of on the trunk of the path to discrete time modeling.
Just like chapter eight will be about continuous time modeling.
What would you add in?

45:32 _Ali:_
Okay, so I think chapters seven and eight really helps to understand in a more practical way how the materials from particularly chapters one through five applies in real time situations.
So even if we somehow didn't get to understand every details of chapters one through four, when we come to chapters seven and eight, I think some of those uncertainties about our understandings can be clarified, at least in a practical sense.
So I believe these two chapters are really helpful in order to consolidate our understandings from the previous chapters.

46:29 _Daniel:_
Awesome, well said.
So it's going to involve specifying some discrete time models.
7.2 goes into perceptual processing and the general structure of the chapter is going to walk through a series of examples that build in complexity where they first start with perception in 7.2, introduce decision making and then describe a few more types of motifs or cognitive structure or patterns and also check out step by step and model stream one where it's built up to in a different way.
So the first example is I'll let you describe it since it's musical.

47:16 _Ali:_
Okay.
So yeah, the first example is the situation in which we try to describe the performance of an amateur musician in terms of how we listen to the performance of an amateur musicians in terms of the predictions we get from our anticipation of the following notes as opposed to the actual notes that's being played.
So these kinds of anticipatory reaction listening reaction to the musician can be successfully formalized using discrete time active inference by putting up by putting together the matrices A for the states and matrix B for the transition between the states or the transition probabilities, which in this case describes the probability from going from one note to the other and obviously the actual sequence that's been played which can be described with the matrix d another point I wanted to mention is for anyone who has downloaded this chapter before I don't know, I think about June or something.
I recommend redownloading it from MIT's website because they have corrected some of the typos that was previously present in this chapter, particularly in Figure 7.2.

49:10 _Daniel:_
Cool.
So this graphical model where a person is listening, this is a general perceptual Bayesian framing.
It's specified just like with any other equations.
There's a lot to look into but A indicates the probability of an outcome given a state.
This is saying if it were all on the diagonal like an identity matrix, this is kind of a common motif then states kind of map to themselves.
So in the context of this model, a represents the mapping between the observed note and the underlying hidden true note and then B.
Describes the transition matrix of how those change to time.
D is the prior they're specified.
Figure 7.2, do you want to describe it?

50:15 _Ali:_
All right, so in figure 7.2, or at least the incomplete version of Figure 7.2 we see here well, at the upper left part of the picture we see the beliefs about each note at each time step and at upper right we somehow translate those beliefs into specific numerical values.
So instead of just assigning some continuous values, we've simplified the situation by assigning some discrete numerical values for each node.
And then the lower left is supposed to show the free energy gradients over time or in other terms the prediction errors we get from comparing our predictions with the actual outcomes.
So lastly, the lower right picture shows in parallel to the upper right picture, determines the values of these errors.
So we can see both the initial or at least initial continuous assignment and values and then the further discretizing of the values in order to get the discrete time situation or the more tractable discrete time situations.

52:13 _Daniel:_
Okay, so it's a general passive inference task where there's priors about how states are going to change through time and then there's real data coming in.
So that's the kind of classical predictive coding video compression coleman filter Bayesian setting 7.3 introduces a key motif which is decision making and planning as inference.
So this is the idea of having a Bayes graph where the variables can relate to different things.
There's high composability and here the idea is that a variable is going to be proposed that we can do inference about that describes the process of decision making or policy selection.
So what would you say about 7.3?

53:04 _Ali:_
Okay, so 7.3 is obviously similar to what we saw in chapter four.
And if I'm not mistaken, even the topology is exactly the same with that picture we saw previously.
This is the initial setup which acts also as a review about how these different components of palmdp generative models needs to be described in such situations.
But ultimately the specific case study we come across in this section is the attempt to model the behavior of a mouse in a teammate of a rat and a teammate, especially teammates, containing an aversive stimulus in one arm and an attractive stimulus on the other.
So this can act as a kind of toy example to use this kind of probabilistic modeling to describe these situations.

54:35 _Daniel:_
Thanks.
So that leads us right to figure 7.4.
Here's a visualization of the situation with the rat in this case where there's a pleasant and aversive stimuli on each end of a decision point and there's also an epistemic opportunity to receive some information about the context that the animal is in.
And so that setting is described for both the case with white on the left, black on the right and black on the left, white on the right.
And those are shown in terms of their differences in the matrices.
The explicit specification of the generative model visualizations show some of the slices of the B variable which reflect different transition probabilities.
C represents the preferences which are expressed over the observable states, d reflects the priors on the different states that need priors.
7.4, what would you say about this?

55:59 _Ali:_
Okay, so in 7.4, it builds up on the previous section and adds other elements that we previously saw in chapters two and four, which is how the exact formulation for expected free energy can be used sorry, variation free energy can be used to formulate the trade off between the information seeking, or at least between the epistemic value and information seeking.
So here it uses again that rad example in a bit more extended and elaborate form to formulate the epistemic value of observing a queue in a given location.
And figure 7.7 is a representation of this situation.
But another situation that's been, let me see yeah, in 7.9, another case study discussed here is the situation of the psychotic eye movements because it is something that can be quite successfully described or characterized in terms of information seeking versus the epistemic value.
And the situation here is let me see.
Yeah.
Shown visually in Figure 7.9, which clearly shows how our visual psychotic eye movement can be described in such a way as to kind of trace the trajectory of our eye movement among different regions of the visual space and how the information we gather from a given region can affect the subsequent trajectories of our psychotic eye movements.
That's basically the main premise of this section, I guess.

58:41 _Daniel:_
Nice.
Great.
7.5, what would you say about it?

58:51 _Ali:_
Okay, so 7.5 again adds another dimension to the previous formulations, and this time, we get to update the generative models by learning and the so the generative models for this situation is a bit more complicated than the previous ones because it now needs to account for a mechanism or a way to update the matrices we had before.
So in the previous situations we didn't account for learning per se, but here we directly update our general sorry, the word update can be confusing.
Here we get to somehow improve our generative models to accommodate for these updating accounts.
The situation here or the case study here, which somehow elucidate the way that the learning can be accounted for with these models is again a toy example of a creature in a simple world of black and white tiles which kind of tries to find a path to reach a given destination, a certain destination.
So it is more complicated than the situation we had for the Rat example because it only had simple trajectories that needed to traverse.
But here the creature, or the agent in this case needs to do lots more learning and information seeking and so on.
So all the previous elements is kind of combined in this example and it's a really good example to see how the different components of active inference can be connected to each other.

1:01:35 _Daniel:_
Nice and 76 hierarchical or deep inference.
First, a box 7.3 interlude on structure learning, boxed off topic and a lot to say, but structure learning broadly refers to learning the structure about a model using the same types of methods that you might to do inference on, for example, a more observable sensor data reading, something like that.
This section works towards the idea of nested inference or multiscale modeling.
What would you say about figure 712?

1:02:22 _Ali:_
Okay, so again, this situation is, I think, the most complex situations of this chapter, which builds up from the previous sections.
And this time it adds another layer to accommodate for the inferences that happen in different time steps.
So in this case we have multi time or multiscale inference and learning happening both at the levels of learning and at the levels of information seeking.
So this is represented in figure seven, point twelve, which represents how kind of this fractal generative model can be seen as a component in this multiscale bigger generative or as a kind of leaf in this bigger generative model.
So it can be seen as a lower level inference happening at the leaf level, going up to the hierarchy and influencing sorry, collaborating on the whole process of learning and inference at the higher level.
Yeah, I guess that somehow summarizes this figure.
So if you have anything to add, that's great.

1:04:14 _Daniel:_
It's an example of the composability of generative models.
What we've talked about and had Toby Sinclair Smith describe as as the compositional cognitive cartography and just what kinds of connectors can and can't you do and how can that motif that the discrete time model introduces and then the rest of these features, including action and learning and so on, get layered in on top?
What can you do with that?
713 gives another example.
Do you want to say anything about it or maybe continue on?

1:04:58 _Ali:_
Yeah, so the case study here is the example of linguistic, I mean, language learning through reading.
So not language learning, maybe just what happens sentence comprehension reading.
Yeah, in comprehension.
So what happens when reading in an anticipatory way the words that comes each after the other.
So why this kind of situation can be most successfully characterized with this kind of modeling because it involves different scales of learning and comprehension, both at the level of at the level of somehow observing the letters and then going onto the words and then word groups and so on.
So, yeah, that's really interesting way to again combine all of those elements into a single unified model to see how those different timescales, slow and fast timescales operate together to build this more encompassing model of more encompassing generative model of the situation.

1:06:33 _Daniel:_
Great.
Any closing thoughts on seven?

1:06:40 _Ali:_
Nothing particular now, thanks.

1:06:43 _Daniel:_
All right, next chapter is chapter eight, which is going to go into the continuous time.
It's all right.
Chapter eight is called active inference in continuous time.
Begins with that timeless quote, everything flows, nothing stands still.
So what would you say about chapter eight?

1:07:19 _Ali:_
All right, so this chapter probably is my most favorite chapter in the book because of my own personal interest in, I don't know, process materialism and so on.
Chapter seven acts as a really good starting point for anyone who wants to develop the discrete time situations to model discrete time situations within active inference framework.
But in chapter eight, we kind of get to model a bit more interesting or let's say more involving situations.
And they're not necessarily kind of toy examples we saw at least at the beginning of chapter seven.
So obviously, as the title suggests, this chapter deals with the continuous time situation.
So in that case we'll need to maybe at this point refresh our memory about what continuous time situation involves by reading the relevant parts, reading or reviewing relevant parts of chapter four.
In chapter four, we saw that the generative model for continuous time situation derives from the Edo's Stochastic calculus in terms of putting the whole process into two elements of Stochastic equations, one of which is the actual states, the condition of actual states or the behavior of the actual states.
And the other one is the randomness that we need to account for in each real time continuous time situations.
So that's what we get here in equation 8.1.
And then building up from that equation, it generalizes that equation to involve the functionals of G and F instead of just the single valued functions of GNF.
So then we get to put that into the situation that can be used for describing the behavior of dynamical systems, which is a very well known situation to use these kinds of Stochastic equations.
And it's widely studied how those kinds of dynamics can be characterized, especially in recent Bayesian mechanics paper by Dalton Saktivetevel and others.
And then it gets to some more specific examples such as Lotgobal Terra dynamics and synchronicity and so on, in order to show how these kinds of dynamics can be elaborated upon and can be generalized and enables them to characterize more complex situations.
That's a really short and brief overview of the whole chapter.
Maybe we can talk about a bit more details as we go through it.

1:11:28 _Daniel:_
Great, well said.
Well, I'm sure for another day the philosophical implications of eight, Seven and Eight and High Road and Low Road and all these other parts of the textbook.
Great topics.
I agree.
I would see chapter eight as demonstrating continuity with some classical continuous time modeling motifs from a few different areas of dynamical systems science, which is applied in many, many fields.
But these are some classic examples.
So figure 8.1 goes a little bit more into depth or at least into more formalism detail about exactly what we saw in chapter five with the spinal reflex arc with the proprioceptive data coming in and then a differential being calculated with the set point which reflects a descending prediction from a decision making layer.
And that can be viewed as this kind of mechanics that plays out in a phase space in continuous time, like a spring moving around with someone making a certain path within a tractor and a spring being dragged around something in that area.
Box 8.1 goes into a very fascinating topic.
Do you want to describe it?

1:12:53 _Ali:_
Well, it's maybe one of the most thought provoking pages of the whole book.
And if I remember correctly, in all of the cohorts, this particular box always gives rise to lots of questions because of some of the interesting and at least initially counterintuitive claims here.
But I don't want to spoil it.
But as a kind of spoiler alert, it kind of gets to really interesting, but alas, very brief discussion about the comparing these terms precision, attention and sensory attenuation and the relation and similarities and difference between these three terms and how understanding each of them is essential to understanding the other ones.
But as I said, it's a really interesting topic which gives rise to lots of discussions and I believe it's one of those topics that's worth looking a bit more looking into in some other literature as well.

1:14:32 _Daniel:_
Great.
Well said.
What a cliffhanger.
Next they go to a classic model family called Lockable Terra.
These dynamics inherit from characterizations of predator prey dynamics in ecology.
So it's kind of a classical ecology model shown in Figure 8.2 on the top.
It's actually the ecosystem model plants, herbivores and carnivores which follow different kinds of oscillatory trends in continuous time.
And so that also has enabled it to be applied for other so called winnerless competitions.
And that relates to topics like neural Darwinism and also neural dynamics where things have kind of oscillatory relationships with each other which are being modeled as a continuous time underlying process with a lot of measurement, noise and discretization through space and time.
Those are the kinds of algorithms that SPM explores more and there's lock of Voltera and a lot of other dynamical systems theory in SPM.
So active inference kind of adds action and more to what was laid out from a pure dynamical systems theory in SPM.

1:15:48 _Ali:_
Here.

1:15:49 _Daniel:_
It really is just showing the ecology example and how you can project if you have three different species, you can think about that motion in a cube or tetrahedron, and then you could project onto kind of like looking at a lower dimensional manifold relating just two of the three species.
And that evinces this kind of oscillatory but also moving behavior that gets connected in Figure 8.3 to neurobiology.
What would you say about this?

1:16:26 _Ali:_
Okay, so here in Figure 8.3 we see some applications of a lot of altera dynamics.
So the left column here represents what happens in eye blink conditioning.
So of course here we need to account for the expected states of the sequences of events that happens in the eye blinking.
So the upper left figure shows the expectations in terms of time.
And then the parallel right hand side equation, sorry, right hand side figures shows the Lotka volterra systems that is applied in the handwriting situation.
So, as we can see, although the mathematical technology is the same, or at least the modeling technology is the same, the outcome of each situation varies drastically in two distinct two distinct neurobiological behavior, not neurobiological, but biological behavior.
So, yeah, we can see how the same modeling framework can give rise to different outcomes based on what parameters needs to be optimized, what parameters are selected for the modeling, and so on.
So I believe it's a quite interesting example to compare handwriting and a blinking together and how those can be compared to each other using the lotkobal thermodynamics great.

1:18:50 _Daniel:_
Thank you.
Box 8.2 gives a variant on the learning here presented with the formalism for continuous models.
Kind of a technical aside, section 8.4 is about generalized synchrony.
So figure 8.4 is going to visualize one of the classic dynamical systems, which is the Lorenz attractor.
So what would you say about this figure?

1:19:16 _Ali:_
Okay, so this section is truly interesting because when one thinks of active inference, probably the first situations that comes to mind is the situations in which we have quite well defined probability distributions for different parameters.
But as we can see here in Section 8.4, actually some of the formalism of active inference can be successfully used to characterize even chaotic systems, and in particular the way in which two chaotic systems can be synchronized with each other.
So this is a classic example of chaotic Lorentz system and it draws upon from some of Professor Prison's earlier work on birdsong synchrony.
And as a side note, any literature before 2016 is considered earlier history in active inference literature because it evolves quite rapidly.
This kind of synchrony between two chaotic systems can be interpreted as providing evidence or even, let's say, a way to model a kind of primitive theory of mind, in the sense that how exactly can we understand or two agents can trace each other's trajectories without any I mean, engaging in any direct exchange of observations between their internal and external states.
So, yeah, that's a really good example, and I believe one of the most interesting examples of how active inference can even account for these kinds of behavior.
And the rest of the section goes into the details of how this kind of synchrony between multiscale Lorentz systems can happen and how can we formulate it mathematically in terms of continuous time active inference.

1:22:04 _Daniel:_
Awesome.
And there's been more recent work on Markov Blankets and Stochastic chaos.
But the Bird example is a classic 8.5 goes into hybrid discrete and continuous models.
So this could be kind of like an in between chapter of seven and eight.
But now that we've been introduced to the pure form of discrete and the pure form of continuous models here shown that that composability extends to so called hybrid models where here the lower level visually is using the continuous time formalism and the higher level is describing a little line added here, the discrete time formalism.
And this was the similar structure described by the authors of the paper.
Active inference does not contradict folk psychology where they described this lower level as motor active inference which was closely allied with the spinal arc reflex shown above.
And then this higher level they called decision active inference because in that case it was referring to a discrete decision.
And so they used that kind of basic motif of continuous activity or continuous time modeling at the more peripheral aspects of a cognitive entity and like Ali said, more discretization and hybridization as well at higher levels of the cognitive modeling.
And that type of an architecture here, instead of describing who wants the ice cream cone, I believe here it's going to be a mixed or a hybrid model that is going to call back the Icicade system where there's a fixed point that is able to be moved as a set point, and then there's a continuous time icicade that pursues the new fixed point.
And so that's analogous to a new set point or fixed point being specified from the top down muscle command about a new location for a muscle followed by movement towards it.
This is a muscular activity that is realizing that but not in the elbow coming away from the hot stove.
This is about the eye circading to an epistemic foraging location specified by top down hierarchical systems.
8.3 describes little technical aside on mixture of Gaussian gaussian mixture models, kind of a technical modeling note.
And 8.6 closes it says it's a huge topic and much has been left out.
And so they list in Table 8.1 key advances in continuous time models.
And those areas are synthetic birdsong, ocular, motor delays, conditioned reflexes, smooth pursuit, eye movements, psychosis illusions, cicades action, observation attention, hybrid models and self organization.
And that's chapter eight.
What else would you say?
And also what would you kind of lead someone to in the philosophical implications of eight?
Because it sounds kind of cool.

1:25:34 _Ali:_
Okay, well, the case of continuous time active inference, I think it leads to really interesting questions both in terms of philosophical questions and also more practical modeling questions about what parameters needs to be accounted for and so on.
And as I said, I believe it's a more interesting way of it's not interesting, but at least more involved way of doing active inference modeling.
But one thing that one of the philosophical questions that Mahault and I have explored in our paper is how the processes, ontological processes can philosophically described using FEP assertions in terms of their intraaction with the environment in which they co constitute themselves.
And we don't necessarily distinguish between the internal and the external states.
So one obvious example of this is that generalized synchrony example that we saw in this chapter in which we don't necessarily distinguish between which of the birds act as the agent and which one is the environment or the vice versa.
So these kind of co constitution of the environment and the agent which gives rise to the partitioning of state space through markup blanket is one of the interesting philosophical points that I think needs to be elaborated a bit.
More using some of the recent advances in philosophy, such as the tools that's been developed in New Materialism School or some other philosophical approaches.
But yeah, these kinds of what exactly gives rise to emergence?
What is the ontological status of emergent properties and so on, are some of the burning questions for many philosophers today.
And I believe active inference, and particularly continuous time active inference, provides a clear, precise mathematical formalism, even if not to answer these questions, but at least to explore it in a more rigorous and practical way, and also practical and attractable way.
So this is the area that I believe philosophy and science are beautifully intertwined into a coherent view of not only the phenomena of interest, but even about the whole world.

1:29:17 _Daniel:_
Wow.

1:29:21 _Ali:_
Pretty cool.

1:29:22 _Daniel:_
Yeah.
A lot to say about that topic.
After completing chapters seven and eight, you've seen the kind of two major branches or two major motifs of just one kind of modeling.
But these kind of models have so many different forms that that's why it's such a hands on process to specify the generative model in chapter six and fit it with data in chapter nine.
Those are all what's required.
And that's kind of the last mile of where these discussions about general motifs gets you.
But also playing with these pedagogical models can be really helpful because it will help you understand the basic patterns and relationships and start to see different patterns in the graphical models and know from there what levels of technical processes can be kind of coarse grained over.
All right.
Okay.
Well, that's it.
I guess next time we will do probably 910 and maybe something else.
All right, I'll end it now.
Thanks, Ali.

1:30:41 _Ali:_
Thank you.
Bye.