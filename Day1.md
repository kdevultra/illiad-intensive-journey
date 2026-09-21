# Day 1
**Date:** Sep 21 2026

## Entropy and KL Divergence
### Entropy
Entropy can be seen as the "noise" or the pertubation, or the energy of change and imprevisibility in a system, that quantifies its likelihood to change (and maybe is tied somehow to the degrees of freedom of the system). In information theory, it quantifies the average number of "bits" necessary to describe an event from a probability distribution. 

Another intuition (personal) might be the energy the system takes to come back to the initial stable state. If it is stable (expected no disturb), it is null. The contrary explains itself.

Its mathematical formula is: $\boxed{ H(P) = -\sum P(x) \log_{2} P(x)}$ (P is a probability distribution).
### KL Divergence
Stands for **Kullback-Leibler Divergence** (or relative divergence). Given two probs dist. P (the true distribution, ideal and complex) and Q (its approximation), $D_{KL}$ measures the "impact" or "penality" that is done when using Q. Its interpretation is quite complicated, but [Six (and a half) intuitions for KL divergence](https://www.lesswrong.com/posts/no5jDTut5Byjqb4j5/six-and-a-half-intuitions-for-kl-divergence) by CallumMcDougall (2022) on LessWrong gives good ideas. I believe this one from the same post is a good general understanding:
> $D_{KL}(P||Q)$= measure of how much our model Q differs from the true distribution P. In other words, we care about how much P and Q differ from each other _in the world where P is true_, which explains why KL-div is not symmetric.

It is expressed as: $\boxed{D_{KL}(P||Q)=\sum P(x)\log_{2} \frac{P(x)}{Q(x)}}$.

> [!NOTE] Important
> The core thing here is that $D_{KL}(P||Q) \not = D_{KL}(Q||P)$ : the KL-divergence is asymetric, and is not a "geometric" measure because of that.



