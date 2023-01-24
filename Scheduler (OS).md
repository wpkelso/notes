#programming #operating_systems #embedded_systems

A central part of an [[Operating System|operating system]], the scheduler determines which [[Task (OS)|tasks]] to run, and for how long. Task execution may have a seemingly arbitrary order of execution, often with interleaving and preemption. Often a scheduler will be used in conjunction with an [[Interrupt|interrupt]]-based system to allow for greater responsiveness.

![[Pasted image 20221108150916.png]]

>[!example] Types of Schedulers
> [[Run-To-Completion Scheduler|Run-to-Completion]]: Doesn't allow preempting, only sequential
