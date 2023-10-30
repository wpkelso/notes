---
tags: compilers, automata, discrete_mathematics, programming
---

# Finite Automata

## Characteristics of a Finite Automata
- Finite set of states
- Edges from one state to the next, each with a symbol that determines when it is taken
- One start state
- Some number of accepting (match) states

## Conversion from NFA to DFA
1. For a given input and state in a [[Non-Deterministic Finite Automata|non-deterministic finite automata]], consider all state transitions in the [[Epsilon Closure|e-Closure]] of the active state.
2. The next state is the union of the $\epsilon$-closure of all possible transitions. *Each unique set of states we discover must be a single state in the final [[Deterministic Finite Automata|deterministic finite automata]] .*
3. Brute-force exploration to discover all possible state-transitions for all possible inputs.