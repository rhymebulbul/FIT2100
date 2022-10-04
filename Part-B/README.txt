 * Monash University
 * FIT2100 - Operating Systems
 * In-semester Assignment Part B
 * User Documentation
 * Created by rhyme on 23/9/22.

    ** Assumptions: * Each process has a pre-defined total service time
                    * Does not use I/O and can never be in a blocked state
                    * Will eventually run to completion and does not encounter any errors
                    * Time is measured in seconds and represented as integers
                    * Processes are listed in order of arrival time
                    * There are at most 100 processes
                    * Process names are never more than 10 characters long
                    * Process names do not contain spaces
                    * There may be more than one process that arrives at any point in time
                    * Deadline for any given process will always be greater than it's service time

    ** Usage: * Compile with gcc on the command line on linux.
              * Run with filepath as only argument, uses "processes.txt" otherwise
              * Program runs simulation while outputting entry, running and exit times of each
                process to the command line
              * Writes the results to "results-tasknum.txt" file
              * One process per line, with space-separated values
              * Each process :[Process Name] [Wait Time] [Turnaround Time] [Deadline Met]

        *** Task 1 : FCFS, First Come First Serve Scheduling
            ** Assumptions: * If more than one process arrives at any point in time, any of those
                              processes can be serviced
                            * A process should still continue to run to completion even if it does not manage
                              to meet its deadline

        *** Task 2 : RR, Round Robin scheduling with time quantum of 2
            ** Assumptions: * Please assume that newly arriving process gets higher priority (stays ahead) in
                              the ready queue if a process gets preempted at the same time.
                            * A process should still continue to run to completion even if it does not manage
                              to meet its deadline

        *** Task 3 : Deadline-based Scheduling
            ** Assumptions: *