---
tags:
  - parallel_computing
  - computer_architecture
created: 2023-10-01T15:42
updated: 2023-11-28T12:15
---

# MSI Protocol

The MSI protocol is an example of an invalidation-based [[Cache Coherence]] protocol. In it, cache block must be in one of the following states at any point in time:

- **M**odified
- **S**hared
- **I**nvalid

###### Requesting core:

![[Pasted image 20231001163457.png]]

###### Receiving cores:

![[Pasted image 20231001163505.png]]

## Shared State

The cache block contains data that is similar to that in [[Memory Block|memory]], but there could be **similar copies** on other caches.

## Modified State

The cache block contains updated data that is modified _and is the only copy._

## Invalid State

The cache block contains outdated and unmodified data.
