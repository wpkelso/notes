---
created: 2024-09-30T09:12
updated: 2024-09-30T09:12
---

# Model Coverage

Model coverage analysis determines which requirements expressed by the model were not exercised by verification based on the requirements from which the model was developed.
It does not eliminate [[Code Coverage]], but instead supports the detection of unintended functionality within the design of the model.


## Methodology

- *Stream occurrence* $s$:: covered by a scenario showing its influence on an output
- A model is “covered” if all it’s stream occurrences are