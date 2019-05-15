# Title : Your Programmable NIC Should be a Programmable Switch
[panic hotnets 2018](https://www.cs.uic.edu/~brents/docs/panic.hotnets18.pdf)

# Authors :
Brent Stephens, Aditya Akella, Michael M. Swift

# Summary
This paper propose a new design for Network Interface Cards (NICs).
Authors are proposing a NIC that limits head of line blocking, high latency inherent to many core architecture and allow complex offload unlike RMT piepeline.
To do so, the NIC is designed arround three different types of components :
- different types of offload engines
- a logical switch
- a logical scheduler
When a packet is processed, it is analyzed by an RMT core that determines all the offload engines the packet should go through.
Each engine contains a local scheduler that determine which packet should be processed by the particular engine.
Also to accelerate transmission between engine and because is is a mesh network, each engine contains a local router that can directly forward packet to the next engine is no process has to be done in the current engine.

# Critics
The proposed architecture can not garantee that every packet will be processed at line rate.
So some assumptions have to be taken into consideration concerning incomming traffic.
For example, authors claim that IPSec can not be done at line rate.
However in there design if all the packets that go through the NIC are IPSec then congestion will happen.

Another point is that the paper present a Network on Chip that let communicate multiple engines.
THe author do not reference any previous work regarding this aspect.
