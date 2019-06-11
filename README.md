# LASNEP Research Lab 
Reference Courses, Papers and Ressources on the topic of: Networking, Operating System , Algorithms, Languages, Computer Architecture and FPGA. Also contains ressources for graduates students. 


# Courses and Books 

## Networking

These two courses are taught at NYU by Anirudh Sivaraman.

Introduction Course on [Computer Networks CSCI-UA.0480-009](https://cs.nyu.edu/courses/fall17/CSCI-UA.0480-009/)

Graduate Course on [Networks and Mobile Systems CSCI-GA.2620-001](https://cs.nyu.edu/courses/spring18/CSCI-GA.2620-001/), with an emphasis on current research challenges in the field of computer networks.


## Operating System

-[Operating System Concepts](http://iips.icci.edu.iq/images/exam/Abraham-Silberschatz-Operating-System-Concepts---9th2012.12.pdf) is a reference book used in most courses.

-[MIT 6.828 Operating System Engeeneering](https://pdos.csail.mit.edu/6.828/2018/schedule.html)


## Algorithms 

-Reference book [The Algorithm Design Manual](http://mimoza.marmara.edu.tr/~msakalli/cse706_12/SkienaTheAlgorithmDesignManual.pdf)

-[Design and Analysis of Algorithms CS161](http://web.stanford.edu/class/cs161/)

-[CS166 Advanced Data Structure](http://web.stanford.edu/class/cs166/)





## Languages


## Computer Architecture




## FPGA

### Associative Memory

TCAM on FPGAs
[Description of the TCAM architecture used by Xilinx](https://dl.acm.org/citation.cfm?id=2537867)
Conclusion:
- FPGA are a poor fit for TCAM emulation using the transposed RAM approach.
- The overhead reported (measured as the memory size used divided by the entry size) ranges from 8.4x up to 65.3x.

# Papers

## Programmable Switches 

### Domain Specific Language

OpenFlow

[P4 Orginial Paper](https://arxiv.org/pdf/1312.1719.pdf).

[P4 Specification](https://p4.org/specs/)

Presentations:
- [P4_16](https://www.hotchips.org/wp-content/uploads/hc_archives/hc29/HC29.20-Tutorials-Pub/HC29.20.1-P4-Soft-Net-Pub/HC29.21.100-P4-Tutorial.pdf)
- [PSA overview](https://p4.org/assets/p4-ws-2017-p4-architectures.pdf) 
- and its [specification](https://p4.org/p4-spec/docs/PSA.html) 

POF

Clarify the differences between them. 

### Domain Specific Architecture

[PISA, Protocol Independant Switch Architecture](http://yuba.stanford.edu/~grg/docs/sdn-chip-sigcomm-2013.pdf)

### In-Network Computing

Programmable switches can be used as a computing platform for distribued applications. 

[A review of previous in-network computing works by the IETF COIN (Computing In the Network) group](https://tools.ietf.org/pdf/draft-he-coin-datacenter-00.pdf)

Some applications offloaded on programmable switches were shown to be accelerated by up to two order of magnitude in terms of throughput, latency and power-efficiency.

However, multiple researcher raised concerns about offloading distributed applications on programmable switchs. Most notably, the following questions were raised.
1)[How programmable switches should be used (vs can be used)](https://people.eecs.berkeley.edu/~apanda/assets/papers/LoadBalancing.pdf)
2)[Which applications can benefits from in-network computing?](https://drkp.net/papers/innetwork-hotos19.pdf)



# Developpment Ressources 

# Graduate Students Ressources

Reflexion on Research

[You and your research](https://www.site.uottawa.ca/~yymao/misc/Hamming_kaiser.html)

[Reading a Paper](https://blizzard.cs.uwaterloo.ca/keshav/home/Papers/data/07/paper-reading.pdf)

[Writting a Paper](https://www.microsoft.com/en-us/research/academic-program/write-great-research-paper/)

[Table presentation](https://inf.ethz.ch/personal/markusp/teaching/guides/guide-tables.pdf)

[Presenting a Paper](https://www.microsoft.com/en-us/research/academic-program/give-great-research-talk/)


