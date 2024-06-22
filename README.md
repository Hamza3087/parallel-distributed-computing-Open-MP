# parallel-distributed-computing-Open-MP

1. Serial Version: Students will implement a program to
i. read a list of numbers from file and store them in an array,
ii. insert the individual numbers into a linked list,
iii. and sort the linked list using merge sort

2. Parallel Version with CPU Affinity:
o Create a pthread function to add roll numbers into the linked list concurrently.
Each thread will handle a subset of the roll numbers.
o Implement a pthread function to parallelize the merge sort algorithm on the
linked list. Threads will work on different portions of the list during the merge
sort process.

o incorporate pthread_setaffinity_np for setting CPU affinity on a per-
thread basis. Each thread in the parallel version will be mapped to a specific

CPU core using pthread_setaffinity_np
i. plan and implement the mapping of threads to specific CPU cores
using the CPU affinity concept, exploiting sched_setaffinity
function calls.
ii. Utilize pthread_setaffinity_np to set CPU affinity for each thread,
specifying the CPU cores they should be bound to.

Thread Mapping Plan:
o Before implementing the parallel version, students should analyze the system's
architecture and come up with a plan for mapping threads to specific CPU cores.
o Consider factors such as the number of available cores, workload distribution,
and potential resource contention.
