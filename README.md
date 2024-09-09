# CPU-Scheduling-Simulation-in-Rust

# CPU Scheduling Simulation in Rust

This project is a Rust-based CPU scheduling simulation designed to implement and compare several CPU scheduling algorithms: **First-Come, First-Served (FCFS)**, **Round Robin (RR)**, and **Shortest Remaining Time First (SRTF)**.

## Project Overview

The simulator reads a list of tasks from an input file (`input.txt`). Each task has a process ID, an arrival time, and a CPU burst time. The simulator schedules the tasks according to the chosen algorithm and prints the task execution order and other statistics like waiting and turnaround time.

The project doesn't involve actual process creation. Instead, it simulates task scheduling and prints the execution timeline to the console.

## Implemented Scheduling Algorithms

### 1. **First-Come, First-Served (FCFS)**
The task that arrives first gets scheduled first.

### 2. **Round Robin (RR)**
Tasks are scheduled in a circular fashion with a fixed time quantum. If a task isn't completed within its quantum, it gets paused and re-added to the queue.

### 3. **Shortest Remaining Time First (SRTF)**
At every time unit, the task with the shortest remaining execution time is chosen for processing.

## Features
- **Task Scheduling:** Simulates task scheduling based on three different algorithms.
- **Metrics Calculation:** Computes average waiting time and average turnaround time for each algorithm.
- **Task Arrival Simulation:** Handles tasks arriving at different times during the simulation.
- **Idle Time Handling:** Simulates CPU idle time if no tasks are ready.

## Input Format

The input file (`input.txt`) should contain lines where each line represents a task with three fields separated by spaces


## Project Structure

src/main.rs: Contains the main logic for scheduling and the CPU simulation.

input.txt: The input file containing task details.

## Future Enhancements

Adding more scheduling algorithms (e.g., Priority Scheduling).

Visualization of task execution.

Dynamic input through user interaction or a graphical interface.
