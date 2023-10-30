---
tags: [mathematics, logic, language]
---

# First-Order Language

A first order language is a [[Formal Language|formal language]] defined by a set of symbols for relations, functions, and constants which when combined with other elementary symbols (such as those of [[Predicate Logic|First-Order Logic]]) single out certain combinations of symbols as sentences.

Like any language, first-order languages have both an [[Alphabet|alphabet]] and [[Grammar|grammar]] included in their [[Syntax|syntax]], in addition to [[Semantics|semantics]].

## Vocabulary

### Group 1: Logical Symbols

#### Logical connectives

| Symbol  | Meaning                  |
| ------- | ------------------------ |
| $\neg$  | negation (“not”)         |
| $\land$ | conjunction (“and”)      |
| $\lor$  | disjunction (“or”)       |
| $\to$   | conditional (“if, then”) | 

#### Quantifiers
| Symbol    | Meaning               |
| --------- | --------------------- |
| $\forall$ | for all               |
| $\exists$ | for each/there exists |

- $\bot$, the propositional constant for falsity
- $=$, the binary identity predicate
- $v_{0}, v_{1}, v_{2}, v_{3}, \dots$, a countably infinite set of [[Variable|variables]]

### Group 2: Punctuation

1. $($
2. $)$
3. ,

### Group 3: Non-logical Symbols

1. Constants: $c_{0}, c_{1}, c_{2}, \dots$
2. [[Predicate|Predicates]]: $R_{0}, R_{1}, R_{2}, \dots$
	- The *arity* ($R^{n}$ where n is a positive integer) denotes the number of operators the predicate holds/involves
	- *Ex.* $<$ in the language of arithmetic
1. [[Function|Functions]]: $f_{0}, f_{1}, f_{2}, \dots$
	- As with predicates, functions also have an arity, denoting how many inputs the function takes
	- *Ex.* $+$, a binary function in the language of arithmetic

## Structures

First-order languages specify [[Sentence|sentences]] as [[Formula|formulas]] without [[Unbound Variable|unbound variables]]. Additionally, we can have structures called [[Model|models]] that satisfy a set of sentences.