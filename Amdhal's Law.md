---
tags:
  - computer_architecture
created: 2023-09-08T14:31
updated: 2023-09-17T15:58
---
A formula which gives the theoretical [speedup](https://en.wikipedia.org/wiki/Speedup "Speedup") in [latency](https://en.wikipedia.org/wiki/Latency_(engineering) "Latency (engineering)") of the execution of a task at fixed [workload](https://en.wikipedia.org/wiki/Workload "Workload") that can be expected of a system whose resources are improved. It states that "the overall performance improvement gained by optimizing a single part of a system is limited by the fraction of time that the improved part is actually used".

>[!note] Formula
>$$S_{\text{latency}}(s)=\frac{1}{(1-p)+\frac{p}{s}}$$
>where
>$S_{\text{latency}}$ is the theoretical speed up of the whole task
>$s$ is the speed up of the part of the task that benefits most from improved system resources
>$p$ is the proportion of execution time that the part benefitting from resources originally occupied
>
>[Source](https://en.wikipedia.org/wiki/Amdahl%27s_law)	
# Considering more than one factor
$$S_{\text{latency}}(s)=\frac{1}{(1-p_1-p_2)+\frac{p_1}{s_1}+\frac{p_2}{s_2}}$$
# Applying to Parallel Units
$$S_{\text{latency}}(s)=\frac{1}{(1-p)+\frac{p}{N}}$$
where
- $S_{\text{latency}}$ is the theoretical speed up of the whole task
- $N$ is the number of parallel units
- $p$ is the proportion of execution time that the part benefitting from resources originally occupied