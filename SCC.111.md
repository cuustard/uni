began: 9th October 2024

# SCC.111 Software Development

This module of the course is taught by 4 Lecturers:

- Hansi Hettiarachchi
- Adrian Friday
- Saad Ezini
- Nigel Davies

The module aims to help me understand software development. This includes...

- ...instilling the knowledge, understanding, and skills expected of a principled computer programmer.
- ...developing a coherent understanding of the principles & practice of imperative programming, the software development lifecycle, and its associated tools and techniques

Assessed with Exam and Coursework:

| Task                       | Week               | Worth         |
| -------------------------- | ------------------ | ------------- |
| "Coursework" (In-lab quiz) | Week 5, 10, 15, 20 | 20% (5% each) |
| Programming Project        | Week 21-25         | 10%           |
| Exam                       | Summer Term        | 70%           |

---

### Table of Contents

| Week | Lecture                                                             | Original Slides                                                | Noted |
| ---- | ------------------------------------------------------------------- | -------------------------------------------------------------- | ----- |
| 1    | [Lecture 1 - Module Introduction](#lecture-1---module-introduction) | [Module Intro](/SCC.111.slides/a.introSlides.pdf)              | Yes   |
| 1    | [Lecture 2 - Writing Code](#lecture-2---writing-code)               | [Intro to C](/SCC.111.slides/b.introToC.pdf)                   | Yes   |
| 2    | [Lecture 3 - Control Flow](#lecture-3---control-flow)               | [Control Flow](/SCC.111.slides/c.controlFlow.pdf)              | Yes   |
| 2    | [Lecture 4 - Functions & Flow](#lecture-4---functions--flow)        | [Functions & Flow](/SCC.111.slides/d.functionsAndFlow.pdf)     | Yes   |
| 3    | [Lecture 5 - Variables & Arrays](#lecture-5---variables--arrays)    | [Variables & Arrays](/SCC.111.slides/e.variablesAndArrays.pdf) | No    |
| 3    | [Lecture 6 - Reading Code](#lecture-6---reading-code)               | [Reading Code](/SCC.111.slides/f.readingCode.pdf)              | No    |
| 4    | [Lecture 7 - Testing](#lecture-7---testing)                         | [Testing](/SCC.111.slides/g.testing.pdf)                       | No    |
| 4    | [Lecture 8 - Debugging](#lecture-8---debugging)                     | [Debugging](/SCC.111.slides/h.debugging.pdf)                   | No    |

---

## Lecture 1 - Module Introduction

A program is a detailed plan or procedure for solving a problem with a computer.

Imperative programming is a programming paradigm of software that uses statements that change a program's state. So I should think about what to represent, and how my program should manipulate that.

C is a compact and low-level language used to generate fast and efficient code that exploits hardware features well. It is compiled (translated into assembly only the computer understands).

## Lecture 2 - Writing Code

```C
#include <studio.h>

int main()
{
    printf("Hello world\n")
}
```

Line 1 copies the contents of the file 'stdio.h' into the file this program is written in. Line 3 declares 'main' a function that is the starting point for execution when the program is run. The '{ }' makes up the body of the main function. Line 5 calls a function printf, which we pass in "Hello world", to output the message.

I solve all problems by repeatedly breaking them down into smaller more manageable steps.

C Vocab:

|          |         |        |          |        |
| -------- | ------- | ------ | -------- | ------ |
| auto     | break   | case   | char     | const  |
| continue | default | do     | double   | else   |
| enum     | extern  | float  | for      | goto   |
| if       | int     | long   | register | return |
| short    | signed  | sizeof | static   | struct |
| switch   | typedef | union  | unsigned | void   |
| volatile | while   |        |          |        |

Programming languages have syntax - rules on how keywords/reserved words are used (the how). Variables hold data (the what). Operators manipulate the data to produce the desired output.

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

Program Flow: 'counter' controls the flow around a loop linked to the keyword 'while'. This is a logical test < or less than which is either true or false.

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
- `<=` less than or equal to, `>=` greater than or equal to
- `==` equivalen to, `!=` not equivilent to
- `!` NOT
- `&&` AND
- `||` OR

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

When writing code we need to see how it is executed to make sense of what it will do. So we need to understand keywords, operators and function calls.

Code can move between programs, blocks of code, statements in the program, and within a line of code as expressions within the statement are evaluated.

Flow can be controlled by conditional statements (statements that must be true for a block of code to execute).

A program executes from start to finish with statements that can be repeated. Choosing the path for a program to flow through can also be decided with if statements.

'Do... while' loops test a condition after the block of code is executed.

## Lecture 4 - Functions & Flow

We solve all problems by decomposing them into smaller components. Sometimes the solution to these components can be packaged up into a functional and callable unit. This means we have to write less code and and makes it easier to maintain and reuse.

C lets us define functions which package and name specific functionality. C also has libraries. In C, functions follow this form:

```
direct-declarator (parameter-type-list)

int function_name()
{
    some code
}
```

They can only return an arithmetic type or nothing (void)

`main()` is the entry point to the program. It takes no parameters and returns a code to the shell.

In C, the parameter values in the function are only ever a copy of what passed in (passed by value).

## Lecture 5 - Variables & Arrays

## Lecture 6 - Reading Code

## Lecture 7 - Testing

## Lecture 8 - Debugging
