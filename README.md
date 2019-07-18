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

[(2018) Advanced Course. Go directly watch the videos on Youtube. ](https://safari.ethz.ch/architecture/fall2018/doku.php)



## FPGA
[Clock Domain Crossing](http://www.sunburst-design.com/papers/CummingsSNUG2008Boston_CDC.pdf) a course about clock domain crossing for bus and signal.

### Associative Memory

TCAM on FPGAs
[Description of the TCAM architecture used by Xilinx](https://dl.acm.org/citation.cfm?id=2537867)
Conclusion:
- FPGA are a poor fit for TCAM emulation using the transposed RAM approach.
- The overhead reported (measured as the memory size used divided by the entry size) ranges from 8.4x up to 65.3x.

TCAM and CAM VLSI:
[Content-Addressable Memory (CAM) Circuits and Architectures: A Tutorial and Survey](https://s3.amazonaws.com/academia.edu.documents/31232313/Pagiamtzis_CAM_JSSC_2006.pdf?response-content-disposition=inline%3B%20filename%3DContent-addressable_memory_CAM_circuits.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWOWYYGZ2Y53UL3A%2F20190702%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20190702T180548Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=afdb37be6159be6af242a9f35185ed7fef58ad0805d6bab6e8be12c0378c2d74)

# Papers

## Programmable Switches 

[Why programmable switches? The road to Software Defined Networking (SDN)](https://www.cs.princeton.edu/courses/archive/fall13/cos597E/papers/sdnhistory.pdf)

### Domain Specific Languages and Domain Specific Architecture

[The first step toward (limited) programmable switches: OpenFlow
](http://ccr.sigcomm.org/online/files/p69-v38n2n-mckeown.pdf)
First step: 
  - OpenFlow supports only a fixed set of network protocols. 
  - Single Match Table model.
  
From OpenFlow to P4.
- Can we design a reconfigurable and protocol agnostic parser, so that new and future protocols can be parsed without tapping out a new chip? 
 - Yes! [Design Principles for Packet Parsers](http://ccr.sigcomm.org/online/files/p69-v38n2n-mckeown.pdf)
 
 What are the missing elements to design a fully programmable switch?
 Question addressed by the paper [Forwarding Metamorphosis: Fast Programmable Match-Action Processing in Hardware for SDN](https://www3.cs.stonybrook.edu/~vyas/teaching/CSE_690-01/Fall13/papers/switchdesign.pdf)
 
The architecture presented in this paper is also refered to as PISA: Protocol Independant Switch Architecture.
 
 While this paper focuses on the hardware architecture, and introduces a domain specific architecture for networking, the language to program PISA is not addressed here.  

This is the topic of the companion paper [P4](https://arxiv.org/pdf/1312.1719.pdf).

[P4 Specification](https://p4.org/specs/)

Presentations:
- [P4_16](https://www.hotchips.org/wp-content/uploads/hc_archives/hc29/HC29.20-Tutorials-Pub/HC29.20.1-P4-Soft-Net-Pub/HC29.21.100-P4-Tutorial.pdf)
- [PSA overview](https://p4.org/assets/p4-ws-2017-p4-architectures.pdf) 
- and its [specification](https://p4.org/p4-spec/docs/PSA.html) 





#### PISA Micro-Architecture 

*Parser*:

*Match-Action*: See CAM/TCAMs.


*Deparser*:

*Packet Scheduler*:
[PIFO](https://people.csail.mit.edu/suvinay/pubs/2015.sched.hotnets.pdf)
[PIFO](https://cs.nyu.edu/~anirudh/pifo-sigcomm.pdf)

[PIEO](http://www.cs.cornell.edu/~vishal/papers/pieo_2019.pdf)

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

[Presentation guidelines](https://users.ece.cmu.edu/~pueschel/teaching/guides/guide-presentations.pdf)


