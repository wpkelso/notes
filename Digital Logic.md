---
tags: logic, digital_logic, microelectronics, circuits
created: 2023-11-13T11:57
updated: 2023-11-15T08:32
---

# Digital Logic

Digital logic is a binary system, mapping regions of high and low voltage in the output of a CMOS [[Field Effect Transistor|FET]] to digital values of `1` and `0` respectively.

## Logic Levels

In the ideal world, there are only two voltage levels defined for the digital logic levels: 

$$
\text{Digital logic level} = 
\begin{cases}
V_{L} & \text{when the logic level is `low'} \\
V_{H} & \text{when the logic level is `high'}
\end{cases}
$$

However, the real world is anything but ideal. As such, there are actually six levels defined, based off the voltage transfer characteristics of the non-ideal [[Inverter|inverter]] (shown below).

![[Pasted image 20231113120803.png]]

This corresponds to the levels shown in the plots as follows:
$$
\text{Digital logic level} =
\begin{cases}
V_{L} & \text{nominal voltage for a `low' logic level, } v_{i}=V_{H} \\
V_{H} & \text{nominal voltage for a `high' logic level, } v_{i}=V_{L} \\
V_{IL} & \text{maximum input voltage for a `low' input logic level} \\
V_{IH} & \text{maximum input voltage for a `high' input logic level} \\
V_{OH} & \text{output voltage corresponding to an input voltage of } V_{IL} \\
V_{OL} & \text{output voltage corresponding to an input voltage of } V_{IH}
\end{cases}
$$

## Noise Margins

Noise margins exist to prevent the circuit from producing erroneous output under noisy input conditions. They are defined for the input levels as follows:
$$
\begin{cases}
NM_{L}=V_{IL}-V_{OL} & \text{for `low' input levels} \\
NM_{H}=V_{OH}-V_{IH} & \text{for `high' input levels}
\end{cases}
$$