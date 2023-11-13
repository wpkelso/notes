---
aliases:
  - FET
tags:
  - electronics
  - circuits
  - microelectronics
created: 2023-09-27T12:46
updated: 2023-11-13T11:57
---

# Field Effect Transistor

## JFET (Junction FET)

## MOSFET (Metal Oxide Semiconductor FET)

![[Pasted image 20231015162527.png]]

The MOSFET is one of the most common types of FETs, often acting as an electronically controlled switch. The MOS in MOSFET stands for Metal Oxide [[Semiconductor]], usually using Silicon Oxide as the semiconductor material.

There are a couple different types of MOSFETS:
- n-channel (NMOS)
- p-channel (PMOS)
- Complementary-symmetry (CMOS)
	- This is a combination of n-channel and p-channel devices on the same IC

Additionally, MOSFETS can either be *depletion-type* or *enhancement-type*. NMOS and PMOS devices parallel each other in their characteristics; however, PMOS has it’s polarity reversed with respect to NMOS devices. Thus, all voltages and currents are reversed.

## Operation Regions

### Cutoff

Occurs when $V_{GS} < V_{T}$. In this region, no inversion layer is formed, and drain and source are separated by a depleted channel. This results in $I_{DS} \approx 0$, as well as $i_{B}=i_{G}=0$.

### Linear (Triode/Ohmic)

The Triode region can additionally be considered as the *voltage-controlled resistance* region

### Saturation

## Biasing 

### Substrate Conditions

#### Accumulation

![[Pasted image 20231018110448.png]]

#### Depletion

![[Pasted image 20231018110554.png]]

#### Inversion (Channel formation)

![[Pasted image 20231018110628.png]]

### Bias Analysis

1. Assume an operation region (usually saturation)
2. Use circuit analysis to find $V_{GS}$ 
3. Use $V_{GS}$ to calculate $I_{D}$, and $I_{D}$ to calculate $V_{DS}$
4. Check validity of operation region assumptions

### Finding the Q-Point

The [[Quiescent Point]] for a FET is found in a similar way to BJTs, but the Q-Point for a FET is found as ($I_{D}, V_{DS}, V_{GS}$).

### Four-Resistor Bias Network

A four-resistor bias network is used for biasing [[Transistor|transistors]] in discrete circuits, as it stabilizes the bias point with respect to device parameter and temperature variations using negative feedback. Generally, it is used to bias transistors in saturation region.