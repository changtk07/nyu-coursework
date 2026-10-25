# Operating Systems (NYU, Spring 2021)

Four labs for Operating Systems, NYU Spring 2021, all written in C++. The original lab specifications are in [`pdf/`](pdf/).

## Contents

| Folder | Lab | Description |
| --- | --- | --- |
| [`lab1`](lab1/) | Linker | Two-pass linker that resolves symbols and relocates module addresses |
| [`lab2`](lab2/) | Process scheduler | Discrete-event simulation of FCFS, LCFS, SRTF, Round Robin, Priority and Preemptive Priority scheduling |
| [`lab3`](lab3/) | Memory management unit | Virtual memory simulation with FIFO, Random, Clock, Enhanced Second Chance (NRU), Aging and Working Set page replacement |
| [`lab4`](lab4/) | I/O scheduler | Disk scheduling with FIFO, SSTF, LOOK, C-LOOK and F-LOOK |

## Build and run

Each lab builds with its own `Makefile`:

```sh
cd lab2
make
```

The `*_assign/` and `autograde/` folders contain the sample inputs, reference outputs and grading scripts (`runit.sh`, `gradeit.sh`) provided with each lab.
