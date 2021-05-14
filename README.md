# CPU-Efficiency

Assignment 1: Predict CPU Efficiency of HPC Cluster Jobs
In a HPC environment, users submit their scripts/programs as jobs to a Job Scheduler. Users can request for resources for their scripts/programs, e.g.: Number of CPU cores, Number of GPUs, Amount of Memory (RAM). The Job Scheduler then dispatches the user's job to remote servers (nodes) when resources are available.

The provided dataset consists of logs of completed/ended jobs. It records the requested resource values as well as actual resource consumption values of each job.

The task for this assignment is to predict the job's CPU utilisation efficiency. An ideal efficient job should use as close as possible to 100%, however realistically we define efficient CPU utilisation as above 75% of requested CPU cores.

CPU_EFF = (USED_CPUTIME / USED_WALLTIME) / REQUESTED_NCPUS
