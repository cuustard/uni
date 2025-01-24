began: 9th October 2024

# SCC.111 Software Development

The module aims to help me understand software development. This includes instilling the knowledge, understanding, and skills expected of a principled computer programmer, and developing a coherent understanding of the principles & practice of imperative programming, the software development lifecycle, and its associated tools and techniques.

| Assessment          | When               | Worth         |
| ------------------- | ------------------ | ------------- |
| In-lab quiz         | Week 5, 10, 15, 20 | 20% (5% each) |
| Programming Project | Week 21-25         | 10%           |
| Exam                | Summer Term        | 70%           |

---

### Table of Contents

| Week | My Notes                                                                                     | Original Slides                                                                        | Noted |
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
|  5   | [Lecture 10 - Indirection & Pointers](#lecture-10---indirection--pointers)                   | [Indirection & Pointers](/SCC.111.slides/j.indirectionPointers.pdf)                    |  🟧   |
|  6   | [Lecture 11 - Pointers & Strings](#lecture-11---pointers--strings)                           | [Pointers & Strings](/SCC.111.slides/k.pointersAndStrings.pdf)                         |  ❌   |
|  6   | [Lecture 12 - Dynamic Memory & Compound Types](#lecture-12---dynamic-memory--compound-types) | [Dynamic Memory & Compound Types](/SCC.111.slides/l.dynamicMemoryAndCompoundTypes.pdf) |  ✅   |
|  7   | [Lecture 13 - Quiz Solutions](#lecture-13---quiz-solutions)                                  | [Quiz Solutions](/SCC.111.slides/m.quizResults.pdf)                                    |  n/a  |
|  7   | [Lecture 14 - APIs & Files](#lecture-14---apis--files)                                       | [APIs & Files](/SCC.111.slides/n.APIsAndFiles.pdf)                                     |  ✅   |
|  8   | [Lecture 15 - More Files](#lecture-15---more-files)                                          | [Files Continued](/SCC.111.slides/o.moreFileStuff.pdf)                                 |  ✅   |
|  8   | [Lecture 16 - Libraries](#lecture-16---multi-file-projects)                                  | [Libraries](/SCC.111.slides/p.libraries.pdf)                                           |  ✅   |
|  9   | [Lecture 17 - Version Control](#lecture-17---version-control)                                | [Version Control](/SCC.111.slides/q.versionControl.pdf)                                |  🟧   |
|  9   | [Lecture 18 - Dynamic Data Structures](#lecture-18---dynamic-data-structures)                | [Dynamic Data Structures](/SCC.111.slides/r.dynamicDataStructures.pdf)                 |  🟧   |
|  10  | [Lecture 19 - C Highlights](#lecture-19---c-highlights)                                      | [C Highlights](/SCC.111.slides/s.cHighlights.pdf)                                      |  ❌   |
|  10  | [Lecture 20 - Fun By The C](#lectuer-20---fun-by-the-c)                                      | [Fun By The C](/SCC.111.slides/t.funByTheC.pdf)                                        |  🟧   |
|  11  | [Lecture 21 - Intro to Term 2](#lecture-21---introduction-to-term-2)                         | [Intro To Term 2](/SCC.111.slides/u.introToTerm2.pdf)                                  |  ✅   |
|  11  | [Lecture 22 - Principles of OOP](#lecture-22---principles-of-oop)                            | [Principles of OOP](/SCC.111.slides/v.principlesOfOOP.pdf)                             |  ✅   |
|  12  | [Lecture 23 - Encapsulation](#lecture-23---encapsulation)                                    | [Encapsulation](/SCC.111.slides/w.encapsulation.pdf)                                   |  ❌   |
|  12  | [Lecture 24 - Debugging](#lecture-24---debugging)                                            | [Debugging](/SCC.111.slides/x.debugging.pdf)                                           |  ✅   |

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

## Lecture 9 - Debugging Part 2

## Lecture 10 - Indirection & Pointers

A pointer is a variable that contains the address of something else in memory such as another variable. This means that the pointer is not the value itself, it is the where to find it. It has its own type - pointer - in C.

Think of computer memory as a street of houses (memory section) each with a unique location identifier (an address).

When we declare a variable, a space in memory is set aside to store that type of data and the location is labelled with a name. E.G. declaring `x = 65` in our program will find free space in memory. In memory location `0x1012`. It labels that memory location as `x` and stores `65` there. We could get that data by the variable name or by targeting the address. This is good because if we have that box labelled x that contains 65, if I want to get that box I either need the address 0x1012 or i need the variable name. But if i want to get to the location 0x1024 I don't have a variable name for it, but I do have an address so I can get there without a name.

What pointers allow us to talk about the space where x is, not what it is. Pointers give us this level in indirection. Pointers are variables themselves that we can change and make them point to different places.

```C
int *p = &y;
// a pointer p is equal to the address of int y
// so if y = 32 is stored in 0x1004 then x = 0x1012
// the & is saying give me the address of y not the data at y.
// the * is declaring a pointer to an integer not the integer itself
```

Dereferencing:

```C
*x = 65;
// go to var x, find the value stored in it, treat it as an address, follow the address, and in the place that youve got to put the number 65.
// so the * is saying, treat the thing in x as an address. then the data at that memory address is set to the RHS in this case 65

// so if you didnt have the *, then the data at x would be replaced by 65. the compiler might complain as x is a type pointer but you trying to put int in it.
```

When we call a function we use a copy of the parameters the function is using. E.G.:

```C

void add_5(int value) {
    value = value + 5;
}

int main() {
    int amount = 10;
    add_5(amount);
    printf("Amount = %d\n", amount);
    // you would expect this to print 15. but the function is passed a copy of the data in var amount, not the actual thing. So the data in var amount is not changed. scope issue.
    return 0;
}
```

To combat this we need to pass in the address of the thing that needs to be changed.

```C
void add_5(int *value) {
    *value = *value + 5;
    // 'value' is now where the data is that we modify
}

int main() {
    int amount = 10;
    add_5(amount);
    printf("Amount = %d\n", amount);
    return 0;
}
```

## Lecture 11 - Pointers & Strings

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

## Lecture 15 - More Files

### Challenge 1 - Copying A File

1. Only copy a file that exists
2. Only write to a 'valid' file
3. Copy data from the input, to the output until we reach the end of the input file

### Challenge 2 - Finding A Pattern in a text file

1. Find a pattern
2. Read the file line-by-line
3. Search the line for the pattern
4. Count how many times we find the pattern

### Challenge 3 - Record Access (Binary Data)

1. Read and write binary data to a file
2. Use binary file IO
3. Assuming that the format of the data structure is the formatof the file

## Lecture 16 - Multi File Projects

Having all our code in a single file can be straightforward as the compiler only has one file to parse to find all the functions in the program. It also means that the programmer only has one place to look. It also means that

However, it is problematic. One file won't scale well. Eventually, scrolling becomes unmanageable, making teamwork and handling larger projects difficult. It also becomes harder to package functions for reuse in other projects. Additionally, there is a risk of hidden dependencies and side effects.

To combat this we can split a project into multiple smaller files. We can create useful sets of functions (cleaner APIs) that are grouped by purpose and can be reused across projects.

![image](images/splitIntoManyFilesEG.png "image")

We need to let main.c (or any function callers) know about the functions, and tell the compiler that there are multiple parts to compile and assemble.

We can tekk the compiler what to expect for a function by declaring a forward declaration:

```C
int dequeue(); // compiler learns about the function spec

int main() {
    // call dequeue from here
    dequeue(); // Compiler knows what to expect here
}

// implementation of dequeue here
int dequeue() {
    // the function
    // Compiler actually declares function here
}
```

Example of splitting across files:

```C
//FILE:  main.c
int dequeue();

int main() {
    dequeue();
}
```

```C
//FILE: queue.c
int dequeue() {
    // ...
}
```

Even better:

```C
//FILE: queue.h
int dequeue();
```

```C
//FILE:  main.c
#include "queue.h"

int main() {
    dequeue();
}
```

```C
//FILE: queue.c
int dequeue() {
    // ...
}
```

But now that we have multiple C files we need to combine them into a single executable: `gcc -o target source1.c source2.c etc.c`. Continued example:

```
gcc -o main main.c queue.c
```

## Lecture 17 - Version Control

Code is changed all the time. We start with nothing and write code line by line. We fix logical and syntax errors. The requirements evolve so we extend the code. We work with multiple developers and in many teams.

We need a more principled approach to tracking your code base. We need to know what was changed, when, and by whom. We need version control.

A version is essentially a new 'save'. Everytime someone makes a change tothe code (including adding/removing files and dependencies) to the project, the new 'version' is the sum of the differences between the source files. It's only a version when you chose to 'mark' the set of changes at some point in time.

So version control is essentially software that we explicitly choose to track of mark certain changes. Revisions are created by 'committing' the changes. We label each revision. The differences between the source files are stored. This forms a revision history over the timeline of the project.

This revision history allows us to see the cumulative differences, where the changes are, what the changes were, and we can 'go back in time' (reverting the changes to previous versions).

## Lecture 18 - Dynamic Data Structures

If the data we want to process is of unknown size then we'd need our application to work despite flexible sixed data. Or we would need a more powerful way of organising the data to make it quicker to search or sort. Simple arrays lend themselves to linear organised data ideally of known size. These are not good enough.

Fortunately we can use dynamic memory to allocate elements in data structures. We can also use pointers between dynamic instances to organise our data structure like a list of tree.

### Building a Dynamic 'singly linked list'

1. Allocate space for a 'node' of the appropriate type
2. Find where to add our item (start, end, insertion point)
3. Adjust the pointers to stay consistent with the type of data structure we're working with

A linked list has 3 operations:

- **Insert**: add to the list
- **Find**: returns a pointer to the item in the list
- **Delete**: remove from the list

To develop these we need a good understanding of pointers, compound types, and dynamic memory (malloc).

```
struct {
    char name[20]
    char college[10]
    struct pointer next
} element {

}
```

### Compound Variables & Dynamic Memory

1. Declare a type for our node (struct)
2. A variable representing the pointer to the data structure
3. For each node, allocate a new node (using malloc)
4. Chain it, so our first item points to the new item

### Algorithms

```C
typedef struct tagNode {
    char name[20], college[10];

    struct tagNode *next;
} tElement;

// insert function
tElement *insert(tElement *head, char *name, char *college) {
    //create new node
    tElement *new = (tElement *) malloc(sizeof(tElement));

    // initialise node
    strcpy(new->name, name);
    strcpy(new->college, college);
    new->next = NULL;

    // look through the list, find where to insert and inser

}

// print function
tElement *print(tElement *head) {
    for (tElement *item = head; item != NULL; item = item->next) {
        print("item %p contains %s\n", item, item-<name);
    }
}

```

## Lecture 19 - C Highlights

## Lectuer 20 - Fun By The C

`gcc -o main main.c` makes preprocesor, c compiler, linker.

The preprocessor defines constants, macros, and includes other files. lets you define a thing then it is substituted in the source file.

there is no true or false, only 1 or 0. can define TRUE and FALS in constant in preprocess,r

```C++
#define FALSE 0
#define TRUE !FALSE

// textually replaces "FALSE" with 0
```

## Lecture 21 - Introduction To Term 2

<audio controls>
  <source src="SCC.111.slides/u.introToTerm2.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

## Lecture 22 - Principles of OOP

<audio controls>
  <source src="SCC.111.slides/v.principlesOfOOP.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

To write scalable code, it must be modular. Modularity relies on standards. The interface between modules and the world must be well-defined. For example, almost every lego brick can plug into every other leg brick. Their interfaces have the same standard. In software, these standards are called an Application Programmable Interface (API).

![image](images/legoModularity.png)

Programming langiuages are classified on the core paradigm on which they are based.

C is a procedural language. This is because there is a well-defined start point, the code is broken down into manageable chuncks (functions), functions are called by one another, and programs hold information in the form of variables. These variables are passed as parameters to those functions, or can be global. So procedural languages are structured around the code.

Procedural programming languages give little thought to the location of the data. Code modularity occurs in functions and libraries. Data modularity only occurs in structures.

### Oobject Oriented Programming

OOP languages combine code and data. Objects are the lego bricks. They group similar data and functions (tight cohesion). They isolate parts of the program from the rest, reducing the complexity of the software.

Objects provide **encapsulation** in which datat and code cannot be separated. Data is defined through **attributes**. Behaviour/methods/functions are defined through **methods**. Objects protect their inner workings through an API. Interactions with objects occur throufh its methods. The programmer only exposes what they choose to. This provides tight control over how it is used. This allows programmers to provide sealed boexes of code in order to promote simplicity.

![image](images/object.png)

Objects are defined by **classes**. This is a specification (like a blueprint) of an object someone might build.

Class: Bank Accont
Object: Jake Evans
Attribute: Current Balance

Bank account blueprint. instantiate for Jake Evans. Current Balance Attribute of £10,000,000.

```c++
// Captialised Camel Case
// Class keyword defines that everything in the block is part of the class. Similar to a structure.

// an objects attributes are implemented through variables. These are declared inside a classs, but outside any method. These attributes provide a new level of scope which are more controlled than global variables but less specific than local.

class Car {
    int milesDriven = 0;
    char *colour;

public:
    void drive(int miles);
    void respray(char *c);
    void show();
};

// implementation of methods from class
void Car::drive(int milels) {
    milesDriven = milesDriven + miles;
}

void Car::respray(char *c) {
    colour = (char *)c;
}

void Car::show() {
    printf("I am a %s car, and I've driven %d miles.\n", colour, milesDriven);
}
```

We initialise a object from a class like this:

```c++
Car amysCar;

amysCar.respray((char *)"White");
amysCar.drive(16);
amysCar.show();
```

## Lecture 23 - Encapsulation

<audio controls>
  <source src="SCC.111.slides/w.encapsulation.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

## Lecture 24 - Debugging

<audio controls>
  <source src="SCC.111.slides/x.debugging.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
</audio>

> "Everyone knows that debugging is twice as hard as writing a program in the first place. So if you're as clever as you can be when you write, how will you ever debug it?" - Brian Kernighan, The Elements of Programming Style, 2nd edition, chapter 2

> "Generative AI tools will mean that typical code written by humans will be harder to write, and they will spend a larger proportion of their time analysing and debugging" - Joe Finney (2003)

> "You can't win until you're not afraid to lose" - John Francis Bongiovi

Finding bugs is a good thing. Compile often. Test frequently. Add one feature at a time. A compiler is your friend when it comes to syntax errors. Compiler messages tell you the file and line of code where the syntax error is found. Debugging is like finding a needle in a haystack... so don't add more hay until you know there is no needle.

Thoroughly read through the code you have written. Dry run it in your head before you execute the code. This is a cheap approach but relys on experience. If your code is modular, you can start at the beginning of the method where the program goes wrong.

If you fail to find a bug by inspection, then stop trying to fix it and instead try to find it using logging diagnostics. Like printf(), entry/exit points, loops, conditionals, outputting the value of a key variable, etc.

Runtime debuggers allow you to visualise what the program is doing. You can see each line of code being executed in real-time, and see the values of variables changing as the program is running. You can also add breakpoints to your program. These pause the program in the debugger when a specified line of code is reached.

Rubber Duck Debugging is when you explain the problem and code to yourself (or any inanimate object) out loud. The act of talking about it often makes your brain think differently, however they may be unconscious bias.

You can also use a divide and conquer technique. Reude the place where the bug can hide by creating a minimal reproducable test case and remove as much unnecessary code as possible, whilst still demonstrating the bug.

![image](images/debuggingWorkflow.png)
