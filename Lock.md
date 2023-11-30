---
tags: parallel_computing, computer_architecture, programming, software
created: 2023-11-30T16:47
updated: 2023-11-30T17:34
---

# Lock
## Implementations

### Test and Set Lock

```asm
lock:   t&s R1, &lockvar // R1 = lockvar
        bnz R1, lock
```

## Performance Evaluation of Implementations

To evaluate the various implementations of locks, consider the following set of criteria:

1. **Uncontended lock-acquisition latency:** the time it takes to acquire a lock when there is no contention between threads
2. **Traffic:** the amount of traffic generated as a function of number of threads or processors that contend for the lock.
    1. Traffic on _lock acquisition when a lock is free_
    2. Traffic on _lock acquisition when a lock is not free_
    3. Traffic on _lock release_
3. **Fairness:** the degree in which threads are allowed to acquire locks with respect to one another.
    - _i.e._ whether or not in the implementation it is possible to for a thread to be _starved_ (unable to acquire a lock for a long period of time even when the lock became free during that time)
4. **Storage:** the amount of storage needed as a function of number of threads.
