---
created: 2023-09-08T14:31
updated: 2023-09-08T14:31
---
#compilers 
Method to represent a **set** of strings in a concise way. A string described in this way is said to "match."

## Concatenation
If two REs are appended in sequence, both must match or the whole expression to match.

## Alternation
An operator ( | ) that allows a choice between two REs

## Repetition of Patterns
$*$ = Match 0 or more times
$+$ = match 1 or more times
$?$ = Match 0 or 1 time
(*A regular expression allowed to match 0 times can match an empty string* , $\epsilon$)
