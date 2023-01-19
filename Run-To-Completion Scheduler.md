---
aliases: [RTCS]
---
#programming #operating_systems #embedded_systems #ECE460 

Round-Robin based [[Scheduler (OS)|scheduler]] that doesn't allow [[Task (OS)|task]] preempting. This means that all tasks have the same priority, task function names are hard-coded into the scheduler, and each tasks makes its own decisions as to whether or not it runs. All tasks also run at the same rate, and have a fixed order of running.

>[!note]
>Tasks cannot preempt each other, and run one after the other in a round-robin format. [[Fair Scheduling (OS)|Fair Scheduling]]

## Example Code
```c
int run_foo;
int run_bar;

void scheduler(void) {
	while(1) {
		task_foo();
		task_bar();
	}
}

void task_foo() {
	if (run_foo > 0) {
		run_foo--;
		//do the foo work
	}
}

void task_bar() {
	if (run_bar > 0) {
		run_bar--;
		//do the bar work
	}
}
```
