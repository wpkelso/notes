---
tags: [parallel_computing, computer_architecture]
---

# MSI Protocol

The MSI protocol is an example of an invalidation-based [[Cache Coherence]] protocol. In it, cache block must be in one of the following states at any point in time:
- **M**odified
- **S**hared
- **I**nvalid

Requesting core:
![[Pasted image 20231001163457.png]]

Receiving cores:
![[Pasted image 20231001163505.png]]

## Shared State

The cache block contains data that is similar to that in [[Memory Block|memory]], but there could be **similar copies** on other caches.

## Modified State

The cache block contains updated data that is modified *and is the only copy.*

## Invalid State

The cache block contains outdated and unmodified data.