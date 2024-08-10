---
tags: computing
created: 2024-07-18T16:46
updated: 2024-07-18T17:21
---

# Information

Information can be defined as knowledge communicated or received, pertaining to a specific fact or situation.
To be able to design a system to work with information, it is necessary to have a way of quantifying information.

> Information resolves uncertainty.
> Information is simply that which cannot be predicted.
> The less predictable a message is, the more information it conveys.
>
> MIT OpenCourseWare, 6.004 Lec01

## Quantifying and Encoding

In [[Computer Architecture|Computer Architectures]], information representation is done through “bits”→
number of binary digits required to encode a choice or choices.
This encoding impacts the design at multiple levels:

- “Mechanism” → devices &amp; number of components used
- “Efficiency” → the number of bits used
- “Reliability” → noise/interference
- “Security” → [[Encryption]]

When given $N$ equally probable choices and some given information narrows it down to $M$ choices, then $\log_{2}\left( \frac{N}{M} \right)$ bits can be used to represent that information.
When choices have different probabilities $p_{i}$, then more information is given when presented with an unlikely choice than a likely choice.

The average information from a choice can be represented by $\sum p_{i} \log_{2}\left( \frac{1}{p_{1}} \right)$, where $\log_{2}\left( \frac{1}{p_{i}} \right)$ is the information from a single choice.
Extending from this, variable-length encoding can be used to encode these choices more efficiently → shorter bit sequences used for high probability choices, and longer bit sequences are used for lower probability choices. See [[Data Compression]] for more info on this.

> [!question] Is redundancy always bad?
> Not necessarily. Sometimes increasing redundancy is a target if we wanted to make information easier to manipulate with [[Fixed-Size Encodings]], or to increase resilience with error detection and correcting codes (ex. parity bit).


