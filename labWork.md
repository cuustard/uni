began: 8th October 2024

# Lab Work

1. [Week 1 - Learning the UNIX Shell](#week-1---learning-the-unix-shell)
2. [Week Two - C, Sets, & Number Systems](#week-2---c-sets--number-systems)

| Week | Lecture                                                               | Original Handout                                        | Date Noted |
| ---- | --------------------------------------------------------------------- | ------------------------------------------------------- | ---------- |
| 1    | [Week 1 - Learning the UNIX Shell](#week-1---learning-the-unix-shell) | [Learning the Unix Shell](/Lab/a.weekOneMaterial.pdf)   | 9/10/2024  |
| 2    | [Lecture 2 - Writing Code](#lecture-2---writing-code)                 | [C, Sets, & Number Systems](/Lab/b.weekTwoMaterial.pdf) | 16/10/2024 |
| 3    |                                                                       |                                                         |            |

## Week 1 - Learning the UNIX Shell

UNIX is an Operating System developed in the 1970s. It is still being developed today, as Linux. It's a stable, multi-user, multi-tasking system for servers, desktops and laptops. Linux is UNIX with a GUI.

The Shell is a powerful extensible command line user interface that is the 'power user' interface for interacting with UNIX and the basis for most system administration on any sensible OS platform.

Linux (Ubuntu) is installed on all the lab machines in SCC's lab.

## Week 2 - C, Sets, & Number Systems

noted : 16th October 2024

### SCC.111 C programs

#### Task 1

Create a derivative of the classic ‘hello world’ program, and get it compiling, fixing any errors on the way. Below is what I did in the terminal:

![Screenshot of Terminal](/labScreenshots/a.terminalForHelloWorld.png "Screenshot showing terminal")

- `ls` to list stuff in current directory
- `code helloworld.c` opens new file with extension c, in vscode
- `gcc -o task1 helloworld.c` uses the GNU Compiler Collection (GCC) to compile the C source file helloworld.c and produce an executable file named task1

Below is the C program:

```C
#include <stdio.h>

int main() {
    printf("Hello world\n");
}
```

- Remember `#include <stdio.h>`
- Remember `;`

#### Task 2

![Screenshot of Terminal](/labScreenshots/b.terminalForFemurLength.png "Screenshot showing terminal")

```C
#include <stdio.h>

int main() {
    float femurLength= 0.0;
    float personHeight = 0.0;

    scanf("%f", &femurLength);
    printf("Femur length = %.2f cm\n", femurLength);
    personHeight = (2.38 * femurLength) + 61.41;
    printf("Approx (+/- 3.93cm) height: %.2f cm\n", personHeight);

    return 0;
}
```

#### Task3

![Screenshot of Terminal](/labScreenshots/c.terminalForSquare.png "Screenshot showing terminal")

```C
#include <stdio.h>

int main() {
    int length = 0;
    scanf("%i", &length);

    int i = 0;
    int j = 0;
    for (i = 0; i < length; i++) {
        for (j = 0; j < length; j++) {
            printf("*");
        }
        printf("\n");
    }
}
```

### SCC.121 Sets

#### Questions & Answers

1. Determine whether each of the following pairs of sets is equal:

   - {1, 3, 5} and {5, 3, 1}
     - {1, 3, 5} = {5, 3, 1} as order of elements does not matter. Same 3 elements in list so equal.
   - {1, 3, 5} and {5, 1, 6}
     - {1, 3, 5} ≠ {5, 1, 6} as different elements in both sets. 3 and 6.

2. Let A = {1, 2, 3, 4, 5} and B = {0, 3, 6}. Find:

   - A ∩ B
     - A ∩ B = {3}
   - A ∪ B
     - A ∪ B = {0, 1, 2, 3, 4, 5, 6}
   - A – B
     - A – B = {1, 2, 4, 5}
   - B − A
     - B - A = {0, 6}

3. Let A = {0, 2, 4, 6, 8, 10}, B = {0, 1, 2, 3, 4, 5, 6} and C = {4, 5, 6, 7, 8, 9, 10}. Find:

   - A ∩ B ∩ C
     - A ∩ B ∩ C = {4, 6}
   - A ∪ B ∪ C
     - A ∪ B ∪ C = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
   - (A ∪ B) ∩ C
     - A ∪ B = {0, 1, 2, 3, 4, 5, 6, 8, 10}
     - (A ∪ B) ∩ C = {4, 5, 6, 8, 10}
   - (A ∩ B) ∪ C
     - A ∩ B = {0, 2, 4, 6}
     - (A ∩ B) ∪ C = {0, 2, 4, 6, 7, 8, 9, 10}

4. If A = {1, 2, 3, a}, B = {1, 2, 3, 4, 5}, C = {a, b} evaluate:

   - A ∪ (B ∩ C)
     - B ∩ C = {} = ∅
     - A ∪ (B ∩ C) = {1, 2, 3, a}
   - (A ∪ B) ∩ C
     - A ∪ B = {1, 2, 3, 4, 5, a}
     - (A ∪ B) ∩ C = {a}
   - C – A
     - C – A = {b}
   - (A – B) – C
     - A – B = {a}
     - (A – B) – C = {b}
   - A – (B – C)
     - B – C = {1, 2, 3, 4, 5}
     - A – (B – C) = {a}
   - (A ∩ C) ∪ B
     - A ∩ C = {a}
     - (A ∩ C) ∪ B = {1, 2, 3, 4, 5, a}
   - A ∩ (C ∪ B)
     - C ∪ B = {1, 2, 3, 4, 5, a, b}
     - A ∩ (C ∪ B) = {1, 2, 3, a}

5. Let A be the set of students who live within one mile of school and B the set of students who walk to
   classes. Describe the students in each of the following sets, in English. - A ∩ B - Intersection of A and B. So this is the set of students that walk to classes and live within one mile of school. - set of studetns who live within one mile of school AND the set of studetns who walk to classes. - A ∪ B - Union of A and B. So this is the set of students that walk to classes or live within one mile of school, or both. - the set of students who live within one mile of school OR the set of students who walk to classes. - A – B - Difference of A and B. So this is the students that live within one mile of school subtracting the students who walk to classes. - the set of students who live within one mile of school AND the set of students who do not walk to classes - B – A - Difference of B and A. So this is the students that walk to school subtracting the students who live within one mile of school. - the set of students who walk to classes AND the set of students who live more than one mile of school

6. Let A = {a, b, c} and B = {y, z}. Find

   - A x B
     - A x B = {<a, y>, <a, z>, <b, y>, <b, z>, <c, y>, <c, z>}
   - B x A
     - B x A = {<y, a>, <y, b>, <y, c>, <z, a>, <z, b>, <z, c>}

7. How many different elements does A x B have if A has m elements and B has n elements?

   - A x B will have m\*n elements.

8. List the members of the following sets

   - {x | x is a positive integer less than 12}
     - {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11}
   - {x | x is the square of an integer and x < 100}
     - {1, 4, 9, 16, 25, 36, 49, 64, 81}

9. For each of the following sets, determine if 2 is an element of that set.

   - { x ∈ R | x is an integer greater than 1}
     - Yes. 2 is a real number and 2 is an integer greater than 2. So 2 is an element of that set.
   - {x ∈ R | x is the square of an integer}
     - No. 2 is a real number but 2 is not a square of an integer. So 2 is not an element of that set.

10. Identify 2 sets whose cardinality is 1 and whose intersection’s cardinality is also 1.

    - A = {1} and B = {1}. |A| = 1 and |B| = 1. A ∩ B = {1}. |A ∩ B| = 1

11. Which of the following is not a proper subset of set A if A = {4, 5, 6, x, y, z}?

    - {4, x, y}
      - Is a proper subset. The elements in this set are all in set A, but set A also has other unique elements.
    - {3, 4, 5}
      - Not a proper subset or a subset. There is an element 3 in this set that is not in A at all.
    - {4, 5, 6}
      - Is a proper subset. The elements in this set are all in set A, but set A also has other unique elements.
    - Ø
      - Not a proper subset or a subset. Ø = {}. There is no nested set of {} in set A.

12. Which is a subset of set A? A = {a, {b}, c, {c}, {x, y}}

    - {a, {b}, c}
      - Is a proper subset. The elements in this set are all in set A, but set A also has other unique elements.
    - {a, b, c}
      - Not a proper subset or a subset. There is an element b in this set that is not in A.
    - {c, x, y}
      - Not a proper subset or a subset. There are elements x and y in this set that is not in A.
    - {x, y}
      - Not a proper subset or a subset. There is an element x and y in this set that is not in A. It would be a proper subset if the set in question was {{x, y}}.

13. Which is false?

    - 1, 2 ⊆ 1, 2, 3
      - True
    - 1, 2 ⊆ 2, 3, 4
      - False
    - ∅ ⊆ 1, 2, 3
      - False

14. Let Universal set U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}, and its 3 sets: E = {2, 4, 6, 8, 10}, O = {x | x is an
    odd number}, and T = {3}. - Enumerate the elements of set O - {1, 3, 5, 7, 9} - What operation can be applied to set E and U to get set O? - comp(E) = O - Define set E through its elements’ property - E = {x | x is an even number} - Which of the sets above are subsets of set O? - Set T and O - Which of the sets above are proper subsets of set O? - Set T - Which of the sets above are proper supersets of empty set? - All of them

### SCC.131 Number Systems

1. Convert the following unsigned binary numbers to decimal:

   - 00001001
     - 9
   - 00101011
     - 43
   - 01001111
     - 79
   - 01111110
     - 126
   - 10000110
     - 134

2. Convert the following decimal numbers to unsigned 8-bit binary:

   - 22
     - 00010110
   - 19
     - 00010011
   - 84
     - 01010100
   - 120
     - 01111000
   - 93
     - 01011101

3. Add the following pairs of unsigned 8-bit binary numbers. Give your answer in unsigned 8-bit binary.
   - 00000100 + 00000011
     - 00000111
   - 00000110 + 00001101
     - 00010011
   - 00001111 + 00010101
     - 00100100
   - 11101001 + 01011110
     - 101000111 9 bits now? what happens to overflow bit (msb). discard overflow: 01000111
   - 11100000 + 00110000
     - 100010000 9 bits now? what happens to overflow bit (msb). discard overflow: 00010000
