# Weeks 6 and 7: Regression and Clustering

## Day 1-7: Intro to applied deep learning

### Understanding NNs visually (3b1b)

1. [Chapter 1: But what is a NN?](https://www.youtube.com/watch?v=aircAruvnKk)

2. [Chapter 2: Gradient descent](https://www.youtube.com/watch?v=IHZwWFHWa-w)

3. [Chapter 3: Backpropagation](https://www.youtube.com/watch?v=Ilg3gGewQ5U)

### What frameworks are out there?

#### Tensorflow

My suggestion if for those people who want to be developers at their core, but also want to be able to incorporate ML into their projects, go with **Tensorflow**. It has numerous tutorials to learn from and various packages like [tensorflow.js](https://www.tensorflow.org/js), [tensorflow lite](https://www.tensorflow.org/lite) and [TFX](https://www.tensorflow.org/tfx) for web apps, mobile apps etc., making life quite easy for you.

It also has 3 layers of abstraction:

1. Sequential API: The most basic version (adding layers one after another)

2. Functional API: A more flexible version, and the one you'll be using the most. (It's easier to understand this API from the docs/ visually rather than me explaining it)

3. Sub-classing API: The one that offers the most customization. But unless you're really into tensorflow for whatever reason, if you find yourself using this/ wanting to use this more than rarely, switch to PyTorch.

4. [Fireship: Tensorflow in 100s](https://www.youtube.com/watch?v=i8NETqtGHms)

**NOTE:** Don't go by the hate on the internet for Tensorflow. Much of it is because of the structure of TF 1.x. Th current versions (2.x) are well maintained and are very simple to use. Most reddit threads or medium articles are based off this previous hatred on the framework, so go with what suits you best right now.

The only point that stands is that there are more pre trained models in PyTorch as a lot of researchers jumped ship to PyTorch during this TF 1.x time. Though most state of the art models should be present in both frameworks right now.

A slightly old article (2022), but one without a biased opinion: [Tensorflow vs PyTorch (and JAX?)](https://www.assemblyai.com/blog/pytorch-vs-tensorflow-in-2023/)

#### PyTorch

PyTorch is probably the most popular deep learning framework out right now. Its's used by researchers and developers both (mostly the former from what I've read on the internet).

From what little experience I have working with the framework, there's mainly two ways of writing PyTorch networks. The sequential way and sub-classing? way. The only difference will be whether you want to write your own forward propagation method.

If the network/ network block is simple/ sequential where the forward prop is obvious, then use the sequential api and the library will know what to do every forward pass. If you have a complex network with different branches/ blocks then use the general sub classing API and define how the forward pass should work.

At first, those shifting from TF (keras) to PyTorch might find writing PyTorch code extremely cumbersome, but trust me it gets easier over time. Also the ease of writing out much more complicated structures in PyTorch is quite nice, especially if you're used to writing Python code.

There's also something called [PyTorch Lightning](https://lightning.ai/docs/pytorch/stable/), which helps you maintain a nice style while writing your pytorch code as well as reduce some boilerplate wherever possible. If you're just starting out continue with vanilla PyTorch and come back to this later when you are comfortable.

There are seperate packages as well that will help you in computer vision, nlp problems, audio etc. like torchvision, torchtext, torchaudio etc.

Both tensorfow and pytorch have rich hubs with pre-trained state of the art models. (We'll revisit this in transfer learning don't worry, but you can read up on it now as well.)

1. [Fireship: PyTorch in 100s](https://www.youtube.com/watch?v=ORMx45xqWkA)

#### JAX

Well, for now I'd day let JAX be. It's an insane library for linear algebra (XLA = Accelerated Linear ALgebra) with Autograd (It isn't a deep learning library, but you can easily create networks using it and there are newer deep learning libraries like Haiku based on it).

However I'm still getting the hang of it, so currently I wont be much for you. But if possible we can hold a ws later on this year for you nerds.

### Videos/ Tutorials (Do 1 & 2 OR 3 after choosing a framework)

1. [Tensorflow: Part 1](https://www.youtube.com/watch?v=tpCFfeUEGs8)

2. [Tensorflow: Part 2](https://www.youtube.com/watch?v=ZUKz4125WNI&list=RDLVtpCFfeUEGs8&index=2)

3. [PyTorch](https://www.youtube.com/watch?v=Z_ikDlimN6A)

**Note:** The Pytorch one has many sections on implementing CNNs (for computer vision) as well, but don't break the flow and go along with it. However this kind of computer vision is extremely basic, so do read the theory linked in the next week.

I haven't done the tensorflow one completely myself, but if the same thing is there in those 2 videos, follow the same. Don't worry if it isn't though, I'll link up some in the next week just in case.

### Optional

1. [3b1b Chapter 4: Calculus in backprop](https://www.youtube.com/watch?v=tIeHLnjs5U8)

## Day 8-14: Computer Vision

### Optional

## Day 15-18: Contest (Final)

Topic: Face identification and clustering

Dataset: To be announced

Problem statement: To be announced

Incentive: If there is one, it will be announced
