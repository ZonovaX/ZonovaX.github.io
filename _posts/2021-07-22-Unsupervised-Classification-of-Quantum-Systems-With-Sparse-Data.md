---
title: Unsupervised Classification of Quantum Systems With Sparse Data
author: Saad Khalid
category: machine learning
layout: post
---

<figure>
  <img src="https://raw.githubusercontent.com/ZonovaX/zonovax.github.io/master/classified_quantum_system.jpg" width = "500"/>
  <figcaption>
  After applying our algorithm, samples from two systems which were previously indistinguishable are now visually distinct.
  </figcaption>
</figure>

Quantum systems are ruled by probability. In practice, this means that if you look at the same quantum system twice, you'll see something different both times. In order to get a full understanding of a quantum system, one has to take many independent pictures (or samples) of it and combine them. However, the number of pictures required to properly identify a system and distinguish it from another grows exponentially with the size of the system, making it practically impossible to do by naively comparing the samples of the two systems. However, being able to efficiently distinguish quantum systems is crucial for creating practical quantum computers. In addition, methods for classification with noisy and sparse data is an active area of research in machine learning; our method is a possible solution to this problem. <br />
<br />
Here we develop an unsupervised classification algorithm to efficiently distinguish quantum systems. Our algorithm works by transforming the original samples to get rid of redundant degrees of freedom. As a result, significantly fewer of the transformed samples are required to distinguish two systems. We generated 10m+ samples of known high-dimensional quantum systems using Monte Carlo methods to test the algorithm. We then applied the algorithm to subsets of this data of varying degrees of sparsity, ranging from 100 to 100,000 samples, and achieved 99% classification accuracy. <br />
[arXiv link!](https://arxiv.org/pdf/2107.10949.pdf)