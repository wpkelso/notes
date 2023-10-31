---
tags: programming, parallel_computing, computer_architecture
created: 2023-10-25T14:23
updated: 2023-10-25T14:39
---

# Release Consistency

Release consistency is a [[Memory Consistency|memory consistency]] architecture that builds upon [[Weak Ordering]] by differentiating between the two synchronization operations, `lock` and `unlock` (or `acquire` and `release`). During a `lock` operation, older memory operations can slip in their completion time, but younger memory operations cannot be executed earlier. During an `unlock` operation, the opposite happens and younger operations can execute earlier, but older memory operations cannot slip execution time.

## Lazy-Release

In the lazy release model, the release message can be combined with the data propagation messages to improve bandwidth usage.