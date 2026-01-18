# Operating System Algorithms in C/C++ (Linux)

## Overview

This project demonstrates key Operating System algorithms implemented in **C/C++** and executed on **Ubuntu Linux**. It covers CPU scheduling, memory management, disk scheduling, process synchronization, and resource allocation, providing a practical insight into how OS components work.

## Algorithms Implemented

### 1. CPU Scheduling

* First Come First Serve (FCFS)
* Round Robin (RR)
* Shortest Job Next (SJN)
* Priority (Preemptive & Non-Preemptive)
* Shortest Time Remaining (STR) (Preemptive & Non-Preemptive)

### 2. Page Replacement

* First In First Out (FIFO)
* Least Recently Used (LRU)
* Optimal Page Replacement

### 3. Disk Scheduling

* FCFS
* Shortest Seek Time First (SSTF)
* SCAN / C-SCAN
* LOOK / C-LOOK

### 4. Deadlock & Resource Allocation

* Banker's Algorithm
* Deadlock Detection & Recovery

### 5. Process Synchronization

* Semaphores
* Mutex
* Producer-Consumer Problem
* Dining Philosophers
* Reader-Writer Problem
* Sleeping Barber Problem
* Cigarette Smoker Problem

### 6. Process Management

* fork() system call demonstration

## Environment

* **OS:** Ubuntu Linux (VirtualBox recommended)
* **Compiler:** GCC / G++
* **Languages:** C / C++

***

## How to Run

Follow these steps for compiling and running the programs in each module.

***

### 1. CPU Scheduling

```bash
cd cpu_scheduling
g++ FCFS.cpp -o fcfs
g++ ROUND_ROBIN.cpp -o rr
g++ SJN.cpp -o sjn
g++ PRIORITY.cpp -o priority_np
g++ PRIORITY_PREMP.cpp -o priority_p
g++ STR.cpp -o str_p
g++ STR_NONPREM.cpp -o str_np


# Run programs
./fcfs < input_FCFS.txt
./rr < input_RR.txt
./sjn < input_SJN.txt
./priority_np < input_PRIORITY.txt
./priority_p < input_PRIORITY_PREMP.txt
./str_p < input_STR.txt
./str_np < input_STR_NONPREM.txt
```

### 2. Page Replacement

```bash
cd ../page_replacement
g++ FIFO_REPLACEMENT.cpp -o fifo
g++ LRU.cpp -o lru
g++ OptimalPageReplacement.cpp -o optimal

# Run programs
./fifo < input_fifo.txt
./lru < input_lru.txt
./optimal < input_optimal.txt
```

### 3. Disk Scheduling

```bash
cd ../disk_scheduling
g++ DS_FCFS.cpp -o ds_fcfs
g++ DS_SSTF.cpp -o ds_sstf
g++ DS_SCAN.cpp -o ds_scan
g++ DS_CSCAN.cpp -o ds_cscan
g++ DS_LOOK.cpp -o ds_look
g++ DS_CLOOK.cpp -o ds_clook

# Run programs
./ds_fcfs < input.txt
./ds_sstf < input.txt
./ds_scan < input_SCAN.txt
./ds_cscan < input.txt
./ds_look < input_LOOK.txt
./ds_clook < input.txt
```

### 4. Banker's Algorithm & Deadlock Detection

```bash
cd ../bankers
g++ banker.cpp -o banker
g++ DeadlockDetectionAndRecovery.cpp -o deadlock

# Run programs
./banker < input.txt
./deadlock < input2.txt

```

### 5. Process Synchronization (Multithreading)

```bash
cd ../synchronization
g++ PRODUCER_CONSUMER.cpp -o producer_consumer -lpthread
g++ DINING_PHILOSOPHERS.cpp -o dining -lpthread
g++ READER_WRITER.cpp -o reader_writer -lpthread
g++ SLEEPING_BARBER.cpp -o barber -lpthread
g++ CIGARETTE_SMOKER.cpp -o smoker -lpthread
g++ SEMAPHORES.cpp -o semaphores -lpthread
g++ MUTEX.cpp -o mutex -lpthread

# Run programs
./producer_consumer
./dining
./reader_writer
./barber
./smoker
./semaphores
./mutex
```

### 6. Fork System Call Example

```bash
cd ../threading
gcc FORK.c -o fork
./fork
```

<sub><sup><span style="color:lightgrey;">Created by Sudais Khan</span></sup></sub>
