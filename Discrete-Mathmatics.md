# Discrete Mathmatics

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
- Conneectives are used for making compound propositions

| Name | Represented | Meaning |
| Negation | ¬p | "not p" |
| Conjuction | p ^ q | "p and q" |
| Disjunction | p ∨ q | "p or q" |
| Exclusive Or | p ⊕ q | "p or q, but not both" |
| Implication | p ⇒ q| "if p then q" | 
| Biconditional | p ⇔ q| "p if and only if q" |

### Truth Tables
- Used to show all possible combinations of statements and connectives along with their truth values.

#### Negation Example

| p | ¬p |
| T | F |
| F | T |

#### Conjuction Example (^, "and")

| p | q | p ^ q |
| T | F | F | 
| T | T | T |
| F | T | F |
| F | F | F |

#### Disjunction Example (∨, "or")

| p | q | p ∨ q |
| T | F | T | 
| T | T | T |
| F | T | T |
| F | F | F |

#### Exclusive Or Example (⊕, "xor")

| p | q | p ⊕ q |
| T | F | T | 
| T | T | F |
| F | T | T |
| F | F | F |

#### Implication Example (⇒, "if p then q")

| p | q | p ⇒ q |
| T | F | F | 
| T | T | T |
| F | T | T |
| F | F | T |

#### Biconditional Example (⇔, "p if and only if q")

| p | q | p ⇔ q |
| T | F | F | 
| T | T | T |
| F | T | F |
| F | F | T |

### Proofs Using Truth Tables
- Formulas p and q are logically equivalent if and only if the truth conditions of p are the same as the truth conditions of q

#### Example
Show that ¬(p ∨ q) ≡ ¬p ^ ¬q

| p | q | ¬p | ¬q | p ∨ q | ¬(p ∨ q) | ¬p ^ ¬q
| T | T | F | F | T | F | F |
| T | F | F | T | T | F | F |
| F | T | T | F | T | F | F |
| F | F | T | T | F | T | F |

The last two columns are equivalent, therefore ¬(p ∨ q) ≡ ¬p ^ ¬q

#### Definitions
Tautology: A statment that always produces truth

Contradiction: A stament that always produces false

### Basic Laws of Logic
Assume T is a tautology and F is a contradiction

#### Double Negation Law
- ¬¬p ⇔ p

#### Identity Laws:
- p ^ T ⇔ p
- p ∨ F ⇔ p

#### Domination Laws:
- p ∨ T ⇔ T
- p ^ F ⇔ F

#### DeMorgan's Laws
- ¬(p ^ q) ⇔ ¬p ∨ ¬q
- ¬(p ∨ q) ⇔ ¬p ^ ¬q 

### Advanced Laws of Logic
Assume T is a tautology and F is a contradiction

#### Distibutive Law:
- p ^ (q ∨ r) ⇔ (p ^ q) ∨ (p ^ r)
- p ∨ (q ^ r) ⇔ (p ∨ q) ^ (p ∨ r)

#### Absorption Laws:
- p ^ (p ∨ q) ⇔ p
- p ∨ (p ^ q) ⇔ p