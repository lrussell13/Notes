# Discrete Mathematics

## Set Theory

### Definitions
Set
: A set is a collection of unordered, distinct objects(could be numbers, could be something else) that we call elements.

### Important Points
- There is no order in a set
- Repeated elements are listed once in a set
- Sets can be finite or infinite

### Important Sets
- Natural Numbers: Set of positive integers
: *N* = {1,2,3,4,... . .}

- Integers: Includes all positive an negative integers
: *Z* = {... . . -2,-1,0,1,2, ... . .}

- Rational Numbers: Include any number you can write as a fraction
: *Q* = {m/n | m, n ε *Z* and n ≠ 0}

### Elements and Cardinality
- Symbol for inclusion is ε (Epsilon)
  * For exclusion, simply put a dash through the epsilon

- Cardinality: The size of a set(number of elements)
  * Notated by straight lines on both sides ie. |A|

### Set Building Notation
- We can create rules and use variables when describing and building a set

: Set Builder Notation = {Rule | Conditions for variables}

### The Empty Set
- The empty set is a special type of set with no elements inside of it
  * {} = ∅
  * |∅| = 0
  * |{∅}| = 1

### Subsets
- B is a subset of A if every element in B is also in A
  * We write this as B ⊆ A
  * The empty set is a subset of any and all sets
  * B is a ⊂ (proper subset) A, if B ⊆ A and B ≠ A

### Power Sets
- The set of all possible subsets
  * Notated by P(A)

- To determine the power set by hand, you can use the tree method:
  * Begin with the empty set then move down one element at a time, either adding the element , or keeping the element out of your set
  * After doing this for all elements, the bottom row will be your power set.

- To determine cardinality of power set:
  * if |A| = n, then |P(A)| = 2<sup>n</sup>

- Possible areas of confusion:
  * P(∅) = {∅}
  * P({∅}) = {∅, {∅}}

### Set Operations
- Each and every subset A is in a universe U
  * A ⊆ U

- Complement of A: Everything in the universe that is not in A (Notated by A<sup>c</sup> or Ā)
  * : Ā = U - A = {x | x ∉ A}

- Intersection of A and B: A ∩ B is the intersection of A and B
  * A ∩ B = {x | x ε A and c ε B}

- Union of A and B: A ∪ B is the union of A and B
  * A ∪ B = {x | x ε A or x ε B}
  * Inclusive or

- Difference of A and B: A - B is the difference of A and B
  * A - B = {x|x ε A and x ∉ B}

### Cartesian Products and Order Pairs
- Order Pair: An ordered pair (a, b) of elements in A is defined to be the set {a, {a,b}}
- The Cartesian Product: The Cartesian Product, AxB, is the set {(a,b)| a ε A and b ε B}
  * Example: Let A = {2,4,6} nd B = {2,4}
  * AxB = {(2,2),(2,4),(4,2),(4,4),(6,2),(4,6)}
- Properties of Cartesian Products:
  * Cardinality will be mn, where m = |A| and n = |B|
  * Order matters: BxA ≠ AxB unless A = B  
  * Empty Set: Ax∅ = ∅

## Propositional Logic

### Definitions
Proposition
: A declarative sentence that is either true or false 

### Syntax
- Propositions are denoted with capital letters: P, Q, and R

### Connectives
- Connectives are used for making compound propositions

| Name | Represented | Meaning |
| --- | --- | --- |
| Negation | ¬p | "not p" |
| Conjunction | p ^ q | "p and q" |
| Disjunction | p ∨ q | "p or q" |
| Exclusive Or | p ⊕ q | "p or q, but not both" |
| Implication | p ⇒ q| "if p then q" | 
| Bi-conditional | p ⇔ q| "p if and only if q" |

### Truth Tables
Used to show all possible combinations of statements and connectives along with their truth values.

#### Negation Example

| p | ¬p |
| --- | --- |
| T | F |
| F | T |

#### Conjunction Example (^, "and")

| p | q | p ^ q |
| --- | --- | --- |
| T | F | F | 
| T | T | T |
| F | T | F |
| F | F | F |

#### Disjunction Example (∨, "or")

| p | q | p ∨ q |
| --- | --- | --- |
| T | F | T | 
| T | T | T |
| F | T | T |
| F | F | F |

#### Exclusive Or Example (⊕, "xor")

| p | q | p ⊕ q |
| --- | --- | --- |
| T | F | T | 
| T | T | F |
| F | T | T |
| F | F | F |

#### Implication Example (⇒, "if p then q")

| p | q | p ⇒ q |
| --- | --- | --- |
| T | F | F | 
| T | T | T |
| F | T | T |
| F | F | T |

#### Bi-conditional Example (⇔, "p if and only if q")

| p | q | p ⇔ q |
| --- | --- | --- |
| T | F | F | 
| T | T | T |
| F | T | F |
| F | F | T |

### Proofs Using Truth Tables
Formulas p and q are logically equivalent if and only if the truth conditions of p are the same as the truth conditions of q

#### Example
Show that ¬(p ∨ q) ≡ ¬p ^ ¬q

| p | q | ¬p | ¬q | p ∨ q | ¬(p ∨ q) | ¬p ^ ¬q
| --- | --- | --- | --- | --- | --- | --- |
| T | T | F | F | T | F | F |
| T | F | F | T | T | F | F |
| F | T | T | F | T | F | F |
| F | F | T | T | F | T | F |

The last two columns are equivalent, therefore ¬(p ∨ q) ≡ ¬p ^ ¬q

#### Definitions
Tautology: A statement that always produces truth

Contradiction: A statement that always produces false

### Basic Laws of Logic
Assume T is a tautology and F is a contradiction

#### Double Negation Law
- ¬¬p ⇔ p

#### Identity Laws
- p ^ T ⇔ p
- p ∨ F ⇔ p

#### Domination Laws
- p ∨ T ⇔ T
- p ^ F ⇔ F

#### DeMorgan's Laws
- ¬(p ^ q) ⇔ ¬p ∨ ¬q
- ¬(p ∨ q) ⇔ ¬p ^ ¬q 

### Advanced Laws of Logic
Assume T is a tautology and F is a contradiction

#### Distributive Law
- p ^ (q ∨ r) ⇔ (p ^ q) ∨ (p ^ r)
- p ∨ (q ^ r) ⇔ (p ∨ q) ^ (p ∨ r)

#### Absorption Laws
- p ^ (p ∨ q) ⇔ p
- p ∨ (p ^ q) ⇔ p

#### Commutativity Laws
- p ^ q ⇔ q ^ p
- p ∨ q ⇔ q ∨ p

#### Associativity Law
- p ^ (q ^ r) ⇔ (p ^ q) ^ r

#### Inverse Laws
- p ^ ¬p ⇔ F
- p ∨ ¬p ⇔ T

#### Conditional Law
- p ⇒ q ⇔ ¬p ∨ q

## Combinations and Permutations

### Introduction to Counting

#### Principle of Addition (Sum Rule of Counting)
For two separate tasks, if task A can be done n ways and task B can be done m ways then A and B can be done in n + m ways.

Ex: How many different ways can you draw a jack or an ace in a standard deck of cards?
- 8 different ways

#### Product Principle (Product Rule of Counting)
In a list, A through B, if there are n ways of choosing A, and m ways of choosing B, then there are n * m ways of choosing AB

Ex: How many different ways can I customize my phone? Assume there are 6 different storage options, 8 different colors, and 2 different firmware's I can choose from.
- 96 different options  

#### Factorials
Factorials are denoted by n!: n * (n-1) * (n-2)... ...2, 1

Special Rule with 0 Factorial: 0! = 1

### Introduction to Permutations
Permutations : All possible arrangements of a collection of things, where order is important

#### Two Types of Permutations
- Permutations with Repetition : Permutations where repeating numbers/objects is allowed
  * Ex: Combination lock where a combination of "1,1,1,1" would work

- Permutations without Repetition : Permutations where repeating numbers/objects is not allowed
  * People running a race; one person cannot be first and second

#### Calculating Permutations

##### Permutations with Repetition
- If something has n choices and we can choose any of them every time, so we have n choices each time.
- General formula: If we are choosing r of something that has n different possibilities, we will multiply n by itself r times, or n<sup>r</sup>
  * Ex: Consider a phone password where you choose 4 digits. Determine how many passcodes are possible.  
    - 10<sup>4</sup> 

##### Permutations without Repetition
- If something has n choices, we must reduce the number of available choices each time.
- General formula: Assume n is the number of things to choose from and we are choosing r of them, no repetitions, order matters. 
  * n!/(n-r)! = P(n,r) 
- Ex:  Consider a race with 10 runners. Determine how many different top 3 finish orders are possible 
  * 720 ways

### Introduction to Combinations
Combinations: All possible arrangements of things, where order doesn't matter

#### Two Types of Combinations
- Combinations with Repetition : Combinations where repeating numbers/objects is allowed
  * Ex: Could be ice cream scoops, 3 scoops are available in each cone but you could have 2 or more of one flavor

- Combinations without Repetition : Combinations where repeating numbers/objects is not allowed
  * The lottery, numbers are drawn one at a time, and if we have the numbers we win no matter what order they are in

#### Calculating Combinations

##### Combinations with Repetition
