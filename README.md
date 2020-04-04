# operating-system
sem4
 Use the following constants to identify the range of possible pid values: 
 #define MIN PID 100  
 #define MAX PID 1000  
 You may use any data structure of your choice to represent the availability   of process identifiers. 
 One strategy is to adopt what Linux has done and use   a bitmap in which a value of 0 at position i indicates that a process id of   value i is available and a value of 1 indicates that the process id is currently in use. 
 Implement the following API for obtaining and releasing a pid:  
 • int allocate map(void)—Creates and initializes a data structure for representing pids; 
 returns—1 if unsuccessful, 1 if successful  
 • int allocate pid(void)—Allocates and returns a pid; 
 returns— 1 if unable to allocate    a pid (all pids are in use) 
 • void release pid(int pid)—Releases a pid   
 Modify the above problem by writing a multithreaded program that tests your solution. 
 
 
 
 We used threads:- 
What are threads? 
A thread is a flow of execution through the process code, with its own program counter that keeps track of which instruction to execute next, system registers which hold its current working variables, and a stack which contains the execution history. A thread shares with its peer threads few information like code segment, data segment and open files. When one thread alters a code segment memory item, all other threads see that. A thread is also called a lightweight process. Threads provide a way to improve application performance through parallelism. Threads represent a software approach 
to improving performance of operating system by reducing the overhead thread is equivalent to a classical process. Each thread belongs to exactly one process and no thread can exist outside a process. Each thread represents a separate flow of control. Threads have been successfully used in implementing network servers and web server. They also provide a suitable foundation for parallel execution of applications on shared memory multiprocessors. The following figure shows the working of a single-threaded and a multithreaded process. 
 
