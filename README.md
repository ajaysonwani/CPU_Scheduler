# CPU Scheduler
## Overview
This repository contains the implementation of various CPU scheduling algorithms used in operating systems. CPU scheduling is a vital process that ensures efficient execution of processes by managing the order and time in which the CPU is assigned to them. This project demonstrates different scheduling techniques and provides a simulation of how each algorithm works.

## Features
#### First-Come, First-Served (FCFS): 
Simplest scheduling algorithm that executes processes in the order they arrive.
#### Shortest Job First (SJF):
Selects the process with the smallest execution time.
Priority Scheduling: Executes processes based on priority, where higher priority processes are executed first.
#### Round Robin (RR):
Each process is assigned a fixed time in a cyclic order.
#### Shortest Remaining Time First (SRTF) Scheduling:
Shortest Remaining Time First (SRTF) is a preemptive scheduling algorithm that selects the process with the smallest amount of time remaining until completion. SRTF is essentially the preemptive version of the Shortest Job Next (SJN) algorithm.
## Deployment

To run the project, follow these steps:

Clone the repository : 
```bash
git clone https://github.com/ajaysonwani/CPU_Scheduler.git
```

Compile the code:
```bash
 g++ -o scheduler scheduler2.cpp
 ```
Run the executable: 
```bash
./scheduler input.txt output.txt
```
## Internal Working
### FCFS (First-Come, First-Served)
**Arrival**: Sort processes by arrival time.

**Execution**: Execute processes in the order they arrive.

**Completion**: Calculate waiting time and turnaround time for each process.

**Output**: Output average waiting time and turnaround time.

### SJF (Shortest Job First)
**Arrival**: Sort processes by arrival time.

**Execution**: Select the process with the shortest burst time among the arrived processes.

**Completion**: Calculate waiting time and turnaround time for each process.

**Output**: Output average waiting time and turnaround time.

### SRTF (Shortest Remaining Time First)
**Arrival**: Sort processes by arrival time.

**Execution**: Select the process with the shortest remaining time among the arrived processes.

**Preemption**: If a shorter job arrives, preempt the current job.

**Completion**: Calculate waiting time and turnaround time for each process.

**Output**: Output average waiting time and turnaround time.

### Round Robin
**Arrival**: Maintain a ready queue.

**Execution**: Execute each process for a fixed time quantum.

**Preemption**: If the process's quantum expires, move it to the end of the queue.

**Completion**: Calculate waiting time and turnaround time for each process.

**Output**: Output average waiting time and turnaround time.

## Learning Takeaways
Understanding of different CPU scheduling algorithms and their implementation in C++.

Hands-on experience with process management and scheduling in an operating system.

Importance of algorithm choice in optimizing CPU utilization and response time.

## Resources/References
Operating System Concepts by Abraham Silberschatz, Peter Baer Galvin, and Greg Gagne

GeeksforGeeks articles on CPU Scheduling Algorithms
