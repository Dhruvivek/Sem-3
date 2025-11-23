# Lecture Transcript: Introduction to Artificial Intelligence with Python

## 1. Introduction and Recap

[MUSIC PLAYING]

- Welcome to the lecture on Artificial Intelligence with Python.
- Recap of previous lecture on search problems:
    - AI agents solving problems by taking actions in an environment.
    - Examples: playing moves in a game or determining driving directions.

## 2. Knowledge and Reasoning

- Focus on the concept of knowledge as a basis for intelligence.
    - Human intelligence relies on knowing facts about the world.
    - Using known information to draw conclusions or reason about new information.
- Objective: Apply knowledge and reasoning to build knowledge-based AI agents.
    - Agents represent knowledge internally and use algorithms to solve problems or derive new information.

## 3. Logical Reasoning Example: Harry Potter Scenario

- Example using Harry Potter facts to illustrate reasoning:
    - Fact 1: If it didn't rain, then Harry visited Hagrid today.
    - Fact 2: Harry visited Hagrid or Dumbledore today, but not both.
    - Fact 3: Harry visited Dumbledore today.
- Reasoning process:
    - From Fact 2 and Fact 3: Harry did not visit Hagrid (since he visited Dumbledore, and it’s one or the other).
    - From Fact 1 and the conclusion that Harry did not visit Hagrid: It must have rained today.
- This logical reasoning uses known facts to deduce new information.

## 4. Formalizing Logic for AI

- Need for formal representation of logic in computers:
    - Human reasoning uses natural language (e.g., English).
    - Computers require a structured knowledge representation language.
- Introduction to **propositional logic**:
    - Based on propositions (statements about the world).
    - Uses **propositional symbols** (e.g., P, Q, R) to represent facts.
        - Example: P = "It is raining," Q = "Harry visited Hagrid."
- **Logical connectives** to combine propositions:
    - **Not (¬)**: Inverts truth value (e.g., ¬P means "It is not raining").
    - **And (∧)**: True if both operands are true (e.g., P ∧ Q).
    - **Or (∨)**: True if at least one operand is true (e.g., P ∨ Q).
    - **Implication (→)**: P → Q means if P is true, then Q is true.
    - **Biconditional (↔)**: P ↔ Q means P is true if and only if Q is true.

## 5. Truth Tables for Logical Connectives

- **Not (¬)**:
    - Truth table: If P is false, ¬P is true; if P is true, ¬P is false.
- **And (∧)**:
    - Truth table: P ∧ Q is true only when both P and Q are true.
- **Or (∨)**:
    - Truth table: P ∨ Q is true if either P or Q (or both) is true.
    - Note: This is inclusive or (not exclusive).
- **Implication (→)**:
    - Truth table: P → Q is false only when P is true and Q is false.
    - If P is false, P → Q is true regardless of Q’s truth value.
- **Biconditional (↔)**:
    - Truth table: P ↔ Q is true when P and Q have the same truth value.

## 6. Knowledge Representation and Models

- **Sentence**: An assertion about the world in a knowledge representation language.
- **Model**: Assigns a truth value (true or false) to every propositional symbol, representing a possible world.
    - Example: For P = "It is raining" and Q = "It is Tuesday," a model might assign P = true, Q = false.
    - Number of possible models: 2^n for n propositional symbols.
- **Knowledge Base (KB)**: A set of sentences known to be true, stored by the AI to reason about the world.

## 7. Entailment and Inference

- **Entailment (⊨)**: Alpha ⊨ Beta means in every model where alpha is true, beta is also true.
    - Example: If KB contains "If it didn’t rain, Harry visited Hagrid," "Harry visited Hagrid or Dumbledore but not both," and "Harry visited Dumbledore," it entails:
        - Harry did not visit Hagrid.
        - It rained today.
- **Inference**: The process of deriving new sentences from existing ones in the knowledge base.
    - Goal: Use inference algorithms to determine if KB ⊨ alpha (does the knowledge base entail a query alpha?).

## 8. Model Checking Algorithm

- **Model Checking**: A method to determine if KB ⊨ alpha.
    - Process:
        1. Enumerate all possible models (all true/false assignments for propositional symbols).
        2. Check if, in every model where KB is true, the query alpha is also true.
    - Example revisited:
        - Symbols: P = "It is Tuesday," Q = "It is raining," R = "Harry will go for a run."
        - KB: (P ∧ ¬Q → R), P, ¬Q.
        - Query: R (Is Harry going for a run?).
        - Result: KB ⊨ R (in the only model where KB is true, R is true).
- Implementation in Python:
    - Uses a logic library with classes for symbols and connectives (e.g., `Not`, `And`, `Or`, `Implication`).
    - Example code (`Harry.py`):
        - Defines symbols: `rain`, `Hagrid`, `Dumbledore`.
        - Encodes KB: (¬rain → Hagrid), (Hagrid ∨ Dumbledore), ¬(Hagrid ∧ Dumbledore), Dumbledore.
        - Uses `model_check(KB, rain)` to confirm it rained.

## 9. Knowledge Engineering: Applying Logic to Problems

- **Knowledge Engineering**: Translating real-world problems into logical representations for AI to solve.
- Example 1: **Clue Game**:
    - Symbols: One for each person (Mustard, Plum, Scarlet), room (Ballroom, Kitchen, Library), weapon (Knife, Revolver, Wrench).
    - KB:
        - One person is the murderer: Mustard ∨ Plum ∨ Scarlet.
        - One room is the crime scene: Ballroom ∨ Kitchen ∨ Library.
        - One weapon was used: Knife ∨ Revolver ∨ Wrench.
        - Additional clues (e.g., ¬Mustard, ¬Kitchen, ¬Revolver).
        - Clue revealed: ¬Scarlet ∨ ¬Library ∨ ¬Wrench.
    - Code (`clue.py`): Uses model checking to deduce which cards are in the envelope.
- Example 2: **Hogwarts Logic Puzzle**:
    - Symbols: One for each person-house combination (e.g., Gilderoy_Gryffindor, Pomona_Slytherin).
    - KB:
        - Each person in one house: Gilderoy_Gryffindor ∨ Gilderoy_Hufflepuff ∨ ...
        - No person in multiple houses: Gilderoy_Gryffindor → ¬Gilderoy_Hufflepuff.
        - Each house has one person: Pomona_Hufflepuff → ¬Minerva_Hufflepuff.
        - Clues: Gilderoy_Gryffindor ∨ Gilderoy_Ravenclaw, ¬Pomona_Slytherin, Minerva_Gryffindor.
    - Code (`puzzle.py`): Solves to assign Gilderoy to Ravenclaw, Pomona to Hufflepuff, Minerva to Gryffindor, Horace to Slytherin.
- Example 3: **Mastermind**:
    - Symbols: One for each color-position combination.
    - KB: Encodes guesses and feedback (e.g., two colors correct in one guess, none in another).
    - Code (`mastermind.py`): Deduces color order (e.g., red, blue, yellow, green).

## 10. Limitations of Model Checking

- Model checking is computationally expensive:
    - For n propositional symbols, it evaluates 2^n possible models.
    - Inefficient for large datasets or complex problems.

## 11. Inference Rules

- **Inference Rules**: Rules to derive new knowledge from existing knowledge without enumerating all models.
    - Structure: Premises above a line, conclusion below.
- **Modus Ponens**:
    - Premise: Alpha → Beta, Alpha.
    - Conclusion: Beta.
    - Example: If raining → Harry inside, raining → Harry inside.
- **And Elimination**:
    - Premise: Alpha ∧ Beta.
    - Conclusion: Alpha (or Beta).
    - Example: Harry friends with Ron ∧ Hermione → Harry friends with Hermione.
- **Double Negation Elimination**:
    - Premise: ¬¬Alpha.
    - Conclusion: Alpha.
    - Example: ¬(Harry did not pass) → Harry passed.
- **Implication Elimination**:
    - Premise: Alpha → Beta.
    - Conclusion: ¬Alpha ∨ Beta.
    - Example: Raining → Harry inside → ¬raining ∨ Harry inside.
- **Biconditional Elimination**:
    - Premise: Alpha ↔ Beta.
    - Conclusion: (Alpha → Beta) ∧ (Beta → Alpha).
    - Example: Raining ↔ Harry inside → (raining → Harry inside) ∧ (Harry inside → raining).
- **De Morgan’s Laws**:
    - ¬(Alpha ∧ Beta) → ¬Alpha ∨ ¬Beta.
        - Example: ¬(Harry ∧ Ron passed) → ¬Harry passed ∨ ¬Ron passed.
    - ¬(Alpha ∨ Beta) → ¬Alpha ∧ ¬Beta.
        - Example: ¬(Harry ∨ Ron passed) → ¬Harry passed ∧ ¬Ron passed.
- **Distributive Law** (partial):
    - Premise: Alpha ∧ (Beta ∨ Gamma).
    - Conclusion: (Alpha ∧ Beta) ∨ (Alpha ∧ Gamma).

## 12. Conclusion

- Propositional logic enables AI to reason logically using knowledge bases and inference.
- Model checking is a straightforward but computationally intensive method.
- Inference rules offer a more efficient way to derive conclusions.
- Knowledge engineering allows real-world problems (e.g., Clue, Hogwarts puzzle, Mastermind) to be solved using logical AI systems.