# CPU Scheduling Algorithms: Round Robin and Preemptive Priority Scheduling

This program implements two CPU scheduling algorithms: Round Robin and Preemptive Priority Scheduling. It simulates the scheduling process for a given set of processes with specified burst times and priorities.

## Features

- **Round Robin Scheduling**: Executes processes in a cyclic order based on a given time quantum.
- **Preemptive Priority Scheduling**: Executes processes based on their priority, preempting the CPU if a higher priority process arrives.

## Getting Started

### Prerequisites

- A C++ compiler (e.g., g++)

### Installation

1. Clone this repository or download the source code.
2. Navigate to the directory where the source code is located.

## Code Explanation
Round Robin Scheduling
The roundRobinScheduling function takes a vector of processes and a time quantum. It simulates the Round Robin scheduling algorithm by executing each process for a maximum of the given time quantum, then moving to the next process in the queue.

Preemptive Priority Scheduling
The priorityScheduling function takes a vector of processes. It simulates the Preemptive Priority Scheduling algorithm by always executing the process with the highest priority (lowest priority number) that is ready to run. If a process with a higher priority arrives, it preempts the current process.

Main Function
Prompts the user for the number of processes.
Reads the burst time and priority for each process.
Reads the time quantum for Round Robin Scheduling.
Calls the roundRobinScheduling function to execute processes using the Round Robin algorithm.
Calls the priorityScheduling function to execute processes using the Preemptive Priority Scheduling algorithm.

### Compilation

To compile the program, run the following command in your terminal:

```bash
g++ -o scheduling scheduling.cpp
Example Usage
Enter the number of processes: 3
Enter details for each process:
Process 1 Burst time: 5
Priority: 1
Process 2 Burst time: 9
Priority: 3
Process 3 Burst time: 6
Priority: 2
Enter the time quantum for Round Robin Scheduling: 4

Executing process 1 for time 4
Executing process 2 for time 4
Executing process 3 for time 4
Executing process 1 for time 1
Executing process 3 for time 2
Executing process 2 for time 5

Average waiting time for Priority Scheduling: 5.66667
