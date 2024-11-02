began: 8th October 2024

# SCC.131 Digital Systems

This module of the course is split into 4 components:

- Computer Architecture
  - Taught by Prof. Qiang Ni
  - Includes: Number Systems, Circuit and Logic, and Computer Architecture Theory/ISA
- Microbit
  - Taught by Dr. Ioannis Chatzigerogiou
  - Includes: Debugging Intro, Physical Computing, and Compilation
- ARM Assembly
  - Taught by Dr. Charalampos Rotsos
  - Includes: Assembly Programming, Memory, and Interrupts/IO
- Systems Programming
  - Taught by Dr. Paul Dempster
  - Includes: Assembly & C, Advanced C, and Network Sockets

The module aims for me to understand Digital Systems. This includes...

- ...fundamental concepts of hardware & Entire Computer Systems
- ...how hardware and software interact
- ...how to program and debug software at low levels

Assessed with Exams and Coursework:

| Task                                 | Type   | Week       | Worth |
| ------------------------------------ | ------ | ---------- | ----- |
| Architecture Quiz                    | Online | Week 5     | 5%    |
| Architecture + Embedded Systems Quiz | Online | Week 10    | 5%    |
| Assembly + Debugging Quiz            | Online | Week 15    | 5%    |
| Assembly                             | Online | Week 20    | 5%    |
| Programming Project                  | Online | Week 23    | 10%   |
| Exam                                 | Online | Week 28-30 | 70%   |

---

### Table of Contents

| Week | Lecture                                                                               | Original Slides                                                                  | Noted  |
| ---- | ------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | ------ |
| 1    | [Lecture 1 - Module Introduction](#lecture-1---module-introduction)                   | [Module Introduction](/SCC.131.slides/a.introSlides.pdf)                         | Yes    |
| 1    | [Lecture 2 - Architecture & Speed](#lecture-2---architecture--speed)                  | [Comp Architecture](/SCC.131.slides/b.compArchitectureIntro.pdf)                 | Yes    |
| 2    | [Lecture 3 - Information Coding](#lecture-3---information-coding)                     | [Information Coding](/SCC.131.slides/c.infoCodingPartOne.pdf)                    | Partly |
| 2    | [Lecture 4 - Information Coding Part 2](#lecture-4---information-coding-part-2)       | [Information Coding Contd](/SCC.131.slides/d.infoCodingPartTwo.pdf)              | No     |
| 3    | [Lecture 5 & 6 - Boolean Logic](#lecture-5--6---boolean-logic)                        | [Boolean Logic](/SCC.131.slides/e.booleanLogic.pdf)                              | No     |
| 4    | [Lecture 7 - Instruction Set Architecture](#lecture-7---instruction-set-architecture) | [Instruction Set Architecture](/SCC.131.slides/f.instructionSetArchitecture.pdf) | No     |
| 4    | [Lecture 8 - Building the ALU](#lecture-8---building-the-alu)                         | [Building The ALU](/SCC.131.slides/g.buildingTheALU.pdf)                         | NO     |

---

## Lecture 1 - Module Introduction & Computer Architecture

Architecture is the science of putting together building materials to produce buildings.

Computer Architecture is the science of putting together hardware to produce computers.

## Lecture 2 - Architecture & Speed

A computer is an electronic device for storing and processing data, in binary form, according to instructions given to it in a variable program.

### Computer History

- Analytical Engine
  - First computer
  - Partly built by Englishman Charles Babbage in the 19th century
  - A fully program-controlled mechanical computer
  - Consisted of the mill (calculating unit), the store, the reader, and the printer
  - Data was entered onto physical punched cards
  - Ada Lovelace wrote the first algorithm for a computer based on this machine.
- ENIAC
  - Electronic Numerical Integrator And Computer was the first programmable, electronic, general-purpose digital computer
  - Built during WW2 in the USA
  - Programmed via switches and cables
- Manchester SSEM
  - Small-Scale Experimental Machine was the first electronic stored-program computer
  - Built in Uni of Manchester
- Cambridge EDSAC
  - Electronic Delay Storage Automatic Calculator
  - Built at Cambridge Uni
  - First practical stored-program computer in regular use
  - Used punched cards to load programs
- IBM Personal Computer
  - Released 1981
  - Led to the era of cheap commodity-based computation

Computer Architecture is rules and methods that describe the functionality, organisation, and implementation of computer systems which can be applied at many levels such as processor, memory, and instruction sets.

### Von Neumman

- Memory that stores, data & instructions together
- A Control Unit (CU) that contains an instruction register and Program Counter (PC)
- Processing unit that contains Arithmetic Logic Unit (ALU) and processor Registers
- Input & Output mechanisms

![Von Neumman Architecture](images/VonNeummanDiagram.png "Diagram of Von Neumman")

CPU contains

- ALU + CU and Cache Memory
- Logically the same as the above diagram

![Von Neumman Architecture](images/VonNeummanDiagram2.png "Diagram of Von Neumman")

### Harvard

Instructions and data are stored in separate memories to overcome the bottleneck of Von Neumman. This allows parallel access to data and instruction so this can be faster.

![Harvard Architecture](images/harvradDiagram.png "Diagram of Harvard")

Modified Harvard:

- Separates instructions and data caches internally but a single main memory is visible to programs.

![Harvard Architecture](images/harvradDiagram2.png "Diagram of Harvard")

### Modern Architecture

![Modern Architecture Diagram](images/modernArchitecture.png "Diagram of Harvard")

### Speed Factors & Limitations

Computer speed metrics:

- Clock Rate
  - 3GHz processor makes 3 billion ticks per second
  - instructions take different numbers of ticks so bad
- Millions of Instructions Per Second (MIPS)
  - Better than previous but depends on which instructions are counted (number of instructions)
  - Different Results for programs
- Floating Point Operations Per Second (FLOPS)
  - Better indication of speed where it counts

Density Limitations

- number of transistors per square inch
- Moore's Law

## Lecture 3 - Information Coding

Computer hardware should be as simple as possible due to cost, performance, and scalability factors. Because of this, we focus on handling small, posotive integers. Any other data type is a code/represenation that maps to positive integers.

### ASCII

The American Standard Code for Information Interchange is a 7-bit binary (2<sup>7</sup>) code for characters.

![ASCII Table](images/ASCIItable.png "ASCII Table")

In practice we use numbers such as negatives, fractions, floating-point, etc. But all these map to small, posotive whole numbers held in memory.

### Decimal in Base-10

Representing 1984:

| Thousands (10<sup>3</sup>) | Hundreds ((10<sup>2</sup>)) | Tens ((10<sup>1</sup>)) | Units/Ones (10<sup>0</sup>) |
| :------------------------: | :-------------------------: | :---------------------: | :-------------------------: |
|    1 \* 10<sup>3</sup>     |     9 \* 10<sup>2</sup>     |   8 \* 10<sup>1</sup>   |     4 \* 10<sup>0</sup>     |
|         1 \* 1000          |          9 \* 100           |         8 \* 10         |           4 \* 1            |
|            1000            |             900             |           80            |              4              |

1000 + 900 + 80 + 4 = 1984.

### Multiplication and Division

1984 \* 10 = 19840

Multiplying a number by 10<sup>n</sup> shifts the number left by n decimal places, feeding in 0's on the right.

Dividing a number by 10<sup>n</sup> shifts the number right by n decimal places.

### Negative Numbers

There are 3 coding approaches for negative numbers:

- Sign and Magnitude
- Excess N
- Twos Complement

## Lecture 4 - Information Coding Part 2

## Lecture 5 & 6 - Boolean Logic

## Lecture 7 - Instruction Set Architecture

## Lecture 8 - Building The ALU
