began: 9th October 2024

# SCC.111 Software Development

This module of the course is taught by 4 Lecturers:

- Hansi Hettiarachchi
- Adrian Friday
- Saad Ezini
- Nigel Davies

This module is assessed with Exams and Coursework:

| Task                             | Type   | Week       | Worth |
|----------------------------------|--------|------------|-------|
| Exam                             |  | Summer Term | 70%   |
| A coursework | Online | Week 5     | 5%    |
| A coursework | Online | Week 10    | 5%    |
| A coursework | Online | Week 15    | 5%    |
| A coursework | Online | Week 20    | 5%    |
| Programming Project              | Online | Week 21-25    | 10%   |

The module aims for me to understand Sofware Development. This includes...

- ...instilling the knowledge, understanding, and skills expected of a principled computer programmer.
- ...developing a coherent understanding of the principles & practice of imperative programming, the software development lifecycle, and its associated tools and techniques

---

### Table of Contents

| ToC                                      | Original Slides                       | Date |
|------------------------------------------|---------------------------------------|------|
| [Lecture 1 - Module Introduction](#lecture-1---module-introduction) | [Module Intro](/SCC.111.slides/a.introSlides.pdf) | 9/10/2024 |
| [Lecture 2 - Writing Code](#lecture-2---writing-code) | [Intro to C](/SCC.111.slides/b.introToC.pdf) |  |
| [Lecture 3 - Control Flow](#lecture-2---control-flow) | [Control Flow](/SCC.111.slides/c.controlFlow.pdf) | |

---

## Lecture 1 - Module Introduction

noted: 9th October 2024

[Lecture Slides](/SCC.111.slides/a.introSlides.pdf)

A program is a detailed plan or procedure for solving a problem with a computer.

Imperative programming is a programming paradigm of software that uses statements that change a programs state. So I should think about what to represent, and how my program should manipulate that.

Starting with C - a compact and low level language used to generate fast and efficient code that exploits hardware features well. It is complied (translated into assembly only the computer understands).

Example of a C program:

```C
#include <stdio.h>

int main()

{
    printf("Hello world\n")
}
```

## Lecture 2 - Writing Code

[Lecture Slides](/SCC.111.slides/b.introToC.pdf)

```C
#include <studio.h>

int main()
{
    printf("Hello world\n")
}
```

Line 1 copies the contents of the file 'stdio.h' into the file this program is written in. Line 3 declares 'main' a function that is the starting point for execution when the program is run. The '{ }' makes up the body of the main function. Line 5 calls a function printf, which we pass in "Hello world" into, to output the message.

I solve all problems by repeatedly breaking it down into smaller more managable steps.

C Vocab:

- auto
- break
- case
- char
- const
- continue
- defualt
- do
- double
- else
- enum
- extern
- float
- for
- goto
- if
- int
- long
- register
- return
- short
- signed
- sizeof
- static
- struct
- switch
- typedef
- union
- unisgned
- void
- volatile
- while

Programming languages have syntax - rules on how keywords/reserved words are used (the how). Vairables hold data (the what). Operators manipulate the data to produce the desired output.

```C
#include <stdio.h>

int main()
{
    //Declaring counter a variable and setting it to 0
    int counter = 0;

    while (counter < 10) {
        // while counter is less than 10, add 1
        counter++;
    }

    printf("The variable counter is now %d\n", counter)
}
```

Program Flow: 'counter' controls the flow round a loop linked to the keyword 'while'. This is a logical test < or less than which is either true or false.

### Variables Types

```C
int main()
{
    int i;
    char c;
    float f;
    double d;
    short s;
    unsigned char b;
    unsigned int u;
}

```

### Operators

Binary Operators:

- `+` add
- `-` subtract
- `/` divide
- `*` multiply
- `%` remainder (mod)
- `<<` left shift
- `>>` right shift

Logical Operators:

- `<` less than
- `>` greater than
- `<=`, `>=`
- `==`, `!=`
- `!` boolean NOT
- `&&` boolean AND
- `||` boolean OR

```C
int main()
{
    int a, b;

    a = -1;
    a = a + 3;
    b = (a * 5) + 2;
    b = b / 2 + 2;

    printf("b is %d\n", b)

    return 0
}
```

## Lecture 3 - Control Flow

[Lecture Slides](/SCC.111.slides/c.controlFlow.pdf)

