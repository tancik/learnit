# Learned Initializations for Optimizing Coordinate-Based Neural Representations
### [Project Page](https://www.matthewtancik.com/learnit) | [Paper](https://arxiv.org/abs/2012.02189)
[![Open Demo in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tancik/learnit/blob/master/meta_demo.ipynb)<br>

[Matthew Tancik](http://tancik.com/)\*<sup>1</sup>,
[Ben Mildenhall](https://people.eecs.berkeley.edu/~bmild/)\*<sup>1</sup>,
Terrance Wang<sup>1</sup>,
Divi Schmidt<sup>1</sup>,
[Pratul P. Srinivasan](https://people.eecs.berkeley.edu/~pratul/)<sup>2</sup>,
[Jonathan T. Barron](http://jonbarron.info/)<sup>2</sup>,
[Ren Ng](https://www2.eecs.berkeley.edu/Faculty/Homepages/yirenng.html)<sup>1</sup><br>

<sup>1</sup>UC Berkeley, <sup>2</sup>Google Research
<sup>*</sup>denotes equal contribution


## Abstract
![Teaser Image](https://user-images.githubusercontent.com/3310961/103447030-36275800-4c43-11eb-92ac-a242130d6e04.jpg)

Coordinate-based neural representations have shown significant promise as an alternative to discrete, array-based representations for complex low dimensional signals. However, optimizing a coordinate-based network from randomly initialized weights for each new signal is inefficient. We propose applying standard meta-learning algorithms to learn the initial weight parameters for these fully-connected networks based on the underlying class of signals being represented (e.g., images of faces or 3D models of chairs). Despite requiring only a minor change in implementation, using these learned initial weights enables faster convergence during optimization and can serve as a strong prior over the signal class being modeled, resulting in better generalization when only partial observations of a given signal are available.

## Code
We provide a [demo IPython notebook](https://colab.research.google.com/github/tancik/learnit/blob/master/meta_demo.ipynb) as a simple reference for the core idea. Scripts for the different tasks are located in the [Experiments](https://github.com/tancik/learnit/tree/master/Experiments) directory.