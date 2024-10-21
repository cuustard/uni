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

| Task                            | Type   | Week       | Worth |
| ------------------------------- | ------ | ---------- | ----- |
| Architecture Quiz               | Online | Week 5     | 5%    |
| Architecture + Embedded Systems | Online | Week 10    | 5%    |
| Assembly + Debugging Quiz       | Online | Week 15    | 5%    |
| Assembly                        | Online | Week 20    | 5%    |
| Programming Project             | Online | Week 23    | 10%   |
| Exam                            | Online | Week 28-30 | 70%   |

---

### Table of Contents

| Week | Lecture                                                                         | Original Slides                                                     | Date Noted |
| ---- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ---------- |
| 1    | [Lecture 1 - Module Introduction](#lecture-1---module-introduction)             | [Module Introduction](/SCC.131.slides/a.introSlides.pdf)            | 8/10/2024  |
| 1    | [Lecture 2 - Architecture & Speed](#lecture-2---architecture--speed)            | [Comp Architecture](/SCC.131.slides/b.compArchitectureIntro.pdf)    | 11/10/2024 |
| 2    | [Lecture 3 - Information Coding](#lecture-3---information-coding)               | [Information Coding](/SCC.131.slides/c.infoCodingPartOne.pdf)       |            |
| 2    | [Lecture 4 - Information Coding Part 2](#lecture-4---information-coding-part-2) | [Information Coding Contd](/SCC.131.slides/d.infoCodingPartTwo.pdf) |            |

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

## Lecture 4 - Information Coding Part 2
