# Information in Physics

Information is something that is encoded in the state of a physical system.

Here are some theoretical milestones that improve our understanding of how physcis address information.

## Landauer's principle

Erasure of information is a dissipative process. 

For example, I can store one bit of information by placing a single molecule in a box, either on the left side or the right side of a partition that divides the box.

Erasure means that we move the molecule to the left side (say) irrespective of whether it started out on the left or right. 

I can suddenly remove the partition, and then slowly compress the one-molecule \gas" with a piston
until the molecule is definitely on the left side. 

This procedure reduces the entropy of the gas by $\triangle S =k\ln{2}$ and there is an associated  flow of heat from the box to the environment. 

If the process is isothermal at temperature T,
then work $W = kT \ln{2} $ is performed on the box, work that I have to provide.

> If I am to erase information, someone will have to pay the power bill

## Reversible computation

In classical computer, NAND gate is irreversible process gate.

$$
(a,b)\rightarrow NAND \rightarrow \neg(a\wedge b)
$$

Information is erased by NAND gate. Classical NAND gate intrinsically cause work dissipation $W=kT\ln{2}$.

But quantum computation is could be reversible. In Toffoli gate,

$$
(a,b,c)\rightarrow Toffoli \rightarrow (a,b,c\oplus a\wedge b)
$$

This computation could be done with negligible dissipation.

## Maxwell's Demon

Let's envision a gas in a box that devided by partion into two parts A and B.

The partition has a shutter operated by small demon. opening the partition and closing the partition need no work. 

Small demon can classify each atom in a gas into cold one and hot one. If a cold one goes left, demon open the partition and close instantly. If a hot one goes right, demon open the partition and close instantly. As time goes by, left side of the box cooler and right side of the box hotter.

Demon does not work, but box's entropy goes down. It is contradiction in terms of thermodynamic law 2.

Breakthrough is that the demon has a finite memory. For lowering the entropy, demon has to remember the state of atoms in a gas. For cooling constantly, demon has to remove some information of atoms to store new information. In the erasure process, work is done by demon. 
