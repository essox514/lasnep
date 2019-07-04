# Title : Fast, Scalable and Programmable Packet Scheduler in Hardware
[Vishal Shrivastav SIGCOMM 2019](http://www.cs.cornell.edu/~vishal/papers/pieo_2019.pdf)

# Author :
Vishal Shrivastav

# Summary
This paper propose a solution to tackle some limitations of Push-In-First-Out (PIFO)[1] expressiveness.
Their solution is called Push-in-Extract-Out (PIEO) and allows to extract a packet at any position in the queue.
Author claims that the proposed solution is "fast, scalable and more expressive than state-of-the-art".

## Algorithmic considerations.
> The used model is build arround the idea that each flow has it's own queue and that each queue of a flow is First-In First-Out (FIFO). 

To support a new class of scheduling the author add to the the concept of *rank* introduced by [1] the concepts of *predicates*. 
A *predicate* indicates if a given flow is elligible for scheduling.
This information allows so to integrate *non-work conserving* algorithms.
The *rank* is a value compute at the insertion of a flow.
As a result, to determine if a given flow can be dequeued, we determine all elligible flow with the *predicate* and then select the flow with the minimum *rank* value.

To program the queue, three functions are proposed : `Pre-Enqueue`, `Post-Dequeue` and `alarm`.
The `Pre-Enqueue` function computes *rank* and  assign a *predicate*. 
The `Post-Dequeue` function receives a flow f as a parameter and forward the head packet of that flow. If the queue of flows f is not empty after the transmisssion, the function enqueue back the flow f to the ordered list (i.e. the FIFO of f is not empty).
The `alarm` function, which is optional, can asynchronously trigger enqueue or dequeue operations.


## Hardware implementation
The author considers that a packet scheduler consist into First-In First-Out (FIFO) queues where each queue contain packet of the same flow.
To allow scalability, author splits accros multiple SRAM blocks the informations.
The announced complexity order is $O(\sqrt{N})$ with N the list size with a constant time to enqueue and dequeue values.

	
# Consideration


[1](https://arxiv.org/pdf/1602.06045.pdf) Programmable Packet Scheduling, Anirudh Sivaraman et al.
