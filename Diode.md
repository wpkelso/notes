---
tags:
  - chemistry
  - electronics
  - circuits
created: 2023-09-08T14:31
updated: 2023-09-08T16:58
---
# Diode
Constructed by depositing a p-type [[Semiconductor|semiconductor]] on top of an n-type semiconductor.

>[!note] Definition
> A **PN Junction** is the interfacing region between the $n$ and $p$ regions inside of a diode or other semiconductor-based component.

In a diode, the $p$ region is on the anode/positive side of the diode, and the $n$ region is on the cathode/negative side of the diode.

![[diode-diagram.png]]

## Biasing

There are three types of biasing, or operating regions in diodes: equilibrium, reverse bias, and forward bias.

### Equilibrium (No Bias)

At $t=0$ under zero bias conditions, carriers naturally diffuse across the junction due to the difference in hole and electron concentrations on each side. This creates a region depleted of mobile carriers at $t=t_{1}$. However, the charge density in the depletion region is still nonzero. *Any carriers that diffuse across the junction are annihilated, as they recombine with majority carriers.* 

With the formation of the depletion region, an [[Electric Field]] emerges, going from this positive charges to the negative charges. The width of this depletion region $W_{d0}=x_{n}+x_{p}=\sqrt{ \frac{2\epsilon_{s}}{q}  \left( \frac{1}{N_{A}} + \frac{1}{N_{D}} \right) \phi_{j} }$, where $\phi_{j}$ represents the **built-in potential**.

>[!note] Definition
> Defined as the negative integral of the electric field created across the junction in equilibrium , the **built-in potential** prevents carriers from diffusing across the junctions.
> TODO add equations