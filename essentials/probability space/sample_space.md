## Sample space

In probability theory, a **random experiment** or (**random trial**) is a mathematical formalization for a corresponding real experiment whose outcomes cannot be determined in advance. The set of all possible outcomes (elementary events) of such an experiment forms a **sample space** and is denoted as $\Omega$, while the stand-alone outcome of random experiment is denoted as $\omega$. In financial markets one can regard this also as the states **of the world**, understanding by this all possible states the world might have. In Kolmogorov’s axiomatics **sample sapce** is one of the elements of the probability space $(\Omega, \mathcal{F}, \mathbb{P})$. 

A collection of outcomes of some random trial must meet following constraints in order to be a sample space:
- The outcomes must be mutually exclusive.  That is, if some outcome occurs, then no other outcome will take place.
- The outcomes must be collectively exhaustive. That is, on every experiment  there will always take place some outcome.
- The sample space must have the right granularity depending on what the experimenter is interested in. Irrelevant information must be removed from the sample space and the right abstraction must be chosen.


## Discrete and continuous sample spaces
Sample space is called **discrete** if the number of its elements is finite or countable. Conversely, any sample space that is not discrete is called **non-discrete**. Specifically, if outcomes of sample space are points of a particular numerical or coordinate space, then the space is called **continuous** (or **continuum**).

***Example 1***. Consider an experiment in which a single coin is tossed. In this case we are dealing with the sample space which is <ins>*countable*</ins> and is given as follows: 
```math 
\Omega=\{H,T\}
``` 
where the outcome $H$ means that the coin is heads and the outcome $T$ means that the coin is tails. 

***Example 2***. Consider a triangular dice with four sides. The values on the first two sides are 2 and 3 respectively. The other two sides of a dice have the same value of 8. Then for the experiment where such a triangular dice is rolled we have the countable sample space:
```math 
\Omega=\bigl\{⚁,⚂,⚄\bigr\}
``` 
In this definition of $\Omega$ it is assumed that the sides that have the same value are indistinguishable (i.e., one only cares about the resulting number). Thats why $\Omega$ contains only three outcomes, which are unique.

***Example 3.*** Consider now a more tricky experiment that involves endless coin toss. Sample space now can be formalized as: 
```math
\Omega=\Bigl\{\omega:\omega=(\omega_1,\omega_2,\omega_3,...),\omega_i\in \{H,T\}\Bigr\}
``` 
In words, $\Omega$ is the set of all elements $\omega$, where each $\omega$ represents a <ins>*countably infinite*</ins> tuple (sequence) of elements $\omega_i$ each of whom are either $H$ (Heads) or $T$ (Tails). 

One can notice that $\omega$ and $\omega_i$ have different meanings here. While $\omega_i$ is elementary outcome of a single coin toss ($H$ or $T$),  $\omega$ represents a family of <ins>*infinite countable*</ins> tuples of these outcomes and denoted as a sequence of values $\omega_i$ enclosed in circular brackets $(\omega_1,\omega_2,\omega_3,...)$. One such sequence might begin as: $$(H,T,H,T,H,T,…)$$ while another might begin as: $$(H,H,H,H,H,H,…)$$ and so on. 

Due to this fact the set of all such sequences (i.e. sample space $\Omega$) is <ins>*uncountable*</ins>. In other words, sample space $\Omega$ represents uncountable set of infinite countable sequences of heads and tails.

***Example 4***. Another example that implies uncountable sample space is an experiment that results to a real number that satisfies a certain predicate $\Phi(x)$. For example:
```math
\Omega=\Bigl\{\omega:\omega\in\mathbb{R}\wedge\cos{(x)>\frac{1}{2}}\Bigr\}
``` 
Here $\Omega$ is the set of all real numbers that satify the predicate $\Phi(x)=\cos(x)>\frac{1}{2}$. Due to the fact $\mathbb{R}$ is uncountable $\Omega$ is also uncountable. 







<!---
## Power set

The number of elements of a finite set is a natural number (possibly zero) and is called the cardinality (or the cardinal number) of the set.
--->

