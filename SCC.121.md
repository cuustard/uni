began: 8th October 2024

# SCC.121 Fundamentals of Computer Science

This module of the course is taught by 4 Lecturers:

- Hansi Hettiarachchi
- Adrian Friday
- Saad Ezini
- Nigel Davies

This module is assessed with Exams and Coursework:

| Task                             | Week       | Worth |
|----------------------------------|------------|-------|
| Exam                             | Week ??? | 70%   |
| Architecture Quiz                | Week 5, 10, 15, 20     | 5%    |

## Lecture 1 - Module Introduction

noted: 8th October 2024

The module aims for me to  understand the fundamentals of Computer Science. This includes...

- ...the role of discrete mathematics and logic
- ...designing algorithms using common data structures
- ...analysing the efficiency of algorithms
- ...the role of abstract data types


### Sets

A Set is a collection of unique (no duplicates) and unordered objects/elements/members. E.g. `A = {4, 3, 2, 1, 5}`

### Membership

Elements in a set have a membership to that set.

For example, the element 4 is in set A. Write this as `4 ∈ A`. This means 4 'belongs to' or 'is an element of' set A.

However, the element 6 is not in set A. Write this as `6 ∉ A`. This means 6 'does not belong to' or 'is not an element of' set A.

### Defining Sets

Finite and small sets are easy to write out. Take set A: `A = {4, 3, 2, 1, 5}`. This is a finite set with just 5 elements.

Infinite/large sets cannot be enumerated. Instead we provide a property that all the sets members satisfy.

For example, set B: `B = {1, 2, 3, 4, 5, 6...}` and so on until infinity. To write this, we can give this set a property of `x`.

We would say that, every object of `x` such that `x` is an integer and greater than 0. So `B = {x | P(x)}`. This means that B is the set of objects `x` such that `x` has property P.


### Set Operations

- Union: `∪`
- Intersection: `∩`
- Difference `-`
- Cartesian Product `x`

For the following examples, `A = {1, 2, 3, 4}`, `B = {4, 5, 6}`.

Unionisation forms a new set from two sets, made of all the ements from both. Remove duplicates of unique elements. For example, `A ∪ B = {1, 2, 3, 4, 5, 6}`. Here we unionised two sets into one and removed duplicate elements at the same time.

Intersection forms a new set from two sets, made of the elements that are common between the original sets. For example, Take set A and B. `A ∩ B = {4}`. This is because both sets have 4 and nothing else in common.

Difference forms a new set from two sets, made of all the elements from the first set that are not in the second set. For example. `A - B = {1, 2, 3, 5, 6}`.

Cartesian Product:

- An Ordered Pair is a pair of elements, with an order (usually ascending) associated with them.
- An Ordered Pair is written as `<x, y>`. Where `x` and `y` are elements.
- Two Ordered Pairs `<a, b>` and `<c, d>` are equal if `a = c` and `b = d`. This means that `<1, 2>` is not equal to `<2, 1>`.

For Example:

`A x R = {<1, 4>, <1, 5>, <1, 6>, <2, 4>, <2, 5> <2, 6>, <3, 4>, <3, 5>, <3, 6>, <4, 4>, <4, 5>, <4, 6>}`

| Symbol | Symbol name | Meaning |
|---|---|---|
| A ∪ B | union | objects that belong to set A or set B |
| A ∩ B | intersection | objects that belong to set A and set B |
| A - B | difference | objects that belong to set A but not set B |
| A x B | Cartesian product | all ordered pairs with the first element from set A and the second from set B |

## Lecture 2

Types of sets:

- Empty
- Disjoint
- Equal
- Sets of sets
- Subsets & Proper Subsets
- Supersets & Proper Supersets
- Universal
- Commplement

### Empty Sets

An empty/null/void set is one that contains no elements. Written as `{}` or `∅`. For example `Z = {}` or `Z = ∅`

### Disjoint Sets

Sets are disjoint if they have no elements in common (if ther intersection is empty). For example, `A = {1}` is disjoint from `B = {2}`. This is because they have no common elements.

### Equal Sets

Sets are equal if they have exactly the same elements. For example `A = {1, 2, 3}` is equal to `B = {2, 3, 1}`. Written as `A = B`. If sets are unequal use the `≠` symbol. For example, `A ≠ Z`.

### Sets of Sets

Sets can contain atomic elements like letters, numbers, or a pair of elements. They can also contain other sets. For example take `A = {1, {2, 3}}`. Set `A` contains the atomic element `1`, and the set `{2, 3}`.

### Cardinality of Sets

The Cardinality of a set is the number of a sets elements. Written as `|A|`. For example, take the set `A = {1, 2, 3, 4, 5}` so `|A| = 5`. For example, `B = {1, {1, 2}, ∅, 4}` so `|B| = 4`.

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

A Universal set is a non-empty set that contains all the possibl elements relevant to the solution of a given problem. Example: `U = {red, orange, yellow, green, blue, indigo, violet}`.

### Complement Sets

A complement set is the difference between the universal set and a given set. Denoted by `comp(A) = U - A`. For example if `A = {red, yellow, blue}`. Then `comp(A) = {orange, green, indigo, violet}`.


### Summary

| Symbol | Symbol name | Meaning |
|---|---|---|
| ∅ | empty set | set with no elements |
| disjoint sets | sets whose intersection is the empty set |
| A = B | equal sets | sets with the same elements |
| A ≠ B | not equal sets | sets which do not have the same elements |
| A | set cardinality | number of elements in a set A |

| Symbol | Symbol name | Meaning |
|---|---|---|
| A ⊆ B | subset | elements of set A are also in set B |
| A ⊂ B | proper subset | A is subset and there is at least one element in set B that is not in set A |
| B ⊇ A | superset | elements of set A are also in set B |
| B ⊃ A | proper superset | B is superset and there is at least one element in set B that is not in set A |
| U | universal set | set of all of the possible elements relevant to a specific problem |
| comp(A) | complement set | the difference between the universe and a given set A |