#compilers 
Gives precise syntactic specification of a language. It can automatically be converted into parsers, similar to the way a [[Lexical Analysis|lexer]] is generated from a set of [[Regular Expression|regular expressions]].

## Context-Free Grammars
These consist of:
- A set of tokens, known as *terminal symbols* (these come directly from the [[Lexical Analysis|scanner]])
- A set of *non-terminals*
- A set of *productions* (A non-terminal on the the left side, and a sequence of tokens and non-terminals on the right)
- A designation that one non-terminal is the *start symbol*

## Ambiguous Grammars
A grammar is ambiguous if there are multiple parse trees for a given program. *We should avoid ambiguous grammars at all cost.*