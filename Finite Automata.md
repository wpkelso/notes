#compilers #automata 
## Characteristics of a Finite Automata
- Finite set of states
- Edges from one state to the next, each with a symbol that determines when it is taken
- One start state
- Some number of accepting (match) states

## Conversion from [[Non-Deterministic Finite Automata|NFA]] to [[Deterministic Finite Automata|DFA]]
1. For a given input and state in an NFA, consider all state transitions in the [[Epsilon Closure|e-Closure]] of the active state.
2. The next state is the union of the $\epsilon$-closure of all possible transitions. *Each unique set of states we discover must be a single state in the final DFA.*
3. Brute-force exploration to discover all possible state-transitions for all possible inputs.