# Addition Law Of Probability

The Addition Law of Probability (also known as the General Addition Rule) is used to find the probability of the union of two or more events.

## Formula for Probability of $A$ Union $B$

The probability of event $A$ **or** event $B$ happening, denoted $P(A \cup B)$, is the sum of their individual probabilities minus the probability of their intersection. We subtract the intersection to avoid double-counting the outcomes that are common to both $A$ and $B$.

$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

## Formula for Probability of $A$ Intersection $B$

While the Addition Law primarily calculates the union, the formula can be rearranged to find the probability of the intersection, $P(A \cap B)$:

$$P(A \cap B) = P(A) + P(B) - P(A \cup B)$$

---

## Special Case: Mutually Exclusive Events (Disjoint Events)

If $A$ and $B$ are **mutually exclusive** (disjoint) events, they cannot happen at the same time. This means their intersection is the impossible event ($\emptyset$), and its probability is zero.

* $A \cap B = \emptyset$
* $P(A \cap B) = 0$

In this case, the Addition Law simplifies to:
$$P(A \cup B) = P(A) + P(B)$$

---

## Addition Law for Three Events

If $A$, $B$, and $C$ are any three events, the formula for the probability of their union is:

$$P(A \cup B \cup C) = P(A) + P(B) + P(C) - P(A \cap B) - P(A \cap C) - P(B \cap C) + P(A \cap B \cap C)$$

---

## Addition Law for $n$ Mutually Exclusive Events

If $A_1, A_2, \dots, A_n$ are $n$ **mutually exclusive events**, the probability of the happening of one of them is the sum of their individual probabilities:

$$P(A_1 \cup A_2 \cup \dots \cup A_n) = P(A_1) + P(A_2) + \dots + P(A_n) = \sum_{i=1}^{n} P(A_i)$$

---
## 🎯 Examples

### Example 1: Divisibility by 6 or 8

**Question:** An integer is chosen at random from two hundred digits (assume the integers are $1, 2, \dots, 200$). What is the probability that the integer is divisible by $6$ **or** $8$?

1.  **Total Cases ($n(S)$):** $200$.
2.  **Define Events:**
    * Event $A$: Integer is divisible by $6$.
    * Event $B$: Integer is divisible by $8$.
    * Event $A \cap B$: Integer is divisible by both $6$ and $8$, meaning it's divisible by the **Least Common Multiple (LCM)** of $6$ and $8$, which is $24$.

3.  **Calculate Probabilities:**
    * $n(A) = \lfloor \frac{200}{6} \rfloor = 33 \quad \implies P(A) = \frac{33}{200}$
    * $n(B) = \lfloor \frac{200}{8} \rfloor = 25 \quad \implies P(B) = \frac{25}{200}$
    * $n(A \cap B) = \lfloor \frac{200}{24} \rfloor = 8 \quad \implies P(A \cap B) = \frac{8}{200}$

4.  **Apply Addition Law:**
    $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
    $$P(A \cup B) = \frac{33}{200} + \frac{25}{200} - \frac{8}{200}$$
    $$P(A \cup B) = \frac{33 + 25 - 8}{200} = \frac{50}{200} = \frac{1}{4}$$

---

### Example 2: Student Passing Two Tests

**Question:** $P(\text{Physics}) = 2/3$. $P(\text{Physics} \text{ and } \text{English}) = 14/45$. $P(\text{At least one}) = 4/5$. What is $P(\text{English})$?

1.  **Define Notation:**
    * $P(P) = 2/3$
    * $P(P \cap E) = 14/45$
    * $P(P \cup E) = 4/5$ (since "at least one" means $P$ **or** $E$)
    * $P(E) = ?$

2.  **Apply Addition Law:**
    $$P(P \cup E) = P(P) + P(E) - P(P \cap E)$$

3.  **Substitute known values and solve for $P(E)$:**
    $$\frac{4}{5} = \frac{2}{3} + P(E) - \frac{14}{45}$$
    $$P(E) = \frac{4}{5} - \frac{2}{3} + \frac{14}{45}$$

4.  **Find Common Denominator (45):**
    $$P(E) = \frac{4 \times 9}{45} - \frac{2 \times 15}{45} + \frac{14}{45}$$
    $$P(E) = \frac{36}{45} - \frac{30}{45} + \frac{14}{45}$$
    $$P(E) = \frac{36 - 30 + 14}{45} = \frac{20}{45}$$

5.  **Simplify:**
    $$P(E) = \frac{4}{9}$$

---

### Example 3: Two Dice Tossed

**Question:** Two dice are tossed. Find $P(\text{Even on first die } \textbf{or } \text{Total of 8})$.

1.  **Total Cases ($n(S)$):** $6 \times 6 = 36$.
2.  **Define Events:**
    * Event $A$: Even number on the first die.
    * Event $B$: Total of $8$.

3.  **Identify Outcomes and Probabilities:**
    * $A = \{(2,1), \dots, (2,6), (4,1), \dots, (4,6), (6,1), \dots, (6,6)\}$
        * $n(A) = 3 \times 6 = 18 \quad \implies P(A) = \frac{18}{36} = \frac{1}{2}$
    * $B = \{(2,6), (3,5), (4,4), (5,3), (6,2)\}$
        * $n(B) = 5 \quad \implies P(B) = \frac{5}{36}$
    * $A \cap B$: Outcomes where the first die is even **and** the total is $8$.
        * $A \cap B = \{(2,6), (4,4), (6,2)\}$
        * $n(A \cap B) = 3 \quad \implies P(A \cap B) = \frac{3}{36}$

4.  **Apply Addition Law:**
    $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
    $$P(A \cup B) = \frac{18}{36} + \frac{5}{36} - \frac{3}{36}$$
    $$P(A \cup B) = \frac{18 + 5 - 3}{36} = \frac{20}{36} = \frac{5}{9}$$

---

### Example 4: Horse Race (Mutually Exclusive)

**Question:** $P(A \text{ winning}) = 1/5$ and $P(B \text{ winning}) = 1/6$. What is $P(\text{one of the horse will win})$?

1.  **Identify Relationship:** Since only one horse can win a race, the events are **mutually exclusive** (if A wins, B cannot, and vice versa).
2.  **Apply Simplified Addition Law:**
    $$P(A \cup B) = P(A) + P(B)$$
    $$P(\text{A or B wins}) = \frac{1}{5} + \frac{1}{6}$$

3.  **Calculate:**
    $$P(A \cup B) = \frac{6}{30} + \frac{5}{30} = \frac{11}{30}$$

---

### Example 5: Drawing a Card (Mutually Exclusive)

**Question:** Find $P(\text{King } \textbf{or } \text{Queen})$ from a $52$-card pack.

1.  **Total Cases ($n(S)$):** $52$.
2.  **Define Events:**
    * $A$: Drawing a King ($4$ Kings). $P(A) = 4/52$.
    * $B$: Drawing a Queen ($4$ Queens). $P(B) = 4/52$.
3.  **Identify Relationship:** You cannot draw a card that is both a King and a Queen. The events are **mutually exclusive**.
4.  **Apply Simplified Addition Law:**
    $$P(A \cup B) = P(A) + P(B)$$
    $$P(\text{King or Queen}) = \frac{4}{52} + \frac{4}{52} = \frac{8}{52}$$
5.  **Simplify:**
    $$P(\text{King or Queen}) = \frac{2}{13}$$

---

### Example 6: Odds and Race (Mutually Exclusive)

**Question:** Odds in favour of $A, B, C, D$ winning are $1:3, 1:4, 1:5, 1:6$ respectively. Find the chance that one of them wins the race.

1.  **Convert Odds to Probability:** If the odds in favour are $a:b$, the probability is $a / (a+b)$.
    * $P(A \text{ wins}) = \frac{1}{1+3} = \frac{1}{4}$
    * $P(B \text{ wins}) = \frac{1}{1+4} = \frac{1}{5}$
    * $P(C \text{ wins}) = \frac{1}{1+5} = \frac{1}{6}$
    * $P(D \text{ wins}) = \frac{1}{1+6} = \frac{1}{7}$
2.  **Identify Relationship:** Since a "Dead Head is Impossible," these events are **mutually exclusive**.
3.  **Apply Addition Law for $n$ events:**
    $$P(\text{one wins}) = P(A) + P(B) + P(C) + P(D)$$
    $$P(\text{one wins}) = \frac{1}{4} + \frac{1}{5} + \frac{1}{6} + \frac{1}{7}$$
4.  **Find Common Denominator (LCM of 4, 5, 6, 7 is 420):**
    $$P(\text{one wins}) = \frac{105}{420} + \frac{84}{420} + \frac{70}{420} + \frac{60}{420}$$
    $$P(\text{one wins}) = \frac{105 + 84 + 70 + 60}{420} = \frac{319}{420}$$

---

### Example 7: Drawing a Card (Non-Mutually Exclusive)

**Question:** Find $P(\text{King } \textbf{or } \text{Heart } \textbf{or } \text{Red Card})$ from a pack of $52$ cards.

1.  **Define Events:**
    * $K$: King (4 total)
    * $H$: Heart (13 total)
    * $R$: Red Card (26 total: 13 Hearts + 13 Diamonds)
2.  **Identify Relationships:** These events are NOT mutually exclusive.
    * A King can be a Heart or a Red Card.
    * A Heart is always a Red Card.
3.  **Simplify the Union:** Since all Hearts ($H$) are included in the set of Red Cards ($R$), $H \subset R$. Therefore, the union of $H$ and $R$ is simply $R$:
    $$P(H \cup R) = P(R)$$
    So, the problem simplifies to finding $P(K \cup R)$.

4.  **Identify Intersection $P(K \cap R)$:** The set of cards that are both a King **and** a Red Card.
    * There are $2$ Red Kings (King of Hearts and King of Diamonds).
    * $P(K) = 4/52$
    * $P(R) = 26/52$
    * $P(K \cap R) = 2/52$

5.  **Apply Addition Law for $K \cup R$:**
    $$P(K \cup R) = P(K) + P(R) - P(K \cap R)$$
    $$P(K \cup R) = \frac{4}{52} + \frac{26}{52} - \frac{2}{52}$$
    $$P(K \cup R) = \frac{4 + 26 - 2}{52} = \frac{28}{52}$$

6.  **Simplify:**
    $$P(K \cup R) = \frac{7}{13}$$

---

# Multiplication Law Of Probability

The **Multiplication Law of Probability** is used to find the probability of the **intersection** of two or more events—the chance that all of them occur. The key word you will often see is "**and**."

## Conditional Probability

**Conditional Probability** is the probability of an event occurring given that another event has already occurred. It changes the sample space for the second event.

* The probability of the happening of an event $A$ when another event $B$ has already happened is called Conditional Probability.
* It is denoted by **$P(A|B)$**, read as "the probability of $A$ given $B$."

### The Formula for Conditional Probability

If $P(B) > 0$, the formula is:

$$P(A\mid B) = \frac{P(A \cap B)}{P(B)}$$

This tells you that to find the chance of $A$ happening given $B$ has happened, you look at the outcomes where both $A$ and $B$ occurred and divide by the probability of the *given* event ($B$). Essentially, $B$ becomes the new, reduced sample space.

---

## Multiplication Law Of Probability

The Multiplication Law is derived directly from the Conditional Probability formula by rearranging it to solve for the intersection $P(A \cap B)$.

### For Two Events $A$ and $B$

The probability that $A$ **and** $B$ both occur is:

$$P(A \cap B) = P(A) \times P(B|A)$$

**OR**

$$P(A \cap B) = P(B) \times P(A|B)$$

**Requirement:** For the formula to be valid, the probabilities of the initial events must be greater than zero, i.e., $P(A) > 0$ and $P(B) > 0$.

---

## Special Case: Independent Events

Events $A$ and $B$ are **Independent** if the occurrence of one event does not affect the probability of the other event.

### Independent Event Condition

An event $A$ is said to be independent of another event $B$ if:

$$P(A|B) = P(A)$$

This means the probability of $A$ remains the same, even when $B$ is given. Similarly, for $B$ to be independent of $A$:

$$P(B|A) = P(B)$$

### Multiplication Law for Independent Events

**Note-1:** If $A$ and $B$ are independent, we substitute the condition $P(B|A) = P(B)$ or $P(A|B) = P(A)$ into the general multiplication law:

$$P(A \cap B) = P(A) \times P(B)$$

This simplified formula is used when the events are independent (e.g., flipping two different coins, drawing a card **with replacement**).

### Multiplication Law for $n$ Independent Events

**Note-2:** If $A_1, A_2, \dots, A_n$ are $n$ independent events, then the probability that **all** of them occur is the product of their individual probabilities:

$$P(A_1 \cap A_2 \cap \dots \cap A_n) = P(A_1) \times P(A_2) \times \dots \times P(A_n)$$

---

## Summary of Use

| Situation              | Keyword                                    | Probability to Find   | Formula                    |
| :--------------------- | :----------------------------------------- | :-------------------- | :------------------------- |
| **Dependent Events**   | "and," "followed by" (without replacement) | $P(A \cap B)$         | $P(A) \times P(B\mid A)$   |
| **Independent Events** | "and," (with replacement)                  | $P(A \cap B)$         | $P(A) \times P(B)$         |
| **Conditional**        | "given that," "                            | ", "if",$P(A \mid B)$ | $\frac{P(A \cap B)}{P(B)}$ |

### Example 1: Rolling a Pair of Dice

A pair of dice is rolled. Find $P(A | B)$.

* **Event $A$**: $2$ appears on at least one die.
* **Event $B$**: The sum of the numbers appearing on the dice is $6$.

**Problem:** A pair of dice is rolled. Find $P(A | B)$.
* **Event $A$**: $2$ appears on at least one die.
* **Event $B$**: The sum of the numbers appearing on the dice is $6$.

**Conditional Probability Formula:** $P(A|B) = \frac{P(A \cap B)}{P(B)} = \frac{n(A \cap B)}{n(B)}$

1.  **Sample Space ($S$):** $n(S) = 36$ possible outcomes.
2.  **Identify Event $B$ (The condition):** Sum is $6$.
    $$B = \{(1, 5), (2, 4), (3, 3), (4, 2), (5, 1)\}$$
    $$n(B) = 5$$
3.  **Identify Intersection ($A \cap B$):** Outcomes in $B$ where $2$ appears on at least one die.
    * From set $B$, the outcomes containing a $2$ are: $(2, 4)$ and $(4, 2)$.
    $$A \cap B = \{(2, 4), (4, 2)\}$$
    $$n(A \cap B) = 2$$
4.  **Calculate $P(A|B)$:**
    $$P(A|B) = \frac{n(A \cap B)}{n(B)} = \frac{2}{5}$$

The conditional probability that $2$ appears on at least one die, **given** that the sum is $6$, is $\frac{2}{5}$.

---

### Example 2: City Population Survey

From a city population, the following probabilities are known:
1.  The probability of selecting a **Male or a Smoker** is $\frac{7}{10}$.
2.  The probability of selecting a **Male Smoker** is $\frac{2}{5}$.
3.  The probability of selecting a **Male if a Smoker is already selected** is $\frac{2}{3}$.

**Find the probability of selecting:**
* A Non-Smoker
* A Male
* A Smoker if a Male is first selected

**Problem:** Given the following probabilities for selecting an individual from a city population:
1.  $P(\text{Male or Smoker}) = 7/10 \implies P(M \cup S) = 7/10$
2.  $P(\text{Male Smoker}) = 2/5 \implies P(M \cap S) = 2/5$
3.  $P(\text{Male if Smoker is selected}) = 2/3 \implies P(M|S) = 2/3$

**Find the probability of selecting:**

### 1. A Non-Smoker
We can use the formula for Conditional Probability for $P(M|S)$:
$$P(M|S) = \frac{P(M \cap S)}{P(S)}$$
We know $P(M|S) = 2/3$ and $P(M \cap S) = 2/5$. Substitute and solve for $P(S)$:
$$\frac{2}{3} = \frac{2/5}{P(S)}$$
$$P(S) = \frac{2/5}{2/3} = \frac{2}{5} \times \frac{3}{2} = \frac{3}{5}$$

Now, the probability of selecting a **Non-Smoker ($\overline{S}$)** is the complement of a Smoker:
$$P(\overline{S}) = 1 - P(S) = 1 - \frac{3}{5} = \frac{2}{5}$$

### 2. A Male
We use the **Addition Law of Probability** with the known values:
$$P(M \cup S) = P(M) + P(S) - P(M \cap S)$$
$$\frac{7}{10} = P(M) + \frac{3}{5} - \frac{2}{5}$$
$$\frac{7}{10} = P(M) + \frac{1}{5}$$
$$P(M) = \frac{7}{10} - \frac{1}{5} = \frac{7}{10} - \frac{2}{10} = \frac{5}{10} = \frac{1}{2}$$

### 3. A Smoker if Male is first selected ($P(S|M)$)
We use the formula for Conditional Probability:
$$P(S|M) = \frac{P(S \cap M)}{P(M)}$$
Since $P(S \cap M) = P(M \cap S) = 2/5$ and $P(M) = 1/2$:
$$P(S|M) = \frac{2/5}{1/2} = \frac{2}{5} \times 2 = \frac{4}{5}$$

---


### Example 3: Drawing Cards Without Replacement

A card is drawn from a well-shuffled deck of $52$ cards, and then a second card is drawn. Find the probability that the first card is a Spade **and** the second card is a Club, if the first card is **not replaced**.

**Problem:** A card is drawn from a $52$-card deck and the second card is drawn **without replacement**. Find $P(\text{1st is Spade} \text{ and } \text{2nd is Club})$.

1.  **Define Events:**
    * $A$: First card is a Spade.
    * $B$: Second card is a Club.
2.  **Identify Relationship:** Since the first card is **not replaced**, the two events are **dependent**. We use the Multiplication Law: $P(A \cap B) = P(A) \times P(B|A)$.

3.  **Calculate $P(A)$:**
    * There are $13$ Spades in $52$ cards.
    $$P(A) = \frac{13}{52} = \frac{1}{4}$$

4.  **Calculate $P(B|A)$:**
    * The first card drawn ($A$) was a Spade and was **not replaced**.
    * Now there are $51$ cards left.
    * The number of Clubs is still $13$ (since the first card was a Spade).
    $$P(B|A) = \frac{\text{Number of Clubs left}}{\text{Total cards left}} = \frac{13}{51}$$

5.  **Calculate $P(A \cap B)$:**
    $$P(A \cap B) = P(A) \times P(B|A) = \frac{13}{52} \times \frac{13}{51}$$
    $$P(A \cap B) = \frac{1}{4} \times \frac{13}{51} = \frac{13}{204}$$

---


### Example 4: Student Passing Tests

The probability that a student selected at random from a class will pass in Mathematics is $\frac{4}{5}$ and the probability that he/she passes in Mathematics and Computer Science is $\frac{1}{2}$. What is the probability that he/she will pass in Computer Science, if it is known that he has passed in Mathematics?


**Problem:**
* $P(\text{Pass in Maths}) = P(M) = 4/5$
* $P(\text{Pass in Maths and Comp Sci}) = P(M \cap C) = 1/2$
* Find $P(\text{Pass in Comp Sci} \mid \text{Pass in Maths})$ or $P(C|M)$.

1.  **Identify Formula:** This is a direct application of the Conditional Probability formula.
    $$P(C|M) = \frac{P(C \cap M)}{P(M)}$$
    (Note: $P(C \cap M) = P(M \cap C)$)

2.  **Substitute and Solve:**
    $$P(C|M) = \frac{1/2}{4/5}$$
    $$P(C|M) = \frac{1}{2} \times \frac{5}{4} = \frac{5}{8}$$

The probability that the student passes in Computer Science, **given** that they have already passed in Mathematics, is $\frac{5}{8}$.

---

### Example 5: Dice Sum Conditional Probability

A die is thrown twice and the sum of the numbers appearing is observed to be $6$. What is the conditional probability that the number $4$ has appeared at least once?

**Problem:** A dice is thrown twice. The sum is observed to be $6$. What is the conditional probability that the number $4$ has appeared at least once?

1.  **Define Events:**
    * **Event $A$**: $4$ has appeared at least once.
    * **Event $B$**: The sum of the numbers is $6$.

2.  **Identify Event $B$ (The condition):** Sum is $6$.
    $$B = \{(1, 5), (2, 4), (3, 3), (4, 2), (5, 1)\}$$
    $$n(B) = 5$$

3.  **Identify Intersection ($A \cap B$):** Outcomes in $B$ where $4$ appears at least once.
    * The outcomes containing a $4$ are: $(2, 4)$ and $(4, 2)$.
    $$A \cap B = \{(2, 4), (4, 2)\}$$
    $$n(A \cap B) = 2$$

4.  **Calculate $P(A|B)$:**
    $$P(A|B) = \frac{n(A \cap B)}{n(B)} = \frac{2}{5}$$

The conditional probability that $4$ appeared at least once, **given** that the sum is $6$, is $\frac{2}{5}$.