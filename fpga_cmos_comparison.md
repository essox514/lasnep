# Title : Comparing FPGA vs. custom CMOS and the Impact on Processor Microarchitecture
# Conference : FPGA 2011

# Title Quantifying the Gap Between FPGA and Custom CMOS to Aid Microarchitectural Design
# Journal : Transcation on VLSI 2014
extension of Comparing FPGA vs. Custom CMOS and the Impact on Processor Microarchitecture

# Authors :
Henry Wing, Vaughn Betz, Jonathan Rose

# Summary
This paper compare processor microarchitecture implementation on FPGA and custom CMOS circuits.
Two question are raises in the paper :
- What processor's building blocks suits well on the FPGA substrate.
- How processor microarchitecture should be implemented on FPGAs.
To answer those question, independant implementation of different building blocks are compared between CMOS and FPGAs.
FPGAs implementation have 18x-26x more delays and 17x-27x increase in area usage.
However, while delays for most building blocks is stable in regards to complete processors implementation into the FPGA, the area of those different building blocks vary a lot.
For example SRAM implemenation is really efficient in area since there is hard SRAM block inside the FPGA while Content Adressable Memory are really expansive in term of area.


# Opinion
This paper is really insterested.
Results were predictable but it is important to have written them down.
Considering the regain of interest for FPGA today, it would be interesting to do the same work for other types of architecture.
The paper do not address the question of reconfigurability which would have be interested, Processor implementation on FPGAs can be addapted to specific usage and some instruction can be removed considering the required ones.

# Details
We will discuss in more details of the paper here.

## Building blocks analysis

## Microarchitecture considerations
