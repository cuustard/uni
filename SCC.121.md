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

| Task                       | When                | Worth           |
| -------------------------- | ------------------- | --------------- |
| "Coursework" (In-lab quiz) | Week 5, 10, 15, 20  | 20% (5% each)   |
| "Summer Project"           | Summer Term         | 10%             |
| Exam                       | Summer Term         | 70%             |

---

### Table of Contents

| Week  | Lecture                                                                           | Original Slides                                                                | Noted  |
| ----- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ | ------ |
| 1     | [Lecture 1 - Module Introduction & Sets](#lecture-1---sets)                       | [Sets](/SCC.121.slides/b.setsPartOne.pdf)                                      | ✅     |
| 1     | [Lecture 2 - Types of Sets](#lecture-2---types-of-sets)                           | [Types of Sets](/SCC.121.slides/c.setsPartTwo.pdf)                             | ✅     |
| 2     | [Lecture 3 - Relations](#lecture-3---relations)                                   | [Relations](/SCC.121.slides/d.relationsPartOne.pdf)                            | 🟧     |
| 2     | [Lecture 4 - Relations Part 2](#lecture-4---relations-part-2)                     | [Relations Part 2](/SCC.121.slides/e.relationsPartTwo.pdf)                     | ❌     |
| 3     | [Lecture 5 - Functions](#lecture-5---functions)                                   | [Functions](/SCC.121.slides/f.functions.pdf)                                   | ❌     |
| 3     | [Lecture 6 - Functions Part 2](#lecture-6---functions-part-2)                     | [Functions Part 2](/SCC.121.slides/g.functionsPartTwo.pdf)                     | ❌     |
| 4     | [Lecture 7 - Propositional Logic](#lecture-7---propositional-logic)               | [Propositional Logic](/SCC.121.slides/h.propositionalLogic.pdf)                | ✅     |
| 4     | [Lecture 8 - Propositional Logic Part 2](#lecture-8---propositional-logic-part-2) | [Propositional Logic Part 2](/SCC.121.slides/i.propositionalLogicPartTwo.pdf)  | ✅     |
| 5     | [Lecture 9 - Predicate Logic](#lecture-9---predicate-logic)                       | [Predicate Logic](/SCC.121.slides/j.predicateLogic.pdf)                        | ❌     |
| 5     | [Lecture 10 - Predicate Logic Part 2](#lecture-10---predicate-logic-part-2)       | [Predicate Logic Part 2](/SCC.121.slides/k.predicateLogicPartTwo.pdf)          | ❌     |

---

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

| Symbol  | Symbol name        | Meaning                                                                        |
| ------- | ------------------ | ------------------------------------------------------------------------------ |
| A ∪ B   | Union              | Elements that belong to set A **or** set B                                     |
| A ∩ B   | Intersection       | Elements that belong to set A **and** set B                                    |
| A - B   | Difference         | Elements that belong to set A but not set B                                    |
| A x B   | Cartesian Product  | All ordered pairs with the first element from set A and the second from set B  |

---

---

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

| Symbol   | Symbol name      | Meaning                                                                        |
| -------- | ---------------- | ------------------------------------------------------------------------------ |
| ∅        | Empty Set        | Set with no elements                                                           |
|          | Disjoint Sets    | Sets whose intersection is the empty set                                       |
| A = B    | Equal Sets       | Sets with the same elements                                                    |
| A ≠ B    | Unequal Sets     | Sets which do not have the same elements                                       |
| A        | Set Cardinality  | Number of elements in a set                                                    |
| A ⊆ B    | Subset           | Elements of set A are also in set B                                            |
| A ⊂ B    | Proper Subset    | A is a subset and there is at least one element in set B that is not in set A  |
| B ⊇ A    | Superset         | Elements of set A are also in set B                                            |
| B ⊃ A    | Proper Superset  | B is superset and there is at least one element in set B that is not in set A  |
| U        | Universal Set    | Set of all of the possible elements relevant to a specific problem             |
| comp(A)  | Complement Set   | The difference between the universe and a given set A                          |

---

---

## Lecture 3 - Relations

![Associations](images/associations.png "Diagram showing example of assocations between students and academic courses")

Pairs of objects are related in specific ways. We can represent a relationship by describing what course each student takes. Starting from the student and ending with the course. We specify the relationship this way because it is a student that takes a course; a course does not take a student.

Relations are asymmetric. The direction matters because the order of elements in the order pair matters.

The cartesian product will give us all possible ordered pairs (12 in this example). But there are only 5 relations. In real life, which students take which course could be all the possible pairs, but often it will be a subset of the cartesian product.

A binary relation is an ordered pair where two elements are brought together.

Binary Relation R from set A to set B, or over `A x B`. A set of ordered pairs `<a, b>`, `a ∈ A` and `b ∈ B`. An ordered pair `<a, b> ∈ R`. This means element a is related to element b through the relation R.

The relationship between R and A x B is as follows:

- A x B is the set of all ordered pairs (the cartesian product)
- R is a subset of `A x B`. So `R ⊆ A x B`. It is not a proper subset as R could be the cartesian product.

In the above diagram, Relation T (Takes):

- John Takes course1
    - `<John, course1> ∈ T`
- Jim Takes course1
    - `<Jim, course1> ∈ T`
- Helen Takes course2 and course3
    - `<Helen, course2> ∈ T`
    - `<Helen, course3> ∈ T`
- Mary Takes course3
    - `<Mary, course3> ∈ T`

Another example:

- `A = {0, 1, 2, 3}` and `B = {0, 1, 2, 3, 4}`
- List the ordered pairs in the relation R from A to B that satisfy `<a, b> ∈ R`, if `b - a = 1`.
- `b - a = 1` is equivilant to `b = a + 1`. So `<a, b> = <a, a + 1>`:
- So the relation R looks like: `R = {<0, 1>, <1, 2>, <2, 3>, <3, 4>}`

---

---

## Lecture 4 - Relations Part 2

---

---

## Lecture 5 - Functions

---

---

## Lecture 6 - Functions Part 2

---

---

## Lecture 7 - Propositional Logic

Logic is the study of reasoning. It is a rational way of drawing conclusions.

A proposition is a claim about how things are. It can either be true OR false. Not both. For example:

True propositions:

- Grass is green
- Snow is white
- 2 + 2 = 4

False propositions:

- Grass is red
- Snow is pink
- 2 + 2 = 5

The following are examples of non-propositions

- Is the water warm?
- Go for it!
- Where are we?
- Put the phone down!
- Ouch!

An Atomic proposition is one that is true or false value does not depend on that of any other proposition.

A compound proposition is one which is constructed from atomic propositions by combining them with fundamental connectives.

### Truth Tables

These tabulate the value of a compound proposition for all possible values of its atomic propositions and their combination. For example, the truth table for 2 atomic propositions:

| P   | Q   | Compound  |
| --- | --- | --------- |
| F   | F   |           |
| F   | T   |           |
| T   | F   |           |
| T   | T   |           |

### Fundamental Connectives

| Operation      | Symbols  |
| -------------- | -------- |
| AND            | ⋀        |
| OR             | ⋁        |
| XOR            | ⊕, ⊻     |
| NOT            | ~, ¬     |
| Conditional    | →        |
| Biconditional  | ⇔        |

#### AND

![AND Connective](images/connectiveAND.png)

#### OR

![OR Connective](images/connectiveOR.png)

#### XOR

![XOR Connective](images/connectiveXOR.png)

#### NOT

![NOT Connective](images/connectiveNOT.png)

#### Conditional / Implication

IF antecedent THEN consequent. For example: IF the train is late, THEN we will miss our flight.

This combines two propositions into a third proposition called the conditional or implication. The conditional/implication is false when the antecedent is True and the consequent is False.

![Conditional / Implication](images/conditionalImplicational.png)

#### Biconditional

The biconditional is only True when both propositions have the same truth value.

![Biconditional](images/biconditional.png)

### Logical Properties

Tautologies are propositions which are always True, regardless of the truth values of their atomic propositions. For example, Q = "I passed the exam". ~Q = "I did not pass the exam!.

![Tautologies](images/tautologies.png)

Contradictions are propositions which are always false, regardless of the truth values of their atomic propositions. For example, Q = "I passed the exam". ~Q = "I did not pass the exam!.

![Contradictions](images/contradictions.png)

Contingencies are propositions that are neither tautologies nor contradictions. For example, P = "I passed the exam". ~P = "I did not pass the exam".

Contingencies have both True's and Falses in their truth tables.

![Contingencies](images/contingencies.png)

Equivalence is when two propositions are logically equivalent if they have the exact same truth value under all circumstances. Written `P ≡ Q`.

---

---

## Lecture 8 - Propositional Logic Part 2

### Logical Reasoning

- An Argument is a sequence of propositions that end with a conclusion.
    - The argument is VALID if, given that the premises are true, then the conclusion is true.
- A Premise is the basis on which we establish the conclusion.
- A Conclusion is a claim that we try to establish as true.

Written in the form:

![Logcal Reasoning Writen Form](images/logcialReasoning.png)

### Propositional Logic

Building blocks of propositional logic:

- Atomic & Compound Propositions
- Fundamental Connectives

A rule is a function that takes propositions as premises and returns others as conclusions.

- **Inference Rules**: templates for building valid arguments
- **Replacement Rules**: replaces parts of propositions with logically equivalent expressions

### Inference Rules

Inference rules give methods to evaluate the validity of arguments. They highlight logical reasoning behind a valid argument are justify stems from premises to conclusion. An alternative to this is truth tables, but these are inconvenient with more propositions and are less intuitive.

The rules:

| Rule                                      | Description                                                                                                                                                                                                         | Example Image                                                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| Modus Ponens                              | one premise is a conditional statement, the other premise affirms the antecedent and the conclusion affirms the consequent                                                                                          | ![Modus Ponens Example](images/modusPonens.png "Diagram showing example of Modus Ponens Rule")                                |
| Modus Tollens                             | one premise is a conditional statement, the other premise denies the consequent, and the conclusion denies the antecedent                                                                                           | ![Modus Tollens Example](images/modusTollens.png "Diagram showing example of Modus Tollens Rule")                             |
| Addition (disjunction introduction)       | the premise is a proposition, and the conclusion is a disjunction formed by that proposition and any other proposition                                                                                              | ![Addition Example](images/addition.png "Diagram showing example of Addition Rule")                                           |
| Simplification (conjunction elimination)  | the premise is a conjunction, and the conclusion is either of the propositions forming the conjunction                                                                                                              | ![Simplification Example](images/simplification.png "Diagram showing example of Simplification Rule")                         |
| Hypothetical Syllogism                    | the premises are two conditionals such as P → Q and Q → R so that one’s antecedent matches the consequent of the other, and the conclusion is another conditional which results from the chain of reasoning: P → R  | ![Hypothetical Syllogism Example](images/hypotheticalSyllogism.png "Diagram showing example of Hypothetical Syllogism Rule")  |
| Disjunctive Syllogism                     | one premise is a disjunction, the other premise denies one of the propositions in the disjunction, and the conclusion affirms the other proposition in the disjunction                                              | ![Disjunctive Syllogism Example](images/disjunctiveSyllogism.png "Diagram showing example of Disjunctive Syllogism Rule")     |
| Absorption                                | the premise is a conditional: P → Q, and the conclusion is also a conditional whose consequent is a conjunction of the consequent and antecedent: P → ( P ∧ Q )                                                     | ![Absorption Example](images/absorption.png "Diagram showing example of Absorption Rule")                                     |

### Replacement Rules

| Rule/Law             | Description                                                                                                                                                                                                   | Example                                                                   |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- |
| Commutative law      | The order of laws does not affect the result of the conjunction or disjunction                                                                                                                                | `P ∨ Q` = `Q ∨ P` / `P ∧ Q` = `Q ∧ P`                                     |
| Associative law      | The grouping of propositions does not affect the result of the conjunction or disjunction                                                                                                                     | `(P ∨ Q) ∨ R` = `P ∨ (Q ∨ R)` / `(P ∧ Q) ∧ R` = `P ∧ (Q ∧ R)`             |
| Distributive law     | 'Multiply' out the brackets                                                                                                                                                                                   | `P ∧ (Q ∨ R)` = `(P ∧ Q) ∨ (P ∧ R)` / `P ∨ (Q ∧ R)` = `(P ∨ Q) ∧ (P ∨ R)` |
| De Morgan’s laws     |                                                                                                                                                                                                               | `~P ∧ ~Q` = `~(P ∨ Q)` / `~P ∨ ~Q` = `~(P ∧ Q)`                           |
| Absorption law       | The disjunction of any proposition P with (P ∧ Q) has the same truth value as P                                                                                                                               | `P ∨ (P ∧ Q)` = `P` / `P ∧ (P ∨ Q)` = `P`                                 |
| Identity law         | The conjunction of any proposition P with an arbitrary tautology T has the same truth value as P. <br> The disjunction of any proposition P with an arbitrary contradiction F has the same truth value as P   | `P ∧ T` = `P` <br> `P ∨ F` = `P`                                          |
| Idempotence law      | The property of a conjunction or disjunction to be applied multiple times on a proposition without changing the proposition                                                                                   | `P ∧ P` = `P` / `P ∨ P` = `P`                                             |
| Negation law         | The disjunction of any proposition P and its negation is a tautology                                                                                                                                          | `P ∨ ~P` = `True` / `P ∧ ~P` = `False`                                    |
| Double negation law  |                                                                                                                                                                                                               | `~(~P)` = `P`                                                             |
| Implication law      | Implication can be expressed by disjunction and negation                                                                                                                                                      | `P → Q` = `~P ∨ Q`                                                        |
| Contraposition law   |                                                                                                                                                                                                               | `P → Q` = `~P → ~Q`                                                       |
| Equivalence law      | A biconditional is equivalent to the conjunction of two conditionals                                                                                                                                          | `P <--> Q` = `(P → Q) ∧ (Q → P)`                                          |

- Commutative law – states that a compound proposition involving exclusively ANDs, or exclusively ORs is unaltered by reordering its atomic propositions.
- Associative law – states that a compound proposition involving exclusively ANDs or exclusively ORs is unaltered by regrouping its atomic propositions.
- Distributive law – states that a compound proposition involving AND, OR and parentheses, is unaltered by distributing the first connective to link the first proposition separately with each proposition in the parentheses.
- De Morgan's law states that the conjunction of negations is the negation of a disjunction: ~P  ~Q is equivalent to ~(P  Q).
- Absorption law states that the disjunction of any proposition P with (P ∧ Q) has the same truth value as P: P ∨ (P ∧ Q) is equivalent to P; the conjunction of any proposition P with (P ∨ Q) has the same truth value as P: P∧ (P ∨ Q) is equivalent to P.
- Identity law states that the conjunction of any proposition P with an arbitrary tautology has the same truth value as P; the disjunction of any proposition P with an arbitrary contradiction F (a proposition which is always false) has the same truth value as P.
- Idempotence law states the property of a conjunction or disjunction to be applied multiple times on a proposition without changing the proposition: P ∧ P is logically equivalent to P, P ∨ P is logically equivalent to P.
- Negation law states that the disjunction of any proposition P and its negation is a tautology; the conjunction of any proposition P and its negation is a contradiction.
- Doble negation law states that any proposition P is logically equivalent to its double negation ~(~P)
- Implication law states that any implication P → Q is logically equivalent to ~P ∨ Q.
- Contraposition law states that a conditional P → Q is logically equivalent to its contrapositive (implication of negations): ~Q → ~P.
- Equivalence law states that a biconditional P  Q is logically equivalent to the conjunction of two conditionals: (P → Q)  (Q → P).

---

---

## Lecture 9 - Predicate Logic

---

---

## Lecture 10 - Predicate Logic Part 2
