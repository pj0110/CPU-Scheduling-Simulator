# CPU-Scheduling-Simulator

A C++ implementation of popular CPU Scheduling Algorithms with timeline visualization and statistics generation.

## Implemented Algorithms

* FCFS (First Come First Serve)
* Round Robin (RR)
* SPN (Shortest Process Next)
* SRT (Shortest Remaining Time)
* HRRN (Highest Response Ratio Next)
* FB-1
* FB-2i
* Aging

---

## Scheduling Algorithm Comparison

| Algorithm | Preemptive | Main Idea                                  |
| --------- | ---------- | ------------------------------------------ |
| FCFS      | No         | Executes processes in arrival order        |
| RR        | Yes        | Each process gets fixed CPU quantum        |
| SPN       | No         | Shortest burst time first                  |
| SRT       | Yes        | Shortest remaining time first              |
| HRRN      | No         | Highest response ratio first               |
| FB-1      | Yes        | Multi-level feedback queue                 |
| FB-2i     | Yes        | Feedback queue with varying quantum        |
| Aging     | Yes        | Prevents starvation by increasing priority |

---

## Example Timeline Output

![CPU Scheduling Output](images/output.png)

---

## Installation

```bash
g++ *.cpp -o main.exe
```

Run:

```bash
./main.exe
```

---

## Input Format

```text
trace
1,2-3,4
20
3
P1,0,5
P2,1,3
P3,2,1
```

---

## Input Description

* Line 1 → `trace` or `stats`
* Line 2 → Scheduling algorithms
* Line 3 → Simulation time
* Line 4 → Number of processes
* Remaining lines → Process details

---

## Project Features

* Timeline Visualization
* Waiting Time Calculation
* Turnaround Time
* Normalized Turnaround Time
* Multiple Scheduling Policies
* Ready Queue Simulation

---
