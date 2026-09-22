# Day 2
**Date:** Sep 22 2026

Today we’re talking about the theory of computation and Turing machines. The following notes are what I’ve understood, my personal takes, so I know that I may be wrong at some places; please correct me if you notice any problem.

## Theory of computation and Turing machines

The theory of computation is the study of the solvability of problems by machines or computers. It is the foundations of modern computer science and guides problem solving in computational experiments. It has 3 main pillars:

- computability theory
- complexity theory
- automata theory

### Computability theory

This is the theory in computer science that determines whether a problem is solvable by a machine/computer. In other words, it studies what problems are computable or not.
For example, let’s say we have two problems:
- **Problem 1:** Given a set of numbers, we want to pick those that are multiples of 10 for whatever reason. Obviously, this is easily doable on a computer even by a short program.
- **Problem 2:** Given the current books that we have, we would like to predict whether one of the books will disappear the next day (that might be a bizarre problem though, but let’s just keep that). Unless the computer is a seer, that wouldn’t be possible to know. So this problem is not computable.

### Complexity theory

Rather than checking if a problem is computable or not (note that the problem at hand is assumed or proven to be computable), this theory determines the efficiency of the solvability of the problems. This efficiency is measured in time (and I believe resources also). In other words, it answers the following question: how much would it cost to solve this problem ?

When we think about the classification problem from the previous example, we can be certain that the resolution of this problem is quite fast; it depends on the length of the list of numbers but anyway, it is generally fast in a real-life context.

In comparison, a prime-number verification of a 28-digits number is quite complicated, and normal computers take a long time to check it. Moreover, factorisation of prime numbers is a problem in cryptography/cybersecurity that is known to be almost impossible to solve by normal computer. So in our context, this is not an efficiently solvable problem, because it is much more complex than a simple program.

### Automata theory

This is generally considered to be the most important concept in the theory of computability. Its goal is to design abstract machine (or an automaton) to solve computational problems. Such a problem is considered computational when it can be solved by a step-by-step approach.

I view this as an abstract schematization highlighting the process, and the steps, and the actions one might take in a chronological or organized order to solve a problem. I think the best analogy to this is to think about the design and organisation of an algorithm (but can’t we just say that algorithms are abstract machines, or automatons).

If you have been creating processes (onboarding in company, marketing strategies, mindmaps of visual workflows), I think that you already created abstract machines, maybe even whithout knwing it.

### Turing machines

In 1936, Alan Turing introduced the Turing Machine concept (which is I think, an abstract machine, or automaton in the automata theory). I won’t be diving deep into the details, but what’s important to understand here is that it is the foundation of any computer program or algorithm that exists today, after the theory of Church-Turing: anything that can be computed by a physic algorithm can be computed using a Turing Machine.

Therefore come The Halting Problem that can be summarized as follows:

*Is it possible to write a program that tells whether another program halts, or stops ?*

He himself demonstrated that such an algorithm is cannot exist, by using a proof by contradiction.

### How all this apply to AI safety

Every AI system is Turing Machine. And no algorithm does exist that can tell if another one ultimately stops. In the aligment problem, that means that we can never write a perfect algorithm that verifies if an AI system won’t cross a security barrier. In other words, only by code/computational techniques, this is not possible.

Hence, the need to understand at the core what happens, and figure out ways to ensure this goes well, intervening at any stages of AI development.

