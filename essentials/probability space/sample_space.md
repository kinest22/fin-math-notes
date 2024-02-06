## Sample space

In probability theory, a **random experiment** is a mathematical formalization for a corresponding real experiment whose outcomes cannot be determined in advance. The set of all possible outcomes (elementary events) of such an experiment forms a **sample space** and is denoted as $\Omega$. The stand-alone outcome of random experiment is denoted as $\omega$. In Kolmogorov’s axiomatics **sample sapce** is one of the elements of the probability space $(\Omega, \mathcal{F}, \mathbb{P})$. 


## Discrete and continuous sample spaces
Sample space is called **discrete** if the number of its elements is finite or countable. Conversely, any asmple space that is not discrete is called **non-discrete**. Specifically, if outcomes of sample space are points of a particular numerical or coordinate space, then the space is called **continuous** (or **continuum**).

***Example 1***. Consider an experiment in which a single coin is tossed. In this case we are dealing with the sample space which is <ins>*countable*</ins> and is given as follows: 
```math 
\Omega=\{H,T\}
``` 
where the outcome $H$ means that the coin is heads and the outcome $T$ means that the coin is tails.

***Example 2.*** Consider now a more tricky experiment that involves endless coin toss. Sample space now can be formalized as: 
```math
\Omega=\Bigl\{\omega:\omega=(\omega_1,\omega_2,\omega_3,...),\omega_i\in \{H,T\}\Bigl\}
``` 
In words, $\Omega$ is the set of all elements $\omega$, such that each $\omega$ represents a <ins>*countably infinite*</ins> tuple (sequence) of elements $\omega_i$ each of whom are either $H$ (Heads) or $T$ (Tails). It should be pointed out that $\omega$ and $\omega_i$ have different meanings here. That is, $\omega$ represents a tuple or a sequence (is enclosed in circular brackets in the notation above) and includes infinite number of $\omega_i$.







<!---
## Power set
$$\Omega=\{\text{⚀,⚁,⚂,⚃,⚄,⚅}\}$$
The number of elements of a finite set is a natural number (possibly zero) and is called the cardinality (or the cardinal number) of the set.
--->

