Reference Courses, Papers and Ressources on the topic of: Networking, Operating System , Algorithms, Languages, Computer Architecture and FPGA. Also contains ressources for graduates students. 

---

Table of Contents
=================

   * [High Speed and Programmable Packet Processing](#high-speed-and-programmable-packet-processing)
   * [Courses and Books](#courses-and-books)
      * [Networking](#networking)
         * [5G](#5g)
         * [Blogs and news](#blogs-and-news)
      * [Operating System](#operating-system)
      * [Algorithms](#algorithms)
      * [Languages](#languages)
         * [C  ](#c)
         * [Python](#python)
         * [RTL](#rtl)
            * [VHDL](#vhdl)
            * [Verilog](#verilog)
            * [Modern Hardware Description Languages](#modern-hardware-description-languages)
            * [Tools](#tools)
      * [Computer Architecture](#computer-architecture)
         * [Generic](#generic)
         * [Networking](#networking-1)
      * [FPGA](#fpga)
         * [Blogs and News](#blogs-and-news-1)
         * [Associative Memory](#associative-memory)
   * [Papers](#papers)
      * [Router Buffers](#router-buffers)
      * [Programmable Switches](#programmable-switches)
         * [Context](#context)
         * [Domain Specific Architecture](#domain-specific-architecture)
         * [Domain Specific Language](#domain-specific-language)
            * [P4 Compilation](#p4-compilation)
            * [PISA Micro-Architecture](#pisa-micro-architecture)
         * [In-Network Computing](#in-network-computing)
   * [High-Level Synthesis](#high-level-synthesis)
   * [High Speed I/O Framework for Software Packet Processing](#high-speed-io-framework-for-software-packet-processing)
   * [Network Traffic Traces](#network-traffic-traces)
   * [Developpment Ressources](#developpment-ressources)
   * [Conferences / Journal](#conferences--journal)
      * [Networking](#networking-2)
      * [Computer Architecture](#computer-architecture-1)
         * [FPGA](#fpga-1)
         * [All remainings topics](#all-remainings-topics)
   * [Graduate Students Ressources](#graduate-students-ressources)
      * [Reflexion on Research](#reflexion-on-research)
      * [Bibliography manager](#bibliography-manager)
      * [Reading a paper](#reading-a-paper)
      * [Writting a Paper](#writting-a-paper)
      * [Presenting a Paper](#presenting-a-paper)
      * [Presenting your research on your website](#presenting-your-research-on-your-website)
      * [Religion - Emacs](#religion---emacs)

---

# Courses and Books 

## Networking

These two courses are taught at NYU by Anirudh Sivaraman.

Introduction Course on [Computer Networks CSCI-UA.0480-009](https://cs.nyu.edu/courses/fall17/CSCI-UA.0480-009/)

Graduate Course on [Networks and Mobile Systems CSCI-GA.2620-001](https://cs.nyu.edu/courses/spring18/CSCI-GA.2620-001/), with an emphasis on current research challenges in the field of computer networks.

Another [computer network course](http://web.mit.edu/6.829/www/currentsemester/lectures_gen.html) taught at MIT. This is a graduate-level introduction to classic and advanced topics in computer networks.

[Advanced Topics in Networking from MIT (2016)](https://people.csail.mit.edu/alizadeh/courses/6.888/index.html)

[Nick Mckeown Course - Advanced Topics in Networking](http://web.stanford.edu/class/cs244/)

If you prefer to watch videos, the content of the course COS 461 - Computer Networking (Princeton) is available on [Youtube](https://www.youtube.com/playlist?list=PLpherdrLyny-zJw95jcE-uJkcsIAG1MEn).

### 5G

[5G Mobile Networks: A Systems Approach](https://5g.systemsapproach.org/index.html)

### Blogs and news

[OvSorbit](https://ovsorbit.org/) a podcast related to OvS (Open vSwitch), an open-source implementation of a distributed virtual multilayer switch. The main purpose of Open vSwitch is to provide a switching stack for hardware virtualization environments, while supporting multiple protocols and standards used in computer networks.

## Operating System

-[Operating System Concepts](http://iips.icci.edu.iq/images/exam/Abraham-Silberschatz-Operating-System-Concepts---9th2012.12.pdf) is a reference book used in most courses.

-[MIT 6.828 Operating System Engeeneering](https://pdos.csail.mit.edu/6.828/2018/schedule.html)

-[UW–Madison Operating Systems: Three Easy Pieces](http://pages.cs.wisc.edu/~remzi/OSTEP/)


## Algorithms 

-Reference book [The Algorithm Design Manual](http://mimoza.marmara.edu.tr/~msakalli/cse706_12/SkienaTheAlgorithmDesignManual.pdf)

-[Design and Analysis of Algorithms CS161](http://web.stanford.edu/class/cs161/)

-[CS166 Advanced Data Structure](http://web.stanford.edu/class/cs166/)





## Languages

### C++

For modern C++ please use the [C++ Core Guidelines](http://isocpp.github.io/CppCoreGuidelines/CppCoreGuidelines), the book ["A Tour of C++"](https://github.com/maybez/maybe/blob/master/Books/C++/A%20Tour%20of%20C++/A%20Tour%20of%20C++.pdf).

For a more complete list of C++ resources, check [Awesome CPP](https://awesomecpp.com/).

### Python

[Fundamentals of Python Programming](https://python.cs.southern.edu/pythonbook/pythonbook.pdf)

### RTL

#### VHDL 

[VHDL Cookbook](https://www.ics.uci.edu/~alexv/154/VHDL-Cookbook.pdf)

[VHDL Language Reference Manual (VHDL 2008)](ftp://ftp.lpp.polytechnique.fr/jeandet/keep/sync/vhdl/4772740_IEEE-1076_Standard-VHDL-Language-Ref-Manual.pdf)

#### Verilog 

[Verilog, Formal Verification and Verilator Beginner's Tutorial](https://zipcpu.com/tutorial/). This tutorial has pointers to other tutorials.

#### Modern Hardware Description Languages 

See the related projects section on [PyRTL](https://ucsbarchlab.github.io/PyRTL/). 
The page covers the following HDL: [myHDL](http://www.myhdl.org), [Chisel](https://chisel.eecs.berkeley.edu), [PyMTL](https://github.com/cornell-brg/pymtl), [Clash](https://clash-lang.org).

Paper: A Golden Age of Hardware Description Languages: Applying Programming Language Techniques to Improve Design Productivity [Link](http://drops.dagstuhl.de/opus/volltexte/2019/10550/pdf/LIPIcs-SNAPL-2019-7.pdf)

[Spatial: an Argon DSL for programming reconfigurable hardware from a parameterized, high level abstraction.](https://spatial-lang.org/control-flow)


#### Tools 

Open source tools (May be outdated. [Link](http://www.fabienm.eu/flf/open-source-fpga-map/)).

In particular, [CocoTB](https://github.com/cocotb/cocotb) is of high interest if you want to test your design with a Python testbench.

To have an update on open-source tools, checks the ORConf talks [link to conference website](https://orconf.org)

## Computer Architecture


### Generic 

Introduction course for undergrades, or for a refresh. [Link to the course material (check also the video on youtube)](https://safari.ethz.ch/digitaltechnik/spring2018/doku.php?id=schedule)

(2018) Advanced Course for graduate students. [Link to the course material (see also the video on youtube)](https://safari.ethz.ch/architecture/fall2018/doku.php)

Reference books (read in this order):
David A Patterson and John L. Hennessy "Computer Organization and Design: the Hardware/Software Interface"

John L. Hennessy and David A Patterson  "Computer Architecture: A Quantitative Approach"

### Networking

An old (may be outdated) reference to the design of network processors (NPU). [High Performance Switches and Routers](http://rozup.ir/up/netit/Documents/Term3/roostazade/hsn/E-Book/0.pdf)
Please note that NPUs were designed to offer higher processing flexibility over P4-programable data plane (see article below Forwarding Metamorphosis). Hence, NPUs could barely process 200/400 Gbps, while PISA was shown to process Tbps. However, the PISA processing capabilities are restrained over a NPU. PISA is not tailored to process more than 512 bytes of the packet header (no payload processing allowed). 

## FPGA

### Blogs and News
[Zipcpu: the blogs covers many classics topics related to FPGA: bus, AXIs, clock domain crossing, PLL, etc. (In Verilog)](https://zipcpu.com)
[Front de libération des FPGAs (french)](http://www.fabienm.eu/flf/)

[Designing parallel computers and integrated systems-on-chips using FPGAs](http://fpga.org)

[Clock Domain Crossing](http://www.sunburst-design.com/papers/CummingsSNUG2008Boston_CDC.pdf) a course about clock domain crossing for bus and signal.

### Associative Memory

TCAM on FPGAs
[Description of the TCAM architecture used by Xilinx](https://dl.acm.org/citation.cfm?id=2537867)
Conclusion:
- FPGA are a poor fit for TCAM emulation using the transposed RAM approach.
- The overhead reported (measured as the memory size used divided by the entry size) ranges from 8.4x up to 65.3x.

TCAM and CAM VLSI:
[Content-Addressable Memory (CAM) Circuits and Architectures: A Tutorial and Survey](https://s3.amazonaws.com/academia.edu.documents/31232313/Pagiamtzis_CAM_JSSC_2006.pdf?response-content-disposition=inline%3B%20filename%3DContent-addressable_memory_CAM_circuits.pdf&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWOWYYGZ2Y53UL3A%2F20190702%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20190702T180548Z&X-Amz-Expires=3600&X-Amz-SignedHeaders=host&X-Amz-Signature=afdb37be6159be6af242a9f35185ed7fef58ad0805d6bab6e8be12c0378c2d74)

---

# Papers

## Router Buffers

Past, present and future perspectiveso on [sizing router buffers](https://ccronline.sigcomm.org/wp-content/uploads/2019/10/acmdl19-339.pdf).


## Programmable Switches 

A broad selection of papers published on the topic of programmable switches is available [here](https://rg0now.github.io/prog_dataplane_reading_list/README.html#org7f978d7). 

A concise version is presented below. 



### Context

[Why programmable switches? The road to Software Defined Networking (SDN)](https://www.cs.princeton.edu/courses/archive/fall13/cos597E/papers/sdnhistory.pdf)

[A cornerstone paper in modern network hardware design? Yes, there is one!](http://conferences.sigcomm.org/hotnets/2008/papers/1.pdf)

[Where Programmable switches fit in the global picture SDN?](https://www.youtube.com/watch?v=YHeyuD89n1Y)

[An attempt to motivate and clarify Software-Defined Networking (SDN)](https://www.youtube.com/watch?v=WVs7Pc99S7w)

[Why programmable switches are here to stay? A very good presentation by Nick Mckeown.](https://www.youtube.com/watch?v=8ie0FcsN07U)

[Historic Perspective: From Ethane To SDN and Beyond](https://ccronline.sigcomm.org/wp-content/uploads/2019/10/acmdl19-347.pdf). A brief description on the history behind the Ethane paper and its ultimate evolution into SDN and beyond.

### Domain Specific Architecture

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

The Domino paper raises the question of the processing capabilities that sould be integrated in a programable switch (implemented on ASIC). [Link to the Domino paper](https://dl.acm.org/citation.cfm?id=2934900). 
 
While previously presented paper focus on the hardware architecture, the language to program PISA is not addressed here. This is the topic of another paper, P4, see below.

### Domain Specific Language 
First, we highly recommand you to read the [P4 paper](https://arxiv.org/pdf/1312.1719.pdf).

Then, the tutorial [getting started with P4](https://github.com/p4lang/education/blob/master/GettingStarted.md), provided by the P4 Education working group is a good indroduction on P4, and presents examples using the [bmv2, the behavioral model for P4](https://github.com/p4lang/behavioral-model). A more complete tutorial on P4 programming is provided [on the P4 language repo](https://github.com/p4lang/tutorials).

More resources on P4 are available on the [P4 Educational Working Group](https://github.com/p4lang/education). The latest [P4 Specification is available here](https://p4.org/specs/).




Presentations:
- [P4_16](https://www.hotchips.org/wp-content/uploads/hc_archives/hc29/HC29.20-Tutorials-Pub/HC29.20.1-P4-Soft-Net-Pub/HC29.21.100-P4-Tutorial.pdf)
- [PSA overview](https://p4.org/assets/p4-ws-2017-p4-architectures.pdf) 
- and its [specification](https://p4.org/p4-spec/docs/PSA.html) 

#### P4 Compilation 

*to FPGA*

P4FPGA : An open-source P4 compiler for FPGAs (P4 -> BlueSpec). The git repo is no longer maintained. 
Complete reference: Wang, Han, Robert Soulé, Huynh Tu Dang, Ki Suh Lee, Vishal Shrivastav, Nate Foster, and Hakim Weatherspoon. "P4FPGA: A rapid prototyping framework for P4." In Proceedings of the Symposium on SDN Research, pp. 122-135. ACM, 2017.
Link to the paper [P4FPGA](http://www.cs.yale.edu/homes/soule/pubs/sosr17-p4fpga.pdf)

Xilinx SDNet. See [P4-NetFPGA](https://github.com/NetFPGA/P4-NetFPGA-public)

*to CPU*

P4C (P4 Compiler)[https://github.com/p4lang/p4c] compiles P4 programs for the bmv2 (Behavioral Model 2)[https://github.com/p4lang/behavioral-model]. Note that the bmv2 is *not* intended to be a fast CPU target (i.e. run a P4 program fast), as the bmv2 is a *BEHAVIROAL MODEL*.

#### PISA Micro-Architecture 

*Parser*:

*Match-Action*: See CAM/TCAMs.


*Deparser*:

*Packet Scheduler*:
The first paper on this topic, [PIFO @HotNets](https://people.csail.mit.edu/suvinay/pubs/2015.sched.hotnets.pdf). The longer version was presented at the SIGCOMM conference, [PIFO @SIGCOMM](https://cs.nyu.edu/~anirudh/pifo-sigcomm.pdf).

One alternative has been recently presented at SIGCOMM, [PIEO](http://www.cs.cornell.edu/~vishal/papers/pieo_2019.pdf).

Both works are open-source (code available on Github). While PIFO is designed to be implemented on an ASIC, PIEO targets FPGAs.

### In-Network Computing

Programmable switches can be used as a computing platform for distribued applications. 

[A review of previous in-network computing works by the IETF COIN (Computing In the Network) group](https://tools.ietf.org/pdf/draft-he-coin-datacenter-00.pdf)

Some applications offloaded on programmable switches were shown to be accelerated by up to two order of magnitude in terms of throughput, latency and power-efficiency.

However, multiple researcher raised concerns about offloading distributed applications on programmable switchs. Most notably, the following questions were raised.
1)[How programmable switches should be used (vs can be used)](https://people.eecs.berkeley.edu/~apanda/assets/papers/LoadBalancing.pdf)
2)[Which applications can benefits from in-network computing?](https://drkp.net/papers/innetwork-hotos19.pdf)

---

# High-Level Synthesis

See LegUP, Xilinx Vivado HLS.

ahaHLS: An open source high level synthesis (HLS) tool using LLVM. [Link](https://github.com/dillonhuff/ahaHLS)
The authors also presents the main ideas used in his tools in videos [link to Youtube](https://www.youtube.com/channel/UC8qv9c4Ruu0mycMVjI7R48w/videos).

---

# High Speed I/O Framework for Software Packet Processing

A tutorial [on User Space Network Drivers](https://www.net.in.tum.de/fileadmin/bibtex/publications/papers/ixy-writing-user-space-network-drivers.pdf)

[DPDK](https://www.dpdk.org)

[Netmap: A Novel Framework for Fast Packet I/O](https://www.usenix.org/node/168897)

---

# Network Traffic Traces 

Traffic traces can be obtained via [CAIDA](https://www.caida.org)

Prefixes (IPv6 and IPv4) used in core networks can be extracted from BGP dumps available either on CAIDA, [routeviews](http://www.routeviews.org/routeviews/) or on [RIS](https://www.ripe.net/analyse/internet-measurements/routing-information-service-ris/ris-raw-data). Multiple tools/script are available to read the BGP dumps and extracts any information hold in a BGP message.

---


# Conferences / Journal

Do you want to publish to a conference not listed below? Double check the conference statistics on google scholar (under the metrics tab).

## Networking

[USENIX NSDI](https://www.usenix.org/conference/nsdi19)

[SIGCOMM](http://www.sigcomm.org)

[GLOBECOM](https://globecom2019.ieee-globecom.org/)

[INFCOMM](https://infocom2020.ieee-infocom.org/)

[CoNext](https://conferences2.sigcomm.org/co-next/2019/#!/home)

[HotNets](https://www.sigcomm.org/events/hotnets-workshop)

[Transaction on Networking](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=90)

[Usenix ATC](https://www.usenix.org/conferences/byname/131)

[Transactions on Communications](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=26)

[P4 Workshops](https://p4.org/events/2019-09-23-euro-p4-workshop/)
See the P4.org event section for the lastest P4 workshop.

[ANCS](http://www.ancsconf.org/)

[Computer Communication Review](https://www.sigcomm.org/publications/computer-communication-review)

## Computer Architecture 

### FPGA

[FPGA](http://isfpga.org/)

[FCCM](https://www.fccm.org/)

[FPL](http://www.fpl.org/h/)

### All remainings topics

[Transactions on VLSI](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=92)

[ACM Transactions on Computer Systems (TOCS)](https://dl.acm.org/citation.cfm?id=3341160)

[IEEE Transactions on Computers](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=12)

[Design Automation Conference (DAC)](https://www.dac.com/)

[IEEE Transactions on Computer-Aided Design of Integrated Circuits and Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=43)

[Micro](https://www.microarch.org/micro52/submit/papers.html)

[ASPLOS](https://asplos-conference.org/)

---

# Graduate Students Ressources

## Reflexion on Research



[You and your research](https://www.site.uottawa.ca/~yymao/misc/Hamming_kaiser.html)

## Bibliography manager
Endnote 


Zotero, a free an open-source blibliography manager. [Link](https://www.zotero.org) 


Emacs

## Reading a paper
[Reading a Paper](https://blizzard.cs.uwaterloo.ca/keshav/home/Papers/data/07/paper-reading.pdf)

We strongly advise you to take notes when you read a paper. The benefits are multiples: for your literature review, to fully understand an article, and to share with your colleagues!

## Writting a Paper 

[General advices from a Microsoft researcher on writting a paper](https://www.microsoft.com/en-us/research/academic-program/write-great-research-paper/). 

Books: [The Chicago Manual of Style](https://www.chicagomanualofstyle.org/home.html) is a good reference to write a thesis, or a journal paper. However, more specifically for journal papers [Writing Your Journal Article in Twelve Weeks, Second Edition](https://press.uchicago.edu/ucp/books/book/chicago/W/bo26985005.html) is a very good reference on this topic.

[Notes on the table presentation](https://inf.ethz.ch/personal/markusp/teaching/guides/guide-tables.pdf)

We strongly encourage to write a scientific article using LateX. If you are note familiar with LateX we recommand to use the TexStudio LateX editor (available on many platforms). 

## Presenting a Paper
[Presenting a Paper](https://www.microsoft.com/en-us/research/academic-program/give-great-research-talk/)

[Presentation guidelines](https://users.ece.cmu.edu/~pueschel/teaching/guides/guide-presentations.pdf)

## Presenting your research on your website

Use one of the tow following framework [Solo](http://chibicode.github.io/solo/) or [Duo](https://chibicode.github.io/duo/). Many other frameworks are available on Github (for your team, for blogging, etc.).

## Religion - Emacs
Emacs is an editor that is highly recommanded to use as everything can be integrated within emacs (from note taking, latex writting, developpement, etc.). The learning curve is *STEEP* (though), but it is worth it!

[Ovrview](https://www.gnu.org/software/emacs/tour/index.html)
[Tutorials](http://www.jesshamrick.com/2012/09/10/absolute-beginners-guide-to-emacs/)


In particular:
- to write LaTeX
  See the following [overview and tutorial for latex](https://nasseralkmim.github.io/notes/2016/08/21/my-latex-environment/#orgaa3b19e), and a [shorter but complementary tutorial](https://piotr.is/2010/emacs-as-the-ultimate-latex-editor/). hen you install pdf-tools, follow [this instructions](http://google-ebook.com/blog/2016/01/13/pdf-tools-in-emacs/)
- Bibliography management wih ivy-bibtex combined to Zotero [Follow this tutorial](https://nasseralkmim.github.io/notes/2017/02/23/how-i-manage-academic-sources-in-emacs-ivy-bibtex+zotero/)

- Take notes, organize them, GTD (Getting Things done)
  Packages to install: org-mode, org-notes, org-ref
  Org-mode is just ONE good reason to use emacs. See the [following tutorials](https://orgmode.org/worg/org-tutorials/)
- as an IDE (Python, C++, Lisp, VHDL, System Verilog, etc.)
- C++ IDE: Follow this [tutorial](http://syamajala.github.io/c-ide.html), which helps you to configure and install [cmake-ide](https://github.com/atilaneves/cmake-ide)
- Python IDE: Install and configure the [Elpy](https://github.com/jorgenschaefer/elpy) package
- Git Integration. [Magit](https://magit.vc) is just mindblowing! See [this youtube tutorial/demo](https://www.youtube.com/watch?v=vQO7F2Q9DwA)

