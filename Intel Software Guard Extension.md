---
tags: parallel_computing, computer_architecture, compilers, programming
---

# Intel Software Guard Extension

Intel Software Guard Extensions are a hardware based [[Memory|memory]] encryption scheme that achieves its security guarantees by partitioning [[Trusted Execution Environment|private regions]] (called enclaves in Intel terminology) for code and data to live in. This data is then decrypted on the fly in the [[Computer Processor|CPU]], meaning guarantees are made about encryption up until the point of execution.

>[!Help] 
>Further information can be found here: [Wikipedia](https://en.wikipedia.org/wiki/Software_Guard_Extensions)