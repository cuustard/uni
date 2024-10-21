began: 8th October 2024

# SCC.121 Fundamentals of Computer Science

This module of the course is taught by 4 Lecturers:

- Discrete Maths & Logic
  - Taught by Corina Sas
  - Weeks 1 - 5
- Data Structures
  - Taught by Amit Chorpra
  - Weeks 6 - 11
- Algorithms & Complexity
  - Taught by Emma Wilson
  - Weeks 12 - 15
- Sorting, Trees, & Graphs
  - Taught by Fabien Dufoulon
  - Weeks 16 - 20
- Linear Algebra, Searching & Sorting, Sorting & its efficiency, PageRank, Revision Lectures
  - Taught by Mixed Lecturers
  - Weeks 21 - 25

The module aims to help me understand the fundamentals of Computer Science. This includes...

- ...the role of discrete mathematics and logic
- ...designing algorithms using common data structures
- ...analysing the efficiency of algorithms
- ...the role of abstract data types

Assessed with Exams and Coursework:

| Task       | Type          | Week               | Worth |
| ---------- | ------------- | ------------------ | ----- |
| Exam       |               | Summer Term        | 70%   |
| Coursework | "in-lab quiz" | Week 5, 10, 15, 20 | 30%   |

---

### Table of Contents

| Week | Lecture                                                       | Original Slides                                            | Date Noted |
| ---- | ------------------------------------------------------------- | ---------------------------------------------------------- | ---------- |
| 1    | [Lecture 1 - Module Introduction & Sets](#lecture-1---sets)   | [Sets](/SCC.121.slides/b.setsPartOne.pdf)                  | 8/10/2024  |
| 1    | [Lecture 2 - Types of Sets](#lecture-2---types-of-sets)       | [Types of Sets](/SCC.121.slides/c.setsPartTwo.pdf)         | 10/10/2024 |
| 2    | [Lecture 3 - Relations](#lecture-3---relations)               | [Relations](/SCC.121.slides/d.relationsPartOne.pdf)        | 15/10/2024 |
| 2    | [Lecture 4 - Relations Part 2](#lecture-4---relations-part-2) | [Relations Part 2](/SCC.121.slides/e.relationsPartTwo.pdf) | 17/10/2024 |

---

## Lecture 1 - Sets

A Set is a collection of unique and unordered objects/elements/members. E.g. `A = {4, 3, 2, 1, 5}`

### Membership

Elements in a set have a membership to that set.

For example, the element 4 is in set A. Write this as `4 ∈ A`. This means 4 'belongs to' or 'is an element of' set A.

However, the element 6 is not in set A. Write this as `6 ∉ A`. This means 6 'does not belong to' or 'is not an element of' set A.

### Defining Sets

Finite and small sets are easy to write out. For example, set A: `A = {4, 3, 2, 1, 5}` is finite with just 5 elements.

Infinite/large sets cannot be enumerated. Instead, we provide a property that all the set's elements satisfy.

For example, set B: `B = {1, 2, 3, 4, 5, 6...}` and so on until infinity. To write this, we can give this set a property of x. We would say that, every element of x such that x is an integer and greater than 0. So `B = {x | P(x)}`. This means that B is the set of elements x such that x has the property P.

### Set Operations

- Union: `∪`
- Intersection: `∩`
- Difference `-`
- Cartesian Product `x`

For the following examples: `A = {1, 2, 3, 4}`, `B = {4, 5, 6}`.

Unionisation forms a new set from two sets, made of all the elements from both. Any duplicates of an element are removed. For example, `A ∪ B = {1, 2, 3, 4, 5, 6}`. Here we unionised two sets into one and removed duplicate element, 4, at the same time.

Intersection forms a new set from two sets, made of the elements that are common between A and B. For example, `A ∩ B = {4}`. This is because both sets have element 4, and nothing else, in common.

Difference forms a new set from two sets, made of all the elements from the first set that are not in the second set. For example. `A - B = {1, 2, 3}`.

To understand Cartesian Product, first I need to understand Ordered Pairs:

- An Ordered Pair is a pair of elements, with an order (usually ascending) associated with them
- An Ordered Pair is written as `<x, y>`. Where x and y are elements
- Two Ordered Pairs `<a, b>` and `<c, d>` are equal if `a = c` and `b = d`. This means that `<1, 2>` is not equal to `<2, 1>`

The Cartesian Product of two sets creates a set of all possible ordered pairs between the sets. For example:

```
A x B =
{
  <1, 4>, <1, 5>, <1, 6>,
  <2, 4>, <2, 5> <2, 6>,
  <3, 4>, <3, 5>, <3, 6>,
  <4, 4>, <4, 5>, <4, 6>
}
```

Summary of set operations:

| Symbol | Symbol name       | Meaning                                                                       |
| ------ | ----------------- | ----------------------------------------------------------------------------- |
| A ∪ B  | Union             | Elements that belong to set A **or** set B                                    |
| A ∩ B  | Intersection      | Elements that belong to set A **and** set B                                   |
| A - B  | Difference        | Elements that belong to set A but not set B                                   |
| A x B  | Cartesian Product | All ordered pairs with the first element from set A and the second from set B |

## Lecture 2 - Types of Sets

Types of sets:

- Empty
- Disjoint
- Equal
- Sets of sets
- Subsets & Proper Subsets
- Supersets & Proper Supersets
- Universal
- Complement

### Empty Sets

An empty/null/void set contains no elements. Written as `{}` or `∅`. For example `Z = {}` can also be written as `Z = ∅`.

### Disjoint Sets

Sets are disjoint if they have no elements in common (if their intersection is empty). For example, `C = {1, 2, 3}` is disjoint from `D = {4, 5, 6}`. This is because they have no common elements.

### Equal Sets

Sets are equal if they have the same elements. For example `E = {1, 2, 3}` is equal to `F = {2, 3, 1}`. Written as `C = D`. If sets are unequal use the `≠` symbol. For example, `D ≠ E`.

### Sets of Sets

Sets can contain atomic elements like letters, numbers, or a pair of elements. They can also contain other sets. For example take `A = {1, {2, 3}}`. Set `A` contains the atomic element `1`, and the set `{2, 3}`.

### Cardinality of Sets

The Cardinality of a set is the number of a set's elements. They are written as `|A|`. For example, `A = {1, 2, 3, 4, 5}` so `|A| = 5`. For example, `B = {1, {1, 2}, ∅, 4}` so `|B| = 4`.

### Subsets & Supersets

Set A is a subset of set B if every element of A is also an element of B. This is written as `A ⊆ B`. This would mean that if `x ∈ A`, then `x ∈ B` In some cases A could also be equal to B.

For example, if `A = {1, 2, 3}` and `B = {1, 2, 3, 4, 5}` then:

- `1 ∈ A` and `1 ∈ B`
- `2 ∈ A` and `2 ∈ B`
- `3 ∈ A` and `3 ∈ B`

All of A's elements are in B so `A ⊆ B`.

This makes B a superset of A. Written `B ⊇ A`.

#### Proper Subsets & Proper Supersets

A is also a proper subset of B because B has some elements not in A. So `A ⊂ B`. This makes B a superset of A. Written as `B ⊃ A`. This also means that for a Proper Subset, `A ≠ B`.

### Universal Sets

A Universal set is a non-empty set that contains all the possible elements relevant to the solution of a given problem. Example: `U = {red, orange, yellow, green, blue, indigo, violet}`.

### Complement Sets

A complement set is the difference between the universal set and a given set. Denoted by `comp(A) = U - A`. For example if `A = {red, yellow, blue}` then `comp(A) = {orange, green, indigo, violet}`.

Summary of Type of sets:

| Symbol  | Symbol name     | Meaning                                                                       |
| ------- | --------------- | ----------------------------------------------------------------------------- |
| ∅       | Empty Set       | Set with no elements                                                          |
|         | Disjoint Sets   | Sets whose intersection is the empty set                                      |
| A = B   | Equal Sets      | Sets with the same elements                                                   |
| A ≠ B   | Unequal Sets    | Sets which do not have the same elements                                      |
| A       | Set Cardinality | Number of elements in a set                                                   |
| A ⊆ B   | Subset          | Elements of set A are also in set B                                           |
| A ⊂ B   | Proper Subset   | A is a subset and there is at least one element in set B that is not in set A |
| B ⊇ A   | Superset        | Elements of set A are also in set B                                           |
| B ⊃ A   | Proper Superset | B is superset and there is at least one element in set B that is not in set A |
| U       | Universal Set   | Set of all of the possible elements relevant to a specific problem            |
| comp(A) | Complement Set  | The difference between the universe and a given set A                         |

## Lecture 3 - Relations

## Lecture 4 - Relations Part 2
