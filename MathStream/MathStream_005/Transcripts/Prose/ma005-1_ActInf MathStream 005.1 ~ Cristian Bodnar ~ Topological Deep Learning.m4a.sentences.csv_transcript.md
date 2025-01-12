
00:05 _Daniel:_
Hello and welcome.
It's July 17, 2023.
We're here in Active Inference math stream number 5.1 with Chris Bodnar on topological deep learning graphs, complexes, and sheaves.
So thank you for joining, Chris.
Looking forward to your presentation and discussion.

00:25 _Chris:_
Yeah, thanks so for having me.
So, yeah, as I was just saying, this is my PhD thesis, which I finished a couple of months ago.
It's also kind of public online.
So if you want to go into the details, just kind of look this up on the Internet and you should be able to find it easily.
Obviously, there's lots of stuff in there.
So I kind of try to give an overview today and maybe also go in a little bit more detail in certain aspects since there's not a lot of time to go through.
Yeah, now I'm Microsoft Research, so this is basically all work that I did in the past and when I was at University of Cambridge.
All right, so let's get started.
Right, so let's start very easily.
Now, I'm actually not sure exactly what's kind of the background of the people who are watching, but in machine learning there's all these kind of subfield that emerged a few years ago which is called geometric deep learning, which is essentially looking at how to apply these kind of deep learning.
Neural network architectures on data, living on all sorts of structures or geometries or spaces if you want.
And this has a lot of application, especially in the life sciences.
And there's kind of been a lot of instances of this in kind of very famous publications, some of which you see here.
But just to give some examples, for instance, if you have proteins or molecules or things like that, they usually represented as graphs.
And you kind of have some data living on these graphs, like kind of the properties of certain atoms and so on.
So these kind of things and so far, these kind of spaces or these kind of problems, learning problems, if you want, they have been approached mostly kind of with a geometrical mindset, as the kind of name of this subfield also mentions.
But something that I would argue is that geometry is not everything that you need and there's kind of other non geometrical aspects when you are in such a setting.
And this is kind of quite obvious once you realize that the spaces that kind of show up in the field and in many applications, they are very heterogeneous.
So, as I mentioned, for instance, you could have graphs that could represent anything.
In this case, it's the caffeine molecule that you see here on the left.
And you want to have some models that predict certain properties of this molecule and so on.
But for instance, you can have grids.
And we see grids all the time and data living on grids.
And I'm referring to images, videos, they are all kind of pixels living on a grid.
And then you can have more sophisticated things.
You could have some meshes, for instance.
They're all over in computer graphics and then you could have some sort of manifold.
So for instance, if you're doing maybe weather modeling or something, we live on a sphere, topologically speaking.
So you might want to model your data as living on a sphere and so on.
But nonetheless, even if these spaces are kind of geometrically, kind of heterogeneous, and some of them don't even have a geometrical structure in kind of a strict mathematical sense, they all have what's called a topological structure, which is kind of like kind of a weaker kind of structure, but it's kind of more general.
And I'm going to talk a bit in a few seconds about what that means by in general.
When you do kind of mathematical physics, you kind of have a ladder of structures where you kind of keep building on top and the more structure you have, the more sophisticated things you can do and so on.
And kind of at the base of this diagram just have sets, just kind of a collection of elements with no kind of extra structure and then you kind of keep going up in this ladder and you add stuff on top of sets and so on.
And as I was saying, kind of most of the work is kind of focused on maybe the top levels of this hierarchy, but it's kind of topological level, which are kind of the weakest kind of level you can add on top of sets has kind of been neglected to a large extent.
And part of what I've been doing in my PhD thesis was essentially looking at these kind of learning problems on these kind of spaces from a more topological perspective and kind of try to fill in these blanks.
So this is kind of the overview, okay, so if we are to adopt this topological perspective, what would that actually mean or how would that look like?
I guess it could look in different ways, but in what I've done, in my cases, it looks kind of like this.
So we have horizontally, we kind of have a space that could be anything.
This is just kind of an abstract space.
It could be a grid or things like we've seen in the previous example and kind of vertically attached to the regions of this space.
We have data.
So data is kind of this vertical component and you kind of see these flags kind of being kind of anchored in these regions.
So that kind of signifies you have some data that's kind of associated with that region.
So that's kind of the high level perspective and I'm going to make that a bit more concrete a bit later.
And there's kind of two essential things about this picture.
A first thing is locality.
So the data is attached to some regions of this space, this topological space, and in that sense it's local, so it's kind of associated with the region.
And maybe to give a concrete example, if you kind of have a temperature sensor somewhere in space, right, you could think of whatever that sensor is measuring is kind of a property of kind of the immediate surrounding around that sensor.
So it's kind of describing some property of a region in space.
So that'll be kind of a concrete example.
And another kind of axiom that we're starting with is that the space has structure.
So the space has kind of, it's kind of made up of various regions and these regions intersect in various ways and that implicitly also makes our data structured because the data is attached to these regions.
So there is kind of some structure in the data.
All right, so that's kind of the picture and actually many of these things relate to category theory.
I'm not going to go in depth into this because it's kind of sophisticated and I'm not an expert myself in category theory, but kind of the high level here is that category theory is kind of a nice way.
To translate between different structure in mathematics and kind of discuss about properties of certain kinds of objects and translate that to some different kinds of objects and find all these kind of relations and connections.
And a concrete example is, for instance, if you want to study some manifolds, some surfaces, you could associate some groups to these surfaces and then any sorts of relations between these kind of surfaces, also translating some relations about these groups or some other algebraic structures.
So you could study these manifolds by doing algebra instead of doing geometry or topology or something else.
So also in this case, it's kind of manifesting the fact that we kind of translate these from spaces to data.
So kind of because we associate the regions in a space, certain kinds of data, this is kind of how this translation manifests in what I've just described in the previous picture.
So you could think of this as some sort of translation or mapping from spaces and regions in that space to kind of data attached to that space.
But yeah, I'm not going to go in a lot of detail into this, but just kind of to keep in the back of your mind that there's this stuff lurking in the background.
All right, so I promise this is the only math definition I'm giving in this talk and then I'll stop.
But just because I'm mentioning topological spaces quite often, I just wanted to kind of give this axiomatic definition, which might sound sophisticated, but I have a picture at the end and hopefully it'll be clear what is it.
So it's just a set.
As I was saying, we start with sets and we put stuff on top, right?
So you start with a set and then you also have a collection of subsets of this set called the open sets that need to satisfy certain axioms.
So you could think of these open sets as kind of regions of this space, very informally speaking.
So something that kind of has to be satisfied is that, well, the empty set and the set itself need to be open set.
So in some sense, you could think of this as saying the set itself is a region of that space very informally, which it's kind of, let's say, obvious.
And then there's some kind of constraints about intersecting and taking units of this region.
So if we take the intersection of two regions, we should get another one of these regions.
And if we take a union of these regions, we should get another region.
And there are some constraints again, like, okay, how big these intersections should be.
There should be finite intersections, but you could have infinite unions.
But that's a technicality and we can just skip anyways.
But to see a picture so on the left, you just see the set x itself.
And here I've put like a potential neighborhood structure or kind of like open set structure on this space.
So we have an open set U, another open set V.
By this axiom, their intersection should also be an open set.
So you see this intersection in the middle being another open set, and then the set itself is another open set.
So it's just kind of splitting stuff into regions, kind of.
You could think of it like that.
All right, so this is a topological space, and now let's add data, right?
So we mentioned that we have data and then we have a space, and then we add data on top.
So so far we've seen how a topological space looks like.
Now let's add this kind of vertical stuff, these flags that you saw before.
We just put some data on top of these regions.
And if we put data on all the regions of the space, on all the open sets, we get these structures that in categories here, like in algebraic topology, also geometry, they are called presheaves, which sounds very fancy, but all is just kind of a definition of what I was already describing.
Essentially, you have some data for each region.
For instance, for region U, you have this f of U, which is kind of the data attached to region U.
So you could think of f of U, some set with describing the data that lives there in that region.
But there's also an extra thing.
You have some sort of maps going between these kind of pieces of data, and these are called restriction maps.
And why is that?
They provide you a way to kind of zoom in if you want, right?
Like you have the data attached to the whole set x, and then you could think, okay, how do I take this data?
How do I go from this data to data on a smaller region on x?
So it's kind of a way to zoom in on that data, essentially.
And I'm going to show some example in a second.
So these are called pre sheaves.
And just to see an example, our space here is kind of one of the simplest kind of space you could think of.
It's just 1D or horizontal line, right?
Just the real line.
And then you have some regions which are just given by open intervals on the real line.
And then some pieces of data could be functions like continuous functions on those regions.
So here's some sample data on this first interval.
Here's another function on the second interval.
Here's some data on this third interval.
And actually in this case, it happens that all these functions agree on the overlap.
So where these regions overlap, they take the same values and we can actually glue them together in a single function over the entire region.
So this is just an example of a preshief and it's called the preshift of continuous functions.
So our data in this case is continuous functions and the space is just the realign and we put these functions on top of the realign.
But it turns out because of this kind of special property, that we can kind of glue data and we uniquely get some other piece of data, right?
We can take these three pieces.
It's just exactly like a puzzle, right?
We put these things together and we get a fourth thing, which is kind of a single function where we just overlap these functions, right?
And these presheaves that satisfy these kind of properties where you can kind of glue them to get a unique piece of data.
They are called sheaves and basically the preshave of continuous functions is actually a sheep.
So this is kind of a way to formalize data attached to these things.
It's going to get less technical in a second.
So just to give more examples.
So for instance, in this way we could describe data on a sphere.
And let's say if this data is just some vector field on a sphere.
So let's say if this is Earth, right, this could be some wind vector field, right?
Like if we do weather modeling or something, you just have a vector field describing the wind on the surface of Earth, right?
And you might want to do some machine learning on top of this, where this kind of vector field has a sheet structure, and you could think of it as a sheath, because if you have some vector field on the red region, a vector field on the yellow region, I can kind of glue them together uniquely if they overlap.
If they agree on the overlap and we get the vector field on this bigger region.
But something that's quite nice is that even if we have a very different kind of space namely a graph which is very different from a sphere in all points of view, we can still apply the exact same kind of axioms and terminology and kind of definitions and we can have a sheath of our graph.
So in this way we could have, for instance, some features associated to the nodes of the graph, some features associated with the edges of the graph, and there's another node which has its own features and this is actually the exact same thing we have in graph machine learning.
So this is quite nice.
What this kind of topological perspective allows us to do is we kind of have a unified way of thinking, if you want, about very kind of heterogeneous spaces and we can model on all of them data attached to them by using this kind of sheet terminology and other ways as well.
But I'm not going into that in this talk.
All right, so this is kind of an overview of what I've been doing in my thesis.
And just to kind of dive a bit deeper into this, I just wanted to go into one paper that we did at Europe last year.
Yeah.
So this was last year on what's called shift diffusion.
So essentially, how can we use what I've just described to do some useful stuff when doing machine learning on graphs, all right?
And this was a collaboration with Francesco de Giovanni ben Chamberlain pietro Leo, my advisor and Michael Bronstein.
Okay?
So before I dive into this, I just want to give some background in case people are not familiar with this.
So the kind of favorite architecture of people doing machine learning on graphs these days are these things called graph neural networks, which are actually very simple kind of models.
So in the setting you have some features.
So each node in your graph will have some features.
This is what this h vector here denotes.
So it's the vector h associated with node A at layer or time t, whatever.
So you have some features for each of these nodes and what you're doing each of if you're at a certain node, you want to kind of compute a new representation or new features for this node at the next layer.
So essentially are learning representations and what the graph neural networks are doing.
This node will receive a message from all the other nodes that are neighbors with this node.
And this message can also be passed, can use some neural networks in there, but essentially it's some processing of these features of the neighbors and these are aggregated into this message.
So here in Green and then this is passed through some update function that combines the message from the neighbors with the old representation of this node and it gives you a new representation at the next layer.
And this happens for all the nodes, right?
So then you get some new representations for this node and this is one layer and then you kind of keep repeating this for as many layers as you like.
So this is kind of how you do deep learning on graphs.
It's kind of a very simple recipe and most models actually vary in the way they kind of compute these messages and in the way this update function is designed.
But that's kind of the parameters most of these models use.
Otherwise they all kind of respect this framework and work in this kind of particular way.
And to give you maybe an example for why you would want to do this, you might want to do node classification.
This is kind of a classic problem in graph machine learning.
There are others, but I'm just going to talk about this because it's easier.
So you have a graph and this graph has nodes that have different labels.
Here there's just two kinds of labels, this orange and blue.
And you have some edges between these nodes.
And what you want is you want to do this kind of message passing that I was describing to compute some representations for these nodes where you can easily classify the blue and orange nodes.
Now something that's quite interesting is that for many kind of graph neural networks, depending on the properties of these graphs and how these kind of different nodes are connected, their performance might vary quite a lot.
So in particular they're affected by this property called heterophili.
So this is kind of a measure of how much opposites attractive you want, right?
So it has a very simple formula.
Basically you take the number of edges between orange and blue nodes and you divide by the total number of edges, right?
So basically you kind of check how many connections we have in this graph between things that are quite opposite to each other versus connections that are between similar kind of nodes.
So if you have a lot of these kind of heterogeneous connections, then you have very high heterophili.
And it turns out that many graphene networks actually struggle in that setting.
It's very hard to classify things in that setting.
And intuitively you could kind of also figure out why because you could easily apply some kind of reasoning where oh, this node looks a lot like this other node is connected to.
So they kind of must be in the same community if you want or in the same label.
But it's much harder to do that when all things are kind of different from each other and these communities kind of don't form right, even visually.
If you see a graph and it has some nicely clustered communities, it's quite easy to draw a line between those and say, oh, this is a community, is another community.
But if things are very mixed, then it's quite challenging.
And it turns out it's also challenging for these models, not just for kind of our intuition when we would have to do this.
So this is kind of some problem where this topological perspective I was mentioning will be used to do some useful stuff.
Okay?
So coming back to Sheaves on graphs.
And at this point I think you can largely forget what I mentioned in the introduction or if there's something you misunderstood there.
We kind of start from zero bit here, so there's no problem.
So on the left you just have a graph which is kind of the incidence structure of a graph.
I just drawn here the simplest possible graph that has two nodes v and U.
And then there's an edge between them.
So this is just a graph with one edge.
That's all that's going on here.
And I've just represented it by kind of in this kind of incidence structure kind of way, right?
Node v is incident to node e and node u, sorry, edge e and node U is incident to edge e.
So this is just an incident structure and what this kind of triangle symbol is showing is just this incident structure.
It's just a way to symbolize this incidence relation if you want.
Okay, so this is just a graph, right?
And a way we can kind of think of field zone graphs is just mapping this graph structure.
So this is kind of this categorical theory translation.
We translate this graph into something else which looks very similar.
The structure is kind of the same, it's just kind of the meaning of these things change.
So for each node v we have here, this will be a vector space.
So F of v is a vector space.
For each node u we have F of U which is another vector space.
For each edge e we have this Fe which is another vector space.
So all nodes have their own vector spaces and the features associated to those nodes leaving those vector spaces.
So basically for each node we have a vector space of features that's all that's going on so far.
And also these arrows that these incidence relations also translate into something and they translate into the obvious thing linear maps.
So if these are vector spaces, then these things should be linear maps or just some matrices essentially, right?
So for each arrow you see here we have a matrix and something that I'll argue and show in a few slides is that basically message passing is very similar on graphs, is very similar with group actions in group theory.
So let me explain exactly why.
So we kind of can think of what we have on the left these arrows from the incidence relation.
We could think of these arrows as kind of some buttons we can press.
So what do I mean by that?
So if we have this node v on the left, right, and this e, now if we have some features, some feature living in FOV, right, we could just kind of press this arrow button here and then if we multiply this matrix by this feature, we will get an edge feature.
So it's kind of like if you go along this arrow, this matrix will multiply this feature and this vertex feature and it will give you an edge feature.
So you could think of these arrows as kind of giving you some sort of actions that you can play with to move features from vertex to edge and edge to vertex.
So in this case it's kind of a left action, right?
So this is what I'm saying.
I'm taking this arrow, which is this one here, and I act on some features of node v.
So this HOV that lives here and how I do that is I just take this matrix, this matrix associated with this arrow, and I multiply this vector HOV.
So just matrix times vector, that's all.
And then we get an edge feature.
So this is just kind of a way to move from here to here.
So this already kind of looks a bit like message passing, right?
We're kind of passing a message from this vertex to this edge, but now we also need to pass a message from this edge to these other vertex U.
So we need to get from V to U and we did that by passing through e.
So by doing that, we could do that by kind of going in reverse.
So we could have a right action where instead of applying this matrix, we applied adjoint matrix.
So that's just a transpose matrix.
So if we want to go from here to here, instead of applying this matrix, we apply it transpose because we want to go the other way around.
If we compose these things, then we can move features from V to U.
So this is just a way that kind of we can apply these actions to do message passing and these are called shift actions or preshift actions.
And I'm going to now show what's kind of the relation between this and what we have in group theory.
So one way to represent a group is by kind of having some sort of graph, like here on the left.
So we kind of have some star object, it's just kind of a dummy thing there.
But all the group structure is in these arrows, right?
So for each group element.
So let's say this g is a 90 degree rotation, for instance.
Let's say we do have a group of rotations, just to have some concrete example.
So this arrow could correspond to a 90 degree rotation.
We have another arrow that does the opposite, minus kind of 90 degree rotation.
That's the inverse of that transformation.
So this is kind of the structure of this group.
And if we have, we also do this similar kind of translation as we've just seen.
So basically we define a preshift on this group.
We map this star to a vector space.
So the star kind of replaces the vertex we had before.
Now we just have a single vertex and it's just these arrows we have.
So the star is mapped, this vector space that you show here in blue, right?
And now, if we actually do group actions, which are kind of a very well established concept in group theory, well, for instance, if you want to act on this vertex sorry, not vertex on this vector.
V right here.
You have a vector in this vector space, and you want to act on it by this group transformation g.
So, essentially, you want to press this arrow.
So you apply some action on it.
Then what you do is well, because of this translation, this g has been mapped to some matrix, which is the rotation matrix, the corresponding rotation matrix, and you apply this rotation matrix on v and you get like a 90 degree rotation here.
So this is what's going on.
This kind of vertical vector is showing the rotated vector.
So this is completely analogous with what we've seen on the previous slide.
This is how kind of sheaves connect these kind of actions.
So essentially what you could think of as message passing is same as group actions in group theory, but you just replace this group with a graph.
So it's kind of analogous to that, right?
So it's just kind of a different kind of translations where we replace the object on the left.
Now it looks like this is a graph, this is a group, right?
But kind of the rest stays exactly the same.
And this kind of gives us a way to formalize in a way by looking in this topological perspective to connect all these kind of symmetries and things like that that have been explored quite a lot in machine learning to message passing on graphs and to see one way in which they are related.
Okay, so now you might say, okay, this was all very sophisticated and nice, but you know, what, is this going anywhere, basically?
And I'm just going to show you kind of a very short example.
There's more, but the time is limited.
And something we showed is that, as I was saying in the beginning, many graph neural networks kind of struggle in these heterophilic graphs.
And what we showed is that no matter how heterophilic or kind of weird your graph is, you can always kind of find some shift structure, essentially kind of a message passing neural network, that if you use sufficient layers, it will be able to disentangle the classes of the nodes, right?
So just to show you in this picture what you have here on the very far left, the colors of the nodes, they show the class.
So there's three colors here.
So three classes, right?
And this is kind of the graph in the beginning and the position of the nodes in this box denotes the features.
So that's a way to kind of just to visualize the features.
The 2D position is actually the 2D feature vector of each node.
And you can see in the beginning, everything is kind of super messy and entangled, right?
Like if you want to classify these nodes, it's kind of very hard because their representations, their initial representations are very messy and kind of intertwined.
But as we stack more layers of a particular kind of sheath or a message passing model, you see how progressively these classes get kind of more disentangled and more disentangled at each new layer.
So these representations kind of collapse and they form these kind of clusterings, right?
And then when you get with something like at the end, you can kind of see these three communities very clearly and it's extremely easy to separate.
And kind of the essence behind these results was we showed for different kinds of problems what sorts of chief or message passing models you need by using this theory to solve kind of problems.
And this is quite important because it kind of shows you some important bits and pieces in the architecture that you might want to kind of change or use in order to solve certain kinds of problems.
And we also had some sort of impossibility resolved.
So if you use a graph neural network of some kind, you can't solve this problem or you'll struggle to solve this problem.
And we also saw, okay, if you use some more general ones, then you might have a chance.
So this is kind of some high level view behind this theoretical stuff.
And what we actually do in practice is to essentially learn these message passing functions or to learn the sheath or these matrices.
So in practice, like when someone gives you a node classification task, it's very hard to know beforehand what exactly is the right sheep or the right message passing model to solve that task.
And what we do essentially, we learn that from data.
So we learn these matrices that do the message passing.
We learn them from data by using some neural networks which are shown here in red.
And then you learn how to kind of transfer features between these vector spaces and kind of move them around.
So this is just showing how these vectors, which are features of these nodes and edges, how they're kind of moved around by kind of going through via these matrices, just some matrix multiplications.
Okay, so that's kind of the high level view behind this model.
And we evaluated this on some kind of real world heterophilic data sets where you have to classify nodes based on kind of various communities or different kinds of labels.
And these data sets going from right to left, they are getting more heterophilic.
So in some sense more challenging for classic architectures.
And our models, which are kind of inspired by all this stuff that I mentioned, they score quite highly in these benchmarks.
And at the same time, they also revealed some or justified some various choices that other models in this space have done.
But maybe they were not so well justified, or maybe they had different kind of motivations.
We also managed to kind of show why various things they were already doing, why they made sense from the point of view of this kind of theory.
All right, well, that's all I had.
Yeah, thanks for listening and yeah, happy to chat more about this and also have lots of backup slides in case, depending on how far we venture off with this question.
Cool.

34:04 _Daniel:_
Well, awesome work.
Thank you for the presentation.
For people who are in the live chat, they can write some questions, but there's many things I think we could talk about.
So I want to start with reading a quote from an abstract of the paper by von der Laur, Kudal and DeVries just to kind of ground this in the active inference context and really justify why the message passing approaches that you are describing are helping in the active inference modeling.
It's two papers.
It's called Realizing Synthetic Active Inference Agents and they wrote, with a full message passing account of synthetic active inference agents, it becomes possible to derive and reuse message updates across models and move closer to industrial applications of synthetic active inference framework.
So how does knowing the message passing structure help reuse a model across different settings or facilitate the legibility of the model?

35:10 _Chris:_
Right?
So first of all, I'm not super familiar with the kind of active inference literature, so you'll have to help me there a bit to anchor maybe the discussions a bit more into that.
But I think if I understand correctly, the kind of question you're getting at is basically how can kind of message passing help us generalize in kind of various kinds of settings or maybe from one graph to another and things like that?
And this is a kind of active area of research, how exactly digitalization is happening.
But something you could notice, for instance, something that for instance, was shown like these models are quite good at, for instance, plotting patterns or structures depending on how exactly you implement them.
But for instance, let's say you have a triangle in your graph or that'll be kind of the simplest structure, right?
You have a triangle or some other kind of kind of gadget in your graph, like particular subgraphs that might show up in different kinds of various graphs.
The graphs themselves might look completely different from each other, but these kind of patterns might kind of be reemerging in multiple like local patterns might reemerge in multiple graphs and that could help you a way to kind of generalize, right?
Like you could see, for instance, if you have clicks, they're super important in kind of when you do social network modeling and things like that because they kind of show this kind of close group of friends, right?
They all talk to each other, so they kind of form a click like everyone's connected to each other, right?
And then you might be able to use that engine like another completely different social context where these agents are again kind of communicating in a similar manner or are connected in a similar manner, even if the kind of overall pattern is quite different.
And it goes way beyond just kind of structural similarities because there's also features in there.
So there's combinations of kind of structural patterns and features that give you even more complicated patterns, right?
Like you might have a triangle, but then also two of the features in this triangle look in a certain way and one that looks in another way.
So that gives you even more kind of refinement and even kind of richer pattern detection abilities.
So you have essentially this ability to kind of spot patterns at multiple scales as well.
So you could see this happening at multiple scales.
You could have patterns of patterns, right?
You could have entire communities connected in various patterns and so on.
And again, it's kind of also a research question.
How do you capture these hierarchical patterns and so on.
In general, you have to do more message passing if you want to capture things that are further away from each other because otherwise they can't talk to each other, right?
So, yeah, I don't know if that actually answered your question or if I was kind of going in the right direction there.

38:11 _Daniel:_
It's great.
It brings up a lot of different cool ideas like this patterns all the way down, but totally agree.
I think we can now perhaps explore some more specific connections to active inference because hopefully the listenership or viewership of this, it's kind of like a two way street.
Like some people may be coming from more of your background and then learning about active inference and generative models as a specific system of interest for The First time.
But also, certainly for A lot of people in the active inference space, these methods coming from category theory have only recently come up to, I guess, more prominence in Bayesian modeling, at least where we are.
So it's a cool connection to make.
I think one of the biggest touch points off the bat was, like you mentioned, multiplying a matrix by a vector and interpreting that as an edge.
So just in the inference part of the generative model about sensory observations, we always talk about the thermometer observation and then the underlying hidden state temperature.
So that exactly describes that case.
And that's why we can represent the active inference generative models, the perceptual parts and the action parts in terms of matrix multiplication.
It's why the MATLAB code for generative models does look mostly like matrix multiplication and it can all be done explicitly that way.
Are there models that don't have this feature?
Or what do we gain by having all of our edges defined as appreciative action with a matrix and a vector in this setting of agent generative models with perception and action?
Any thoughts on that?

40:08 _Chris:_
Yeah, I think essentially kind of the graph structure is kind of telling you these things interact in some way, right?
So there's some communication between these vertices if we're kind of in a crash setting, right, and then kind of what the sheath is giving you or any message passing model essentially is expressing a way in which way that connection should manifest in the model or in what way that connection should be used to process information.
So in this case I was mentioning, okay, you have linear maps because you could go on the type if your type of data are vector spaces, then this transformation will be some sort of linear maps.
But it doesn't necessarily have to be.
So for instance, it could go to any nonlinear transformation, right?
And this is what's happening in general.
In practice, if you have a neighbor, the message coming from that neighbor could be modulated by any sort of transformation you want.
So it could be linear, it could be nonlinear, it could be something, I don't know, you can specify it basically.
But essentially you could think of this as you have a structure level telling you who should communicate to whom.
And then you kind of have some semantics that this kind of shift is adding on top saying how should these things communicate?
Right?
Like the first thing is who should communicate or what should communicate.
And then the semantics we add on top essentially describe how should that communication manifest.
Essentially.

41:54 _Daniel:_
Very cool.
I think that maps exactly to how we talk about the sparsity of variables in degenerative model.
So here the topology of the nodes in the graph that we want to do message passing on are going to be describing the agent and the environment or the generative model that includes perception, cognition and action.
So a lot of people have proposed different sparsity architectures for integrated modeling of perception, cognition, action.
So one example would just be like kind of around the clock, like action influences the environment, environment influences perception.
Back to cognition, you could add a self loop using an arkov blanket and different kinds of connectivities and that defines the sparsity topologically, which is where you showed the stack and you were on the second and the third levels, I think, of the stack and then what flows it has to be described, what that edge does.
So what is that?
That is also being provided.

43:02 _Chris:_
Yeah, exactly.
And it could even go to the extreme where does that edge actually do anything?
So for instance, if you have a matrix that's just the zero matrix, for instance, associated to that edge, it will just kind of multiply by zero and that gives you zero and it's kind of essentially pruning that edge, right?
Like I kind of get rid of it, I don't want that communication to happen.
But there's also kind of this possibility where these kind of semantics, they override the structural level where you say, okay, I don't need to communicate with this other agent person or whatever.
It depends on what these rates actually mean and in what context you are.
And then there's also the case where you could do some sort of selective pruning where this matrix depending on so in kind of linear algebra, the matrix has a kernel.
So it's all the stuff that that matrix sends to zero.
So what vectors are sent to zero, right?
But not everything will be sent to zero unless you're the zero matrix.
So depending on the features of the neighbors, you could also just send some of the neighbors to zero, right?
And that kind of removes those neighbors from the equation.
They just kind of get they're not factored in anymore.
So you kind of have this it's a way to get this parsity, I guess, that you were also talking about where certain only maybe a small subset of the inputs or kind of only subset of the features are actually kind of doing some meaningful stuff among the neighbors and everything else will be kind of zeroed out.

44:43 _Daniel:_
Yeah, that makes me think of the Lasso regression, which tries to set most variables of having an impact of zero so that a few hopefully important variables really pop out in the analysis.
But also there's newer techniques, I guess, of attention modeling and reweighting that isn't just like, okay, set five of them to one and then the rest of them to zero.
More nuanced.
So I think that sparsity with the expressivity is basically the best of both worlds because you do want to have a situation where there is an edge, but the attention being paid to it is zero.
So functionally, that doesn't have an update on the belief state, even though in principle the edge exists.
And that's why we can model situations where the agent believes they have impact in the world.
But actually, just because the edge in principle exists doesn't mean that it has any given impact.
And so that allows the articulation of these models where they factorize and keeps interpretable motifs in terms of just little clusters of motifs.
Here in our case describing the action perception and cognition types of systems of interest.
But people, I believe, already implicitly do this.
They will often add an adjective and refer to x kind of active inference.
So like deep active inference with a temporal horizon, sophisticated active inference with this kind of nesting.
And those are pointing to a given feature.
But of course, those features, as we're hoping, should be composable.
And so this seems to be bringing tools that are even more general than just action perception modeling because they're at a lower level of abstraction than any specific system of interest.
But where this work and kind of timeless thinking around cybernetic systems come together through the active inference generative model as a Bayes graph, it gets very exciting.

46:53 _Chris:_
Yeah.
And maybe also something worth emphasizing here is that even if this kind of semantic level can get rid of some edges, right, by doing this kind of pruning.
Something it cannot get rid of is the computation.
So something that kind of that structural graphs level forces you to do.
It kind of tells you what should you spend compute time on, right?
Because even if you're going to decide to prune an edge, you still need to decide that which takes compute time.
So you still need to look at all your neighbors if you're a node, right, and decide what to prune.
Or maybe you don't prune anything or whatever, but you have to look at every edge.
And one way to look at this is the graph structure defines you a computational graph or kind of a computational series of computational steps you have to execute.
And then the kind of the sheet structure or the message passing model actually specifies what those steps are and in what particular way they look.
Exactly.
That's one point.
And you also mentioned attention, and actually I'm glad you did, because this is actually quite related and in certain ways more general than attention.
And actually, maybe going back to this slide, it might be a nice way to see this.
So here basically what happens in attention.
Instead of learning these matrices that we learn here in attention, you learn attention coefficients here.
So you just learn a scalar.
That's the attention coefficient.
How much attention should I pay to essentially this overall edge, let's say, which will be just a scalar?
What we do is kind of a bit more complicated because you just learn, how do I transform these neighbors?
So it's kind of a whole matrix rather than a single scalar, but there's also some subtle differences.
But in a follow up work we did, we also combined this with attention and went a bit more general and that also worked quite well.
But the kind of underlying idea is very similar.
You want to modulate the way you transform information based on the information itself, right?
So you have this kind of one level of recursivity.
If you want that, you are also alluding to that.
It happens in active inference, where, okay, so if I'm node v, right, my neighbor knew it has some features, and based on these features, which are xu, I'm going to find out the matrix that will be used to process xu, right.
So it's kind of very recursive and it's what happens with attention, right.
Based on the features of node u, I'm going to compute an attention coefficient that I'm going to apply to this feature of you, right?
I'm going to decide based on this feature, how much attention should I pay to it.
And here we decide how should I process it more generally in a linear way.
So you have this kind of loopiness structure embedded in there.

50:02 _Daniel:_
Awesome.
I'll bring up a few more points because I think there's so many great pieces.
So Toby St.
Clair, Smyth who we recently discussed his dissertation in Livestream 54, introduced a term or at least a phrasing, the compositional cognitive cartography.
And so thinking about the compositionality of cognitive systems, and I think what you're describing here with this notion that the mappings are more general than the kind of attention mechanisms known, famously today, that those represent, like a lower dimensional special case of one kind of architecture.
Makes me think about how the Bayesian graph is kind of semantic in principle and can have all of these nice categorical formalisms around them.
And you can even build the connector to empirical data with the presheaf and the sheaf, which may be news to even many empirical researchers doing data analysis certainly was for me.
But the message passing provides a rigorous translation from whatever semantic model is proposed topologically to an implementation procedure that can be planned for and executed in linear time or at least with definable characteristics.
So message passing plays a really important part in going from the abstract what is possible, to the implementations of any of these actual models.
And it does it in a really general way where is it accurate to say that we hope that implementation with message passing compatible generative models will kind of roll out better because we won't have some of the engineering challenges that less reusable abstractions might carry?

52:05 _Chris:_
It's hard to say.
I think there's also certainly some limitations to this paradigm as well.
So just kind of doing this kind of message passing, I think, as you were mentioning, one thing is that it kind of scales up quite easily, like linearly with the size of the graph, but that also come at a cost.
So there's certain results showing this has limits in expressivity.
So if you actually want to go beyond this, for instance, instead of just looking at pairs of nodes, you have to look at tuples and these kind of high order groupings of nodes in order to kind of get higher explicitity.
There's all sorts of techniques to do that and there's always this kind of tension between being more expressive and being efficient that will always be there in any sort of algorithm or method.
It's kind of hard to say.
We can definitely say this is kind of not the optimist solution.
Let's say if you want to do things message passing in itself but maybe doing some sort of computations on graphs could be maybe also something that's kind of maybe missing a bit in kind of the graph ML setting.
Is the context where you assume your graph is known.
And you need to have some graph structure, at least a sensible way to construct it.
Right.
But for many kind of more I don't know, how should I phrase that?
I guess for less clearly defined things like, okay, if I'm an agent doing perception in the real world or something, right?
If I'm trying to create a graph of the world, what's an object, what do I create a node for?
Right?
If I want to have one note or object and there's some connections between objects and things like that.
I know it's like some wild example that comes to mind.
I don't know if you actually want to do that but let's say you want, right?
Then there's also all these kind of blurry things like what's an object and what's not an object?
What's kind of somewhere in between maybe is that a node?
So it's kind of like what I'm trying to say, that the graph structure is kind of very discreet, right?
The node is either there or it's not there and edges there is not there.
But then the world is kind of very fuzzy, right?
So if you use graphs as a model for your world then there probably has to be some decision to be made somewhere about these kind of fuzzy concepts.
They actually translate in a concrete graph entity like an object, an edge or whatever or not based on some kind of inference procedure.
And I don't know if we do that or not as kind of humans as intelligent agents, but that's kind of some interesting thing to think about.
Maybe you could also well, maybe one way to solve that is also kind of stuff like soft edges and things like that.
And in some way if you have attention coefficients, it's a bit like that.
If an edge has a weight of 0.1 or something, it's almost like not being there but it's still kind of there.
So it's a bit of a soft graph architecture.
I guess at the edge level you can implement this softness but I think it's a bit harder at kind of the node level, right?
Like how do you kind of model a node that's kind of there and not there?
Yeah, there's just some random thoughts that's.

55:57 _Daniel:_
Very interesting about the fuzzy object identification and kind of similarities and differences between nodes and edges even though in some ways they have some similarities too or interoperabilities too.
One other point of contact was like an underlying hidden space that we understand topologically that projects a vector space from different places so that could be a vector of thermometer readings and we want to have a smooth path within the homeostatic range defined up to a boundary point.
Not saying that that's the structure of the world but a structure of a very heuristic and simple model might be to aim for continuity and have a defined hidden estate space that has continuity underneath and is able to emit vectors.
That kind of brings some of these classifier type discussions that you brought up and the kind of fundamental impossibility of geometric classification because you are going to end up with gray zones whereas even if it takes a bitwise description, you can separate the network.
So that gives an actual completeness measure and that allows measures like I mean amount of computational resources or in a more statistically principled way like the Bayesian Information criterion.
So how many nodes should we have?
We should be on some trade off front in some modeling space.
I don't know what to tell you.
It's a map, not a territory.
And that's more justifiable.
And so even lifelike organisms might want to self evidence staying emitting from a living state.
And so that provides a really simple graphical architecture to cybernetic systems.
And then active Inference explores a lot of different more specific motifs within that broader blanket persistence picture and the path of least action.
So that's what enables the physics in that space and why these methods, which as far as I understand are often used in quantum mechanics, are being able to come together with active inference this way.

58:23 _Chris:_
Yeah, something that comes to mind when you mention this, I think there's also like a recent avenue of research in this area where people and it's again kind of generated by the fact that you don't know the graph beforehand many times.
And I think kind of the old school approach was, well, you construct it based on some rules, right?
Like you're going to say, I don't know, some things are similar, I'm going to put an edge between them and you define similar in whatever way you like and so on.
And there was this kind of recent trend where what you try to do is kind of latent graph inference, or some people call it manifold learning, if you think of the graph as some sort of manifold.
But this kind of very informally speaking and essentially what you would do is like you would map whatever you try to learn the raw observations into some latent space.
And that's where you actually construct the graph.
You construct the graph in the latent space rather than kind of in the raw space.
So that might be kind of a way to deal with fuzziness as well.
Right?
Because then I guess you might lose some of these kind of very concrete one to one mappings because you might learn some node in the latent space that maybe corresponds to three or four concepts kind of mixed together.
There's all these kind of nice experiments with neurons in deep networks, kind of visualized, and they learn maybe kind of a mixture of concepts.
If you see what actually activates that neuron is actually maybe a few classes or different kinds of things.
It's not necessarily a single thing.
So it could be something very similar here where you have some very entangled representations that are kind of distilled in this latent graph.
And then in a way, at least in concept space, even if in the latent space, that's still kind of a very clear combinatorial structure with respect to kind of your raw observations.
That structure can still kind of encode the fuzziness of the world to some degree because you have this kind of mixture of concepts that got distilled in the same node or things like that.
Or maybe some concepts could be represented by multiple nodes depending on what way you see these concepts.
There might be all sorts of variations or concept or points of view and so on.
So I think kind of latent graph inference could be quite an interesting way maybe to address some of these issues we were discussing.
Although I think it kind of died off a bit in the recent year, at least as far as I've seen.
There were a few slightly fewer papers on the topic.

1:01:15 _Daniel:_
Well, certainly the agent's proposed latent structure of the world, the causal structure of the world is just mapped on the territory and so it enables maybe some of those core screenings.
Could you go to the slide where there was a mapping between a smooth sphere and then a regular geometric shape?

1:01:35 _Chris:_
Yeah, let's see in this one.

1:01:40 _Daniel:_
Yeah, just wanted to make one point and see if you had any comments.
At the heart of some of the relationships that you're describing and where you pulled back to in terms of generalization helps us understand this relationship between the sphere and the geometry and the implications for data processing and all of the computational science areas is if you are preserving or learning or analyzing geometry but not topology or the other way around, you might get these different data set.
Aberrations.
Like you might have the topology of the coffee cup, but it looks like something totally different.
And so what we would really want to do would be understand the relationship between geometry and topology.
Because if we could understand it in principle, like you have it on the left side and then in practice with the data scheme on the right side or insert your own left and right side there, then we'd be able to do data analysis in a way that respected preserved both the topology and the geometry.
So it's like two compatible perspectives that have their different strengths and weaknesses and heuristics and so understanding that relationship between geometry and topology and the implicit spaces that geometry requires and so on, that has tremendous use.
And it just in closing, reminds me of Buckminster Fuller's Synergetics, which uses a close packing architecture and a tetrahedron centric model of coordinates to find more continuity between surface area and volume and between the smooth surfaces and the great circles on them and like the points of connectivity on shapes.
So I think it's an incredibly deep area and really has fundamental impact in active inference.
Helps us think about our models in this way, kind of like the inflated balloon with the fuzziness and the architecture and the finiteness.
It really brings a lot to active inference.
And so I appreciate you sharing the work with us today and continuing to work in this way.

1:04:10 _Chris:_
Thanks a lot.

1:04:12 _Daniel:_
Any last thoughts?

1:04:14 _Chris:_
Yeah, what you mentioned, I think it's been all over my thesis this.
Kind of tension between topology and geometry.
And maybe what I want to emphasize is that I'm not saying kind of the previous perspective of looking maybe more geometrically at things was wrong in any way.
And on the contrary, actually, there's lots of interesting places where these things intersect.
Even in kind of this chief paper I briefly went through, like, if you actually read the paper, there's a lot of beautiful intersections.
Actually, my main collaborator, Francesco, he's a differential geometry, so he actually had lots of kind of inputs from that side.
And indeed, I think we should try to use all these kind of layers of structure are in the best way possible for all our methods.

1:05:07 _Daniel:_
Awesome.
All right, thank you.
Till next time.

1:05:10 _Chris:_
Thanks a lot.
Thanks for having me.
Bye.
