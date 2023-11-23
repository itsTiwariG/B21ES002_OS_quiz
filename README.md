# XV Quiz (CSL 3030)

Welcome to the XV Quiz for CSL 3030 - Operating Systems!



## Instructions
- Answer the multiple-choice questions by selecting the correct option.
- For theoretical questions, provide concise and accurate explanations.
- Feel free to use this quiz for self-assessment or educational purposes.

## Multiple-Choice Questions

#### Question 1: Basics
1. What is XV6?
   - a. A programming language
   - b. A Unix-like operating system
   - c. A file system
   - d. An assembly language

#### Question 2: Architecture
2. XV6 is based on which earlier operating system?
   - a. Windows
   - b. Linux
   - c. BSD
   - d. DOS

#### Question 3: File System
3. Which file system is used in XV6?
   - a. FAT32
   - b. NTFS
   - c. ext4
   - d. simple

#### Question 4: System Calls
4. How are system calls implemented in XV6?
   - a. As functions in the C standard library
   - b. As interrupts
   - c. Through the command line
   - d. As external programs

#### Question 5: Processes
5. In XV6, what is the maximum number of processes that can run simultaneously?
   - a. 128
   - b. 256
   - c. 512
   - d. 1024

#### Question 6: Shell
6. What is the name of the shell used in XV6?
   - a. Bash
   - b. Zsh
   - c. Sh
   - d. Fish

#### Question 7: Scheduling
7. How does XV6 handle process scheduling?
   - a. Round-robin scheduling
   - b. Priority-based scheduling
   - c. First-Come-First-Serve (FCFS)
   - d. Random scheduling

#### Question 8: Memory Management
8. Which memory management technique is used in XV6?
   - a. Paging
   - b. Segmentation
   - c. Virtual Memory
   - d. None of the above

#### Question 9: Interrupts
9. How are interrupts handled in XV6?
   - a. Through polling
   - b. Using hardware interrupts
   - c. Using software interrupts
   - d. Both b and c

#### Question 10: Multithreading
10. Does XV6 support multithreading?
    - a. Yes
    - b. No

#### Bonus Question:
11. Who developed XV6?
    - a. Microsoft
    - b. Google
    - c. MIT
    - d. IBM

## Theoretical Questions

#### Question 12: Process States
12. Briefly explain the different states a process can be in within the XV6 operating system.

#### Question 13: File System Structure
13. Describe the structure of the file system in XV6. Include the key components and their roles.

#### Question 14: System Calls vs. Library Functions
14. Explain the difference between system calls and library functions in the context of XV6. Provide examples of each.

#### Question 15: Memory Paging
15. How does memory paging work in XV6? Discuss the benefits of using paging in memory management.

#### Question 16: Shell Commands
16. Name and briefly explain three essential shell commands in the XV6 operating system.

#### Question 17: Process Synchronization
17. Discuss the concept of process synchronization in XV6. Why is it essential, and what mechanisms are used to achieve it?

#### Question 18: Interrupt Handling
18. Explain the role of interrupts in the XV6 operating system. How are interrupts handled, and what is their significance in system operation?

#### Question 19: Virtual Memory
19. What is virtual memory, and how is it implemented in XV6? Discuss the advantages of using virtual memory.

#### Question 20: Boot Process
20. Outline the steps involved in the boot process of XV6. What happens from the moment the computer is powered on to when the XV6 kernel is loaded into memory?

## Answers
Please write your answers here
1. c Unix Like Operating system
2. b Linux
3. d. simple
4. b interrupts
5. a 64 (maximum number of processes that can run is NPROC = 64)
6. c. Sh
7. a. Round-Robin Scheduling
8. a. Paging
9. d. both b and c
10. a. Yes
11. c. MIT
12. {UNUSED:- The process has been created but not scheduled yet.
    EMBRYO :- The process is in the state of being created. SLEEPING:- The process is waiting for I/O operation or timer interrupt has occured.
    RUNNABLE:- The process can be scheduled for running. RUNNING:- The process has currently occupied the CPU. ZOMBIE:- The process has finished its execution, parent process is waiting for its exit status.}
13. ahbs
14. System calls provide a way for user-level processes to interact with the lower-level functionalities of the operating system, which are typically implemented in the kernel.Examples :- fork(), exit(), pipe() etc.
    Library functions are higher-level functions provided by libraries that are linked to user-level programs. These functions are written in user space and are not part of the operating system kernel.
 Examples :- printf(),cprintf(),malloc() etc.
15.In XV6, memory paging divides virtual and physical memory into fixed-size pages, managed by two-level page tables. Paging allows for virtual memory, memory isolation, efficient use of physical memory, and dynamic memory allocation. It simplifies address translation and facilitates page faults and replacement when needed.
16. ls:- list all the files in the current directory, cd:- used to change the current working directory, cp:- used to copy files from one directory to another.
17. Spinlocks: Basic lock for mutual exclusion.
        Semaphores: Higher-level synchronization primitive.
        Condition Variables: Used for signaling between processes.
    Importance: Prevents data corruption, avoids race conditions, ensures orderly execution, and maintains system stability.
18.    Role: Signals to the CPU for immediate attention.
    Handling: Managed by ISRs in the Interrupt Vector Table.
    Significance:
        Efficient I/O handling.
        Real-time responsiveness.
        Supports concurrency and multitasking.
        Facilitates device interaction.

