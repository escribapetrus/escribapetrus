---
title: "Logic"
author: "P. Schreiber"
date: "2024-05-30"
---

# Logic

## Where to start

### Fundamental Topics of Logic

- Propositional Logic (Sentential Logic)
- Predicate Logic (First-Order Logic)
- Modal Logic
- Set Theory
- Proof Theory
- Model Theory
- Philosophical Logic

### Main Modes or Schools of Logic

- Classical Logic: Standard logic based on bivalence 
(every proposition is either true or false)
- Intuitionistic Logic: Logic that emphasizes constructive proofs and rejects 
the law of excluded middle
- Modal Logic: Logic dealing with necessity and possibility
- Non-Classical Logics: Includes fuzzy logic, relevance logic, paraconsistent logic, etc.
- Formal Logic: Focus on formal systems and symbolic representations
- Mathematical Logic: Applications of logic in mathematics, including set theory, model theory, proof theory, and recursion theory
 Philosophical Logic: Focus on issues in the philosophy of logic, including the nature and scope of logical systems

### References for the Study of Logic

- "Introduction to Logic" by Irving M. Copi and Carl Cohen: A comprehensive introductory textbook.
- "A Concise Introduction to Logic" by Patrick J. Hurley: Another popular textbook for beginners.
- "Logic, Language, and Meaning" by L.T.F. Gamut: A two-volume set that provides an in-depth introduction to logic from a linguistic perspective.
- "Modal Logic" by Brian F. Chellas: An authoritative text on modal logic.
- "Set Theory and Its Philosophy" by Michael Potter: A philosophical introduction to set theory.
- "Proofs and Types" by Jean-Yves Girard: A study on proof theory and type theory.
-  Stanford Encyclopedia of Philosophy (SEP): Offers detailed articles on various topics in logic.
- Internet Encyclopedia of Philosophy (IEP): Provides accessible articles on many areas of logic.

# Introduction to Propositional Logic

## What is Propositional Logic?

Propositional logic, also known as sentential logic or Boolean logic, is a branch of logic that deals with propositions (statements that can either be true or false) and their relationships through logical connectives. It is the simplest form of logic and serves as the foundation for more complex logical systems.

## Key Concepts in Propositional Logic

### Propositions
A proposition is a statement that can be either true or false, but not both.
Examples: 
- "It is raining"
- "2 + 2 = 4"
- "The sky is green"

### Truth Values
Each proposition has a truth value: true (T) or false (F).

### Logical Connectives
- **AND ($\land$):** The conjunction of two propositions $P \land Q$ is true if both $P$ and $Q$ are true.
- **OR ($\lor$):** The disjunction of two propositions $P \lor Q$ is true if at least one of $P$ or $Q$ is true.
- **NOT ($\neg$):** The negation of a proposition $\neg P$ is true if $P$ is false.
- **IMPLIES ($\rightarrow$):** The implication $P \rightarrow Q$ is true if whenever $P$ is true, $Q$ is also true.
- **IF AND ONLY IF ($\leftrightarrow$):** The biconditional $P \leftrightarrow Q$ is true if $P$ and $Q$ are either both true or both false.

### Truth Tables
A truth table is a tabular representation of all possible truth values of propositions and their combinations using logical connectives.

Example: Truth table for $P \land Q$

| $P$ | $Q$ | $P \land Q$ |
|:---:|:---:|:-----------:|
|  T  |  T  |      T      |
|  T  |  F  |      F      |
|  F  |  T  |      F      |
|  F  |  F  |      F      |

### Logical Equivalence
Two propositions are logically equivalent if they have the same truth value in every possible scenario.
Denoted as $P \equiv Q$.

### Tautologies, Contradictions, and Contingencies
- **Tautology:** A proposition that is always true.
- **Contradiction:** A proposition that is always false.
- **Contingency:** A proposition that is sometimes true and sometimes false.

These three concepts classify propositions based on their truth values across all possible scenarios.

#### Tautologies

A **tautology** is a proposition that is always true, regardless of the truth values of its constituent propositions. In other words, a tautology is true in every possible interpretation.

- **Example:** The proposition $P \lor \neg P$ (P or not P) is a tautology because it is always true whether $P$ is true or false.

  - Truth table for $P \lor \neg P$:

| $P$ | $\neg P$ | $P \lor \neg P$ |
|:---:|:--------:|:---------------:|
|  T  |    F     |       T         |
|  F  |    T     |       T         |

#### Contradictions

A **contradiction** is a proposition that is always false, regardless of the truth values of its constituent propositions. A contradiction is false in every possible interpretation.

- **Example:** The proposition $P \land \neg P$ (P and not P) is a contradiction because it is always false whether $P$ is true or false.

  - Truth table for $P \land \neg P$:

| $P$ | $\neg P$ | $P \land \neg P$ |
|:---:|:--------:|:----------------:|
|  T  |    F     |        F         |
|  F  |    T     |        F         |

#### Contingencies

A **contingency** is a proposition that is neither always true nor always false. In other words, a contingency is true in some interpretations and false in others.

- **Example:** The proposition $P \land Q$ (P and Q) is a contingency because its truth value depends on the truth values of $P$ and $Q$.

  - Truth table for $P \land Q$:

| $P$ | $Q$ | $P \land Q$ |
|:---:|:---:|:-----------:|
|  T  |  T  |      T      |
|  T  |  F  |      F      |
|  F  |  T  |      F      |
|  F  |  F  |      F      |

## Further Examples and Exercises

1. **Identifying Tautologies:**
   - Determine if the following propositions are tautologies:
     - $P \lor \neg P$
     - $(P \rightarrow Q) \lor (\neg P)$
     - $(P \land Q) \rightarrow P$

2. **Identifying Contradictions:**
   - Determine if the following propositions are contradictions:
     - $P \land \neg P$
     - $(P \rightarrow Q) \land (P \land \neg Q)$
     - $\neg(P \lor P)$

3. **Identifying Contingencies:**
   - Determine if the following propositions are contingencies:
     - $P \land Q$
     - $P \lor Q$
     - $P \rightarrow Q$

4. **Truth Table Practice:**
   - Create truth tables for the following propositions and classify them as tautologies, contradictions, or contingencies:
     - $(P \rightarrow Q) \leftrightarrow (\neg P \lor Q)$
     - $\neg(P \land Q) \leftrightarrow (\neg P \lor \neg Q)$
     - $(P \leftrightarrow Q) \leftrightarrow ((P \rightarrow Q) \land (Q \rightarrow P))$

### Formal Proofs
Methods to show that a given proposition logically follows from a set of premises.
Common techniques include direct proof, proof by contrapositive, and proof by contradiction.

#### 1. **Direct Proof:**

   - **Description:** A direct proof demonstrates that a conclusion follows logically from its premises without assuming the opposite (negation) of the conclusion.
   - **Example:** To prove $P \rightarrow Q$, assume $P$ is true, and then show that $Q$ must also be true based on the premises and logical rules.

#### 2. **Proof by Contrapositive:**

   - **Description:** Proof by contrapositive establishes the validity of $P \rightarrow Q$ by showing $\neg Q \rightarrow \neg P$. It demonstrates that if $Q$ is false, then $P$ must also be false.
   - **Example:** To prove $P \rightarrow Q$, assume $\neg Q$ is true, and then show that $\neg P$ must follow logically.

#### 3. **Proof by Contradiction (Reductio ad Absurdum):**

   - **Description:** Proof by contradiction assumes the negation of the proposition to be proved and then derives a contradiction from this assumption. This contradiction demonstrates that the original proposition must be true.
   - **Example:** To prove $P$, assume $\neg P$ and derive a contradiction using logical rules or premises, thereby showing that $\neg P$ leads to an impossible or contradictory situation.

### Steps in Formal Proofs

1. **State the Premises:** Begin by clearly stating the premises or assumptions from which the proof will proceed.
   
2. **State the Conclusion:** Clearly state the proposition or conclusion that you intend to prove.

3. **Outline the Proof Strategy:** Choose an appropriate method (direct proof, proof by contrapositive, or proof by contradiction) based on the nature of the proposition and premises.

4. **Execute the Proof:**
   - For **Direct Proof:** Use logical inference rules to connect the premises to the conclusion step-by-step.
   - For **Proof by Contrapositive:** Assume the negation of the conclusion and derive the negation of the premise.
   - For **Proof by Contradiction:** Assume the negation of the proposition and derive a contradiction.

5. **Conclusion:** Summarize the proof and conclude that the proposition is logically derived from the premises using the chosen method.

### Example Formal Proof

#### Proposition:
Prove that if $n$ is an even integer, then $n^2$ is also an even integer.

#### Proof Outline:
- **Premise:** Let $n$ be an even integer.
- **Conclusion:** Show that $n^2$ is an even integer.
- **Method:** Direct proof.

#### Proof:
Assume $n$ is an even integer, so $n = 2k$ for some integer $k$.
\[ n^2 = (2k)^2 = 4k^2 \]
Since $k$ is an integer, $4k^2$ is divisible by 2 (specifically, $4k^2 = 2(2k^2)$).
Therefore, $n^2$ is an even integer.
Hence, if $n$ is an even integer, then $n^2$ is also an even integer.

### Further Reading and Practice

- For more detailed explanations and examples of formal proofs, refer to textbooks such as:
  - "Mathematical Proofs: A Transition to Advanced Mathematics" by Chartrand, Polimeni, and Zhang.
  - "Discrete Mathematics and Its Applications" by Kenneth H. Rosen.

## Basic Logical Laws

- **Identity Law:**
  - $P \land T \equiv P$
  - $P \lor F \equiv P$
- **Domination Law:**
  - $P \lor T \equiv T$
  - $P \land F \equiv F$
- **Idempotent Law:**
  - $P \lor P \equiv P$
  - $P \land P \equiv P$
- **Double Negation Law:**
  - $\neg(\neg P) \equiv P$
- **Commutative Law:**
  - $P \lor Q \equiv Q \lor P$
  - $P \land Q \equiv Q \land P$
- **Associative Law:**
  - $(P \lor Q) \lor R \equiv P \lor (Q \lor R)$
  - $(P \land Q) \land R \equiv P \land (Q \land R)$
- **Distributive Law:**
  - $P \lor (Q \land R) \equiv (P \lor Q) \land (P \lor R)$
  - $P \land (Q \lor R) \equiv (P \land Q) \land (P \land R)$
- **De Morgan's Laws:**
  - $\neg(P \lor Q) \equiv \neg P \land \neg Q$
  - $\neg(P \land Q) \equiv \neg P \lor \neg Q$

## Suggested Exercises

### Constructing Truth Tables
Create truth tables for the following expressions:
- $P \lor Q$
- $P \land \neg Q$
- $\neg (P \lor Q)$
- $P \rightarrow Q$
- $P \leftrightarrow Q$

### Identifying Logical Equivalence
Determine if the following pairs of propositions are logically equivalent:
- $P \land Q$ and $Q \land P$
- $\neg (P \lor Q)$ and $\neg P \land \neg Q$
- $P \rightarrow Q$ and $\neg P \lor Q$

### Proving Logical Statements
Prove that $P \rightarrow Q$ is logically equivalent to $\neg Q \rightarrow \neg P$.


