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
This information allows so to integlrate *non-work conserving* algorithms.
The *rank* is a value compute at the insertion of a flow.
As a result, to determine if a given flow can be dequeued, we determine all elligible flow with the *predicate* and then select the flow with the minimum *rank* value.

To program the queue, three functions are proposed : `Pre-Enqueue`, `Post-Dequeue` and `alarm`.
The `Pre-Enqueue` function computes *rank* and  assign a *predicate*. 
The `Post-Dequeue` function receives a flow f as a parameter and forward the head packet of that flow. If the queue of flows f is not empty after the transmisssion, the function enqueue back the flow f to the ordered list (i.e. the FIFO of f is not empty).
The `alarm` function, which is optional, can asynchronously trigger enqueue or dequeue operations.

## expressiveness 
> TODO

## Hardware implementation
To limit the number of comparison the author stores a list of N elements over $2\*\sqrt(N)$ sublist of size $\sqrt(N)$.
In addition, a register bank, called "*Ordered-Sublist-Array*" (OSA), of size $2 \* \sqrt(N)$ stores for each sublist the minimum *rank*, the smallest *predicate*, the number of elements and the sublist id.

Thus to perform an enqueue, a sublist is selected by looking at the OSA and determing the first sublist (using a priority encoder) with a smallest rank smaller than the new rank to insert.
Also, the next sublist on the right (if not full) or an empty sublist is read to be able to store an element in case the selected sublist is full.
Since the smallest element of the sublist on the right is greater than the new element to insert, it an evidence that the global order can be garantee.
Once the sublist are read, the funciton determine where to insert the new element and then update the OSA.
> Since all the elements are ordered, it appears that the priority encoder will garantee the closest sublist.

To perform a dequeue operation, the sublist is selected by determining which one has the smallest elligible element.
Afterward the element is extracted, and the OSA updated.
To be able to dequeue a specific flow *f*, a list of flow with their coresponding sublist is kept.

> It seems that the \sqrt(N) is arbitrarly choose. However, we can consider it as a solution to optimize resource consumption since we will have the same size between OSA and sublist which allow to share comparators and other resources. If this is the reason, then only the square root function is elligible.
> As a result a question is raised : what are the right values for N to optimize HW resource usage ?



[1](https://arxiv.org/pdf/1602.06045.pdf) Programmable Packet Scheduling, Anirudh Sivaraman et al.
