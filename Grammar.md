---
tags:
  - compilers
  - programming
  - logic
  - language
created: 2023-09-08T14:31
updated: 2023-10-18T09:22
---

# Grammar

Gives a precise syntactic specification of a language. 

## Compilers

Grammars can automatically be converted into a parser, similar to the way a [[Lexical Analysis|lexer]] is generated from a set of [[Regular Expression|regular expressions]].

There are a couple of topics specific to their use in programming language compilers. These are known as context-free grammars and ambiguous grammars.

### Context-Free Grammars

These consist of:

- A set of tokens, known as *terminal symbols* (these come directly from the [[Lexical Analysis|scanner]])
- A set of *non-terminals*
- A set of *productions* (A non-terminal on the the left side, and a sequence of tokens and non-terminals on the right)
- A designation that one non-terminal is the *start symbol*

### Ambiguous Grammars

A grammar is ambiguous if there are multiple parse trees for a given program. *We should avoid ambiguous grammars at all cost.*