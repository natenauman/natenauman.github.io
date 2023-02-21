---
layout: page
title: Professor Supriyo Datta's Lab
nav-menu: false
show_tile: false
---

<!-- Main -->
<div id="main" class="alt">

  <!-- One -->
<section id="one">
	<div class="inner">
		<header class="major">
			<h1>Professor Supriyo Datta's Lab</h1>
		</header>

<!-- Content -->
Two years ago, I found myself preoccupied with lofty dreams of breaking RSA encryption—not to bring down the world economy, but to explore a new form of computing between the classical and quantum regimes. Professor Supriyo Datta’s 2017 paper titled “Hardware emulation of stochastic p-bits for invertible logic” lay printed out on my desk with margins consumed by notes and snippets of code. It described how a network of three-terminal neurons with random outputs known as “p-bits” could be interconnected into Boltzmann Machines. The paper used these networks to perform inverted Boolean gate operations. For example, a p-bit multiplication circuit can find a number’s most likely factors. The computational intractability of semi-prime factorization makes it highly attractive for public-key cryptography such as RSA encryption. I pored over the theory and methods until finally writing my own Python simulation of the paper’s hardware. After successfully reproducing the team’s results and taking a computer security course, I realized that I was still very far from cracking the world’s most widely used public-key cryptography method, but the process of deconstructing and emulating Professor Datta’s paper was incredibly fulfilling and inspired me to pursue a future in research.<br><br>

Upon joining Professor Datta’s p-bit FPGA team during the summer after my sophomore year, I was tasked with designing a true random number generator for sampling different parameterizable probability distributions. I also developed a series of verification tests to evaluate my results. My FPGA implementation of a log-normal sampler utilizes range reduction to precisely approximate the exponential function which receives the result of the Box-Muller transform as its input and produces the associated log-normal sample as its output. My program outputs two independent log-normal samples every clock cycle since all operations within the modules are pipelined. Additionally, the mean and variance are parameters which can be altered by the user.<br><br>

Probabilistic models utilize statistic and probabilistic distributions to account for input data uncertainty. These models uphold much of machine learning and artificial intelligence since input data is assumed to derive from an unknown probability distribution. A major goal of ML research is learning the distribution back from the data. Obtaining this distribution would significantly simplify ML tasks into merely performing probabilistic inference. Probabilistic inference is the process of deriving the probability of at least one random variable taking on particular values. A critically important aspect of building a probability distribution is efficiency. Tractable probabilistic models (TPMs) can theoretically guarantee reliable probabilistic inference in polynomial time.<br><br>

Probabilistic Circuits (PCs) are computational graphs that represent joint probability distributions as recursive mixtures and factorizations of simpler distributions such as Gaussian or Bernoulli distributions. PCs are expressive deep generative models that result in exact probabilistic inference in time linear to the number of layers in the circuit. Therefore, PCs are tractable and the cost of performing calculations can theoretically be quantified depending on the circuit's structure. PCs are essentially neural networks (NNs) in which neurons are either input distributions, sum units, or product units. I designed and tested a sum-product network on the FPGA and used it to predict marginal likelihoods for a graduate-level artificial intelligence class.<br><br>

Finally, I also conducted a thorough literature review to find areas of unexplored statistics. While reading an article on genetic modeling, I came across a fascinating finding that the Gaussian distribution was not always suitable for noise in a system. The paper determined that the log-normal distribution was better for certain external noises. I looked at more studies and noticed that many of them only used Gaussian white noise out of mathematical convenience since it integrates to zero, not because it reflects the data. Usually, the normal distribution is a very safe assumption due to the central limit theorem, but I wondered if this held true for highly nonlinear systems. For example, a graphene resonator is an atomically thin, nonlinear sensor in which some noise sources directly affect mass while others indirectly affect the resonant frequency. I decided to explore how log-normal noise changed a system’s behavior while jumping from one steady state to another compared to other types of noise. This was the first time I crafted my own research question and methods on this scale completely independently. After spending weeks collecting data, I presented at the Elmore Emerging Frontiers Center on the Crossroads of Quantum and AI poster session.
