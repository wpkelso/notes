---
tags: [programming]
---
[[Variable]] shadowing is a concept in the Rust programming language, whereby a a variable can be declared with the same name as a previous variable. This second variable then maintains its value until either it goes out of scope or is shadowed itself. This is separate from an [[Variable Mutability|immutable variable]], as a compile-time error will be thrown should an attempt be made to modify the variable without further use of ```let```.

In Rust, this action is completed by declaring the variable again using the ```let``` keyword.