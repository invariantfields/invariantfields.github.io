# Towards Eastin-Knill Theorem

Upon further thought I came to realise, it isn't a good idea to go on with the proof without setting up the problem or explaining the relevance of it. Hence, this post $\exists$. 

## Coding

All physical (both c- and qu-)bits are not totally resistant to errors caused by physical "accidents" . Eg: Bits on a CD suffer random damage from dust and scratches, bits on a hard disk can be damaged by stray magnetic fields and qubits suffer from "decoherence" at any finite temperature. 
The errors need to be protected from, and in order to do so, we convert the bits into a **code** and transmitted, stored and computed with In classical systems the simplest code is called repetition code, in which the given bit is repeated n-times i.e. $1  \mapsto 111$ and $0\mapsto 000$. This code is decoded by majority, i.e. if $\#1> \#0$ we consider it to be $1$ and $0$ otherwise. This gets down the error rates from $p$ for single bit to $3p^2(1-p)+p^3$. 
There exist such techniques for qubits as well and will be discussed in detail in the **Part2** of this series. 

## Gates

The bits are useful for computing, and another building block for making a computer is **gates**. The gates are used to manipulate bits and hence, performing computations. The minimal set of gates needed to perform any possible gate is called **universal gate set**. This set for classical bits consists of  just the NAND gate or NOR gate and for quantum system there are several(thanks to Solvay-Kitaev theorem) finite universal gate sets.

A very naïve way to use our universal gates on the coded systems would be to apply single bit gates individually on each of the bits and 2-bit gates on 2 bits with each from the codes of 2 different  *coded* bits. 
i.e. 
$A \mapsto A_1A_2A_3$
and 
$B \mapsto B_1B_2B_3$ 
 then
  $A$NAND$B\mapsto$ ($A_1$NAND$B_1$)($A_2$NAND$B_2$)($A_3$NAND$B_3$) 

Such an application of gates is termed as **Transversal gates**. 
Though the above operation is valid for universal gates on classical bits, it wasn't completely proved or disproved to be valid for a long time for quantum bits and systems. This finally was proved to be impossible to do for quantum systems by Eastin and Knill in their aptly titled paper [Restrictions on Transversal Encoded Quantum Gate Sets](https://arxiv.org/abs/0811.4262). or rephrasing the central theorem of the paper 
>**It is impossible to make a transversal universal gate set for a quantum code.**

This comes with several caveats which would be discussed in greater detail in **Part-3** of this series, where I would also explain my contribution to generalise this for subsystem codes(to be discussed in **Part-2**)   

## References
[1] Bryan Eastin,Emanuel Knill. [Restrictions on Transversal Encoded Quantum Gate Sets](https://arxiv.org/abs/0811.4262)
## Up next
### Prerequsites 2.0

#### Logical operators
#### Codes
#### Projectors


