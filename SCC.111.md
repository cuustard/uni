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

| Week | Lecture                                                                                      | Original Slides                                                                        | Noted |
| :--: | -------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- | :---: |
|  1   | [Lecture 1 - Module Introduction](#lecture-1---module-introduction)                          | [Module Intro](/SCC.111.slides/a.introSlides.pdf)                                      |  ✅   |
|  1   | [Lecture 2 - Writing Code](#lecture-2---writing-code)                                        | [Intro to C](/SCC.111.slides/b.introToC.pdf)                                           |  ✅   |
|  2   | [Lecture 3 - Control Flow](#lecture-3---control-flow)                                        | [Control Flow](/SCC.111.slides/c.controlFlow.pdf)                                      |  ✅   |
|  2   | [Lecture 4 - Functions & Flow](#lecture-4---functions--flow)                                 | [Functions & Flow](/SCC.111.slides/d.functionsAndFlow.pdf)                             |  ✅   |
|  3   | [Lecture 5 - Variables & Arrays](#lecture-5---variables--arrays)                             | [Variables & Arrays](/SCC.111.slides/e.variablesAndArrays.pdf)                         |  ❌   |
|  3   | [Lecture 6 - Reading Code](#lecture-6---reading-code)                                        | [Reading Code](/SCC.111.slides/f.readingCode.pdf)                                      |  ❌   |
|  4   | [Lecture 7 - Testing](#lecture-7---testing)                                                  | [Testing](/SCC.111.slides/g.testing.pdf)                                               |  ❌   |
|  4   | [Lecture 8 - Debugging](#lecture-8---debugging)                                              | [Debugging](/SCC.111.slides/h.debugging.pdf)                                           |  ❌   |
|  5   | [Lecture 9 - Deubbign Part 2](#lecture-9---debugging-part-2)                                 | [Debugging Part 2](/SCC.111.slides/i.debuggingPartTwo.pdf)                             |  ❌   |
|  5   | [Lecture 10 - Indirection & Pointers](#lecture-10---indirection--pointers)                   | [Indirection & Pointers](/SCC.111.slides/j.indirectionPointers.pdf)                    |  ❌   |
|  6   | [Lecture 11 - Pointers & Strings](#lecture-11---pointers--strings)                           | [Pointers & Strings](/SCC.111.slides/k.pointersAndStrings.pdf)                         |  ✅   |
|  6   | [Lecture 12 - Dynamic Memory & Compound Types](#lecture-12---dynamic-memory--compound-types) | [Dynamic Memory & Compound Types](/SCC.111.slides/l.dynamicMemoryAndCompoundTypes.pdf) |  ✅   |
|  7   | [Lecture 13 - Quiz Solutions](#lecture-13---quiz-solutions)                                  | [Quiz Solutions](/SCC.111.slides/m.quizResults.pdf)                                    |  ❌   |
|  7   | [Lecture 14 - APIs & Files](#lecture-14---apis--files)                                       | [APIs & Files](/SCC.111.slides/n.APIsAndFiles.pdf)                                     |  ✅   |

---

---

## Lecture 1 - Module Introduction

A program is a detailed plan or procedure for solving a problem with a computer.

Imperative programming is a programming paradigm of software that uses statements that change a program's state. So I should think about what to represent, and how my program should manipulate that.

C is a compact and low-level language used to generate fast and efficient code that exploits hardware features well. It is compiled (translated into assembly only the computer understands).

---

---

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

---

---

## Lecture 3 - Control Flow

When writing code we need to see how it is executed to make sense of what it will do. So we need to understand keywords, operators and function calls.

Code can move between programs, blocks of code, statements in the program, and within a line of code as expressions within the statement are evaluated.

Flow can be controlled by conditional statements (statements that must be true for a block of code to execute).

A program executes from start to finish with statements that can be repeated. Choosing the path for a program to flow through can also be decided with if statements.

'Do... while' loops test a condition after the block of code is executed.

---

---

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

---

---

## Lecture 5 - Variables & Arrays

---

---

## Lecture 6 - Reading Code

---

---

## Lecture 7 - Testing

---

---

## Lecture 8 - Debugging

---

---

## Lecture 9 - Debugging Part 2

---

---

## Lecture 10 - Indirection & Pointers

---

---

## Lecture 11 - Pointers & Strings

---

---

## Lecture 12 - Dynamic Memory & Compound Types

A string is a sequence of characters (an array).

```C
int main() {
    char *password = "Password";
    *userEntry = "guess";

    if(userEntry == password) { // this is wrong as it is comparing the values stored in the pointer variables. this returns false because there are different memory addresses stored in password and userEntry
        printf("Correct Login\n");
    }
}
```

#### Comparing Strings

```C
char *password = "pass123";

if (strcomp(password, "paass123") == 0 || strcomp(password, "secret") == 0) {
    printf("Yes\n")
}
```

#### `<string.h>`

```C
int strlen(char *) // find the length of string s
char *strchr(char *, int) // find a character within a string (pointer or NULL)
strcat(char *d, char *s) // append string s to d
strcpy(char *d, char *s) // copy string s to d
```

### Beyond Basic Variables

We have only seen variables that represent simple scalar values like int, char, etc or as fex length arrays of values. These are all declared with a fixed size.

Variables also go out of scope at the end of the block they are declared in. They also incur overhead when copied.

#### Addressing Fixed Size

Types of storage:

- **Literals**
- **Standard Variables**
- **Global Variables**
- **Dynamic Variables** - from the heap

Dynamic Memory is allocated at runtime by my code. It needs managing (must free and return to the heap when done with it). Gotta take extreme care to avoid memory leaks, and crashes.

`maccloc()` gets a pointer to some memory.

```C
//create pointer str to 100 bytes
char *str = (char *) malloc(sizeof(char) * 100);

// do something with it
str[0] = 'h';
strcpy(str, "hello");

// return str to the heap
free(str)

//malloc will return NULL if it fails (we ask for too much)

// `sizeof(char)` asks how much a char is (1 byte)
// `* 100` multiplies 1 byte by 100
// `malloc(100)` allocates the heap space (returns a pointer)
// `char *str` declares pointer str
// `= (char *)` casts thet pointer to be of the type "points to char"
```

### More than just scalar values

Compound types combine simple types into 1 entity. For example, a Q&A are always a pair we keep together.

#### `struct`

```C
// Declare a new type (not variable, struct person)

struct person {
  char name[20]; // array of chars (string name)
  int age;
  char gender; // gender will be a single letter, e.g. 'f' or 'm'
};
// Declare the variable of type struct person */
struct person aPerson;

```

Assigning:

```C
struct person aPerson;

strcpy(aPerson.name, "Nigel");
aPerson.age = 30;
aPerson.gender = 'm';
```

An array of structs:

```C
struct person *people; // A pointer to a 'type struct person'

// Try allocate memory (an array of struct persons)

if ((people = (struct person *)
    malloc(sizeof(struct person) * 100)) != NULL) {
//it worked, do something with 100 people
// free when done

people[50].age = 18;

free(people)

} else {
    // oh no out of memory
}
```

access a struct field from a pointer:

```C
struct person *p = &aPerson;
strcpy(p->name, "Nigel");
p->age = 30;
p->gender = 'm’;
printf("%s's age is %d\n", p->name, p->age);
```

## Lecture 13 - Quiz Solutions

---

---

## Lecture 14 - APIs & Files

### APIs

We need a way of running a program to interact with its environment, get data from long-terms presistent storage, and to handle any errors (missing giles, permissions, read/write data).

To do this we can use an API (Application Programming Interface) is just a software interface. In our case, it's a set of operations defined for interacting with the systme in a controlled way.

In C, An API we access is simply:

- **One or more function** we can call
- **Declared in a header** (.h) file that we need to include to use them

### Files

Informally, a file is a collection of (usually related) data, which can be logically viewed as a stream of bytes. This is the smallest unit of storage in the UNIX file system.

A file:

- Provides persistent storage of data
- Either text or binary format
- Can be accessed serially (line by line), OR randomly (jumping to specific data we want).
- Needs to be opened, read/written to, and closed.

Serially accessing:

1. Open file
2. Read next line
3. Step 2. until all lines read
4. Close File

### Character Streams

Processese input and output at a characater stream level...

```C
int getchar(void) // returns the next input character each time it is called, or when it encounters EOF (End Of File). EOF is defined in <stdio.h>

int putchar(int) // is used for output. it puts the character c on the standard output (the screen). returns the character written, or EOF if an error occurs.
```

### File System Rules

File must be opened by the library function `fopen`. This function takes a file name and returns a pointer (_FILE_ \*) to be used in the reads or writes. This file pointer points to a structure that contains information about the file (e.g. where to read from).

```C
// Declare pointer to a FILE structure
FILE *fp;

// The API call to open a file
FILE *fopen(char *name, char *mode);


// Read and write Characters
int getc(FILE *fp);
int putc(int c, FILE *fp);

// Close file
fclose(FILE *fp);


// working with lines of text (text files)
char *fgets(char *line, int maxline, FILE *fp);



// Reading and writing records (binary files)

size_t fread(void *ptr, size_t size, size-t nobj, FILE *fp);

// fread reads from stream into arry ptr at most nobj objects of size size
// fread returns the number of objects read
// feof and ferror must be used to determine status

//alt:
size_t fwrite(const void *ptr, size_t size, size_t nobj, FILE *fp);
```
