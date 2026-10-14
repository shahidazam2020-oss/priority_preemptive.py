<div align="center">

# ⚡ Preemptive Priority CPU Scheduling

### A Python Implementation of Operating System Scheduling Algorithms

**Efficient Process Scheduling • Priority-Based Execution • Performance Metrics**

<p>
  <img src="https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Domain-Operating%20Systems-6C63FF?style=for-the-badge" alt="Operating Systems">
  <img src="https://img.shields.io/badge/Algorithm-Preemptive%20Priority-00A86B?style=for-the-badge" alt="Preemptive Priority">
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Project Status">
</p>

<p>
  <a href="#-overview">
    <img src="https://img.shields.io/badge/Explore-Overview-2563EB?style=for-the-badge" alt="Overview">
  </a>
  <a href="#-installation--execution">
    <img src="https://img.shields.io/badge/Run-Project-16A34A?style=for-the-badge" alt="Run Project">
  </a>
  <a href="#-algorithm-workflow">
    <img src="https://img.shields.io/badge/Learn-Algorithm-9333EA?style=for-the-badge" alt="Learn Algorithm">
  </a>
  <a href="#-connect-with-me">
    <img src="https://img.shields.io/badge/Connect-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn">
  </a>
</p>

---

**A practical Python project demonstrating how an operating system selects processes for CPU execution according to priority, handles preemption, and calculates essential scheduling performance metrics.**

</div>

## 📌 Overview

Preemptive Priority Scheduling is a CPU scheduling algorithm in which the operating system selects the highest-priority process among the processes that have arrived and are waiting for execution.

In this implementation, **a smaller priority number represents a higher priority**. When a higher-priority process arrives, it can interrupt the currently running lower-priority process.

**This project demonstrates the core concepts of CPU scheduling through a straightforward Python implementation.**

## 🎯 Project Objectives

* Understand the fundamentals of CPU scheduling in operating systems.
* Implement the Preemptive Priority Scheduling algorithm using Python.
* Manage process arrival times, burst times, and priorities.
* Calculate completion, turnaround, and waiting times.
* Determine average waiting time and average turnaround time.
* Practice algorithmic problem-solving and process management.

## ✨ Key Features

<table>
<tr>
<td width="50%">

### ⚙️ Priority-Based Scheduling

**Selects the available process with the highest priority.**

</td>
<td width="50%">

### 🔄 Process Preemption

**Allows a newly arrived, higher-priority process to interrupt execution.**

</td>
</tr>
<tr>
<td width="50%">

### 📊 Performance Metrics

**Calculates CT, TAT, and WT for every process.**

</td>
<td width="50%">

### 🧮 Average Calculations

**Computes average waiting time and turnaround time.**

</td>
</tr>
<tr>
<td width="50%">

### 🐍 Python Implementation

**Uses core Python concepts, lists, dictionaries, loops, and conditional statements.**

</td>
<td width="50%">

### 🎓 Learning-Oriented

**Suitable for operating systems coursework, programming practice, and algorithm study.**

</td>
</tr>
</table>

## 🧠 Algorithm Workflow

**The scheduling algorithm follows these steps:**

1. **Initialize processes:** Define each process's ID, arrival time, burst time, and priority.
2. **Track remaining execution time:** Maintain the remaining burst time for every process.
3. **Identify eligible processes:** Consider processes that have arrived and are not yet completed.
4. **Select the highest priority:** Choose the eligible process with the smallest priority number.
5. **Execute one time unit:** Run the selected process for one unit of CPU time.
6. **Handle preemption:** Reevaluate the available processes at the next time unit.
7. **Calculate metrics:** When a process completes, calculate its completion, turnaround, and waiting times.
8. **Display results:** Print the process scheduling table and average performance metrics.

> **Priority rule:** Priority `1` is the highest priority. A larger priority number represents a lower priority.

## 📥 Input Dataset

**The program uses the following sample processes:**

| Process ID | Arrival Time (AT) | Burst Time (BT) | Priority |
| :--------: | ----------------: | --------------: | -------: |
|     P1     |                 0 |              10 |        3 |
|     P2     |                 2 |               5 |        1 |
|     P3     |                 4 |               3 |        4 |
|     P4     |                 6 |               8 |        2 |
|     P5     |                 8 |               1 |        5 |

### 📖 Input Parameters Explained

| Parameter | Description                          |
| --------- | ------------------------------------ |
| **PID**   | Unique process identifier            |
| **AT**    | Time at which a process arrives      |
| **BT**    | Total CPU execution time required    |
| **PR**    | Priority assigned to a process       |
| **CT**    | Time at which a process completes    |
| **TAT**   | Total time spent in the system       |
| **WT**    | Time spent waiting for CPU execution |

## 📐 Scheduling Formulas

The program calculates the following metrics:

**1. Completion Time (CT)**

The time at which a process finishes execution.

**2. Turnaround Time (TAT)**

```text
TAT = CT - AT
```

**3. Waiting Time (WT)**

```text
WT = TAT - BT
```

**4. Average Waiting Time**

```text
Average WT = Sum of Waiting Times / Number of Processes
```

**5. Average Turnaround Time**

```text
Average TAT = Sum of Turnaround Times / Number of Processes
```

These metrics help evaluate how efficiently processes are scheduled.

## 🛠️ Technologies Used

| Technology                       | Purpose                         |
| -------------------------------- | ------------------------------- |
| Python 3                         | Core programming language       |
| Lists and Dictionaries           | Process data storage            |
| Loops and Conditional Statements | Scheduling logic                |
| Arithmetic Operations            | Performance metric calculations |
| Terminal / Command Prompt        | Program execution and output    |

**Dependencies:** The implementation uses Python's built-in functionality and does not require external packages.

## 🚀 Installation & Execution

### Prerequisites

* Python 3 installed on your computer.
* Git installed if you want to clone the repository.

### Step 1 — Clone the Repository

Replace `YOUR_USERNAME` with your GitHub username.

```bash
git clone https://github.com/YOUR_USERNAME/CPU-Scheduling-Algorithms.git
```

### Step 2 — Navigate to the Project Directory

```bash
cd CPU-Scheduling-Algorithms
```

### Step 3 — Run the Python Program

If your file is named `python priority_preemptive.py`, execute:

```bash
python "python priority_preemptive.py"
```

Alternatively, if you rename the file to `priority_preemptive.py`, execute:

```bash
python priority_preemptive.py
```

### Step 4 — View the Results

The program displays a process scheduling table containing:

* Process ID
* Arrival Time
* Burst Time
* Priority
* Completion Time
* Turnaround Time
* Waiting Time

It also displays the average waiting time and average turnaround time.

## 📂 Project Structure

```text
CPU-Scheduling-Algorithms/
│
├── python priority_preemptive.py
└── README.md
```

**Note:** The structure above reflects the files described in this README. Update the paths if your repository contains additional files or uses a different directory structure.

## 💡 What I Learned

This project reinforces several important concepts in computer science:

* CPU scheduling and process management.
* Preemptive scheduling techniques.
* Priority-based process selection.
* Process execution tracking.
* Calculation of scheduling performance metrics.
* Translating operating systems concepts into Python code.

## 🔮 Potential Improvements

The current implementation provides a foundation for further development. Possible enhancements include:

* **Gantt Chart Visualization:** Display process execution intervals graphically.
* **Dynamic Input:** Allow users to enter process information interactively.
* **Performance Dashboard:** Present scheduling results in a formatted table.
* **Algorithm Comparison:** Compare FCFS, SJF, Round Robin, and Priority Scheduling.
* **Tie-Breaking Rules:** Explicitly define how processes with equal priorities are handled.
* **Input Validation:** Validate arrival times, burst times, and priority values.
* **Visualization Interface:** Build a simple graphical interface to demonstrate process execution.

These are potential extensions, not features currently implemented in this version.

## 👨‍💻 Connect With Me

I'm interested in Python development, artificial intelligence, machine learning, and computer science projects.

Let's connect and explore opportunities to learn, collaborate, and build useful technology solutions.

<p align="center">
  <a href="https://github.com/shahidazam2020-oss">
    <img src="https://img.shields.io/badge/GitHub-Follow%20My%20Work-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/shahid-azam-mughal-787b58235">
    <img src="https://img.shields.io/badge/LinkedIn-Let's%20Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
</p>

---

<div align="center">

### ⭐ Support the Project

If you find this repository useful for learning CPU scheduling and operating systems concepts, consider giving it a **star** on GitHub.

**Built with Python | Designed for Learning | Open for Improvement**

</div>
