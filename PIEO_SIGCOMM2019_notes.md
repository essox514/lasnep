# Title : Fast, Scalable and Programmable Packet Scheduler in Hardware
[Vishal Shrivastav SIGCOMM 2019](http://www.cs.cornell.edu/~vishal/papers/pieo_2019.pdf)

# Author :
Vishal Shrivastav

# Summary
This paper propose a solution to tackle some limitations of Push-In-First-Out (PIFO)[1] expressiveness.
Their solution is called Push-in-Extract-Out (PIEO) and allows to extract a packet at any position in the queue.
Author claims that the proposed solution is "fast, scalable and more expressive than state-of-the-art".

The author considers that a packet scheduler consist into First-In First-Out (FIFO) queues where each queue contain packet of the same flow.
To allow scalability, author splits accros multiple SRAM blocks the informations.
The announce complexity order is 
$O(\sqrt{N}gg)$ with N the list size.

# Critics


[1](https://arxiv.org/pdf/1602.06045.pdf) Programmable Packet Scheduling, Anirudh Sivaraman et al.
