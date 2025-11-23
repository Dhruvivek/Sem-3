# Introduction To Probability

**Probability** is a branch of mathematics that deals with quantifying uncertainty. It provides a numerical measure of how likely an event is to occur.

  * The probability of an event is always a number between **0 and 1**, inclusive.
      * A probability of **0** means the event is **impossible**.
      * A probability of **1** means the event is **certain** to happen.
      * A probability of **0.5 (or 50%)** means the event is **equally likely** to happen or not happen.

-----

# Definition Of A Random Variable

A **Random Variable** is a function that assigns a unique numerical value to each possible outcome of a random experiment. In simpler terms, it is a way of translating the non-numerical (or numerical) results of a random event into a specific, quantifiable number that we can work with mathematically. Random variables are typically denoted by capital letters, like $X$ or $Y$.

## Example

Consider the experiment of **tossing a coin twice**. The possible outcomes are: (Head, Head), (Head, Tail), (Tail, Head), and (Tail, Tail).

Now, let $X$ be the **Random Variable** representing the **number of Heads** obtained.

  * For the outcome (H, H), $X$ assigns the value **2**.
  * For the outcome (H, T), $X$ assigns the value **1**.
  * For the outcome (T, H), $X$ assigns the value **1**.
  * For the outcome (T, T), $X$ assigns the value **0**.

The possible values for the random variable $X$ are $\{0, 1, 2\}$.

## Outcome

An **outcome** is the result of a single execution of an experiment. For example, when you toss a single coin, the possible outcomes are *Head* or *Tail*.

## Trial and Event

When an experiment is repeated under the same conditions, it results in any one of the several possible outcomes.

  * **Experiment is called Trial**: The act of performing the experiment is called a **Trial**.
      * *Ex 1:* **Tossing A Coin** $\rightarrow$ Trial
      * *Ex 2:* **Throwing A Die** $\rightarrow$ Trial
  * **Possible Outcomes is called Event / Cases**: An **Event** (or a Case) is a subset of the possible outcomes. It is a specific outcome or a collection of outcomes that we are interested in.
      * *Ex 1:* The turning up of head or tail (or just getting a **Head**) $\rightarrow$ Event
      * *Ex 2:* Getting $1$ or $2$ or $3$ or $4$ or $5$ or $6$ (or just getting an **odd number**) $\rightarrow$ Event/Cases.

### Simple and Compound/Composite Event

An **Event** is a subset of the Sample Space.

  * **Simple Event**: An event is called **Simple** if it corresponds to a **single possible outcome** of the experiment.
      * *Ex:* In throwing a single die, the event of getting a **5** is a simple event.
  * **Compound or Composite Event**: An event is called **Compound** or **Composite** if it corresponds to **more than one possible outcome** of the experiment.
      * *Ex:* In throwing a single die, the event of getting an **even number** ($\{2, 4, 6\}$) is a composite event.

### Sample Point and Sample Space

  * **Sample Point**: The **outcome** of the random experiment is called a **sample point**. Each individual result is a sample point.
  * **Sample Space**: The **Set of all possible outcomes** of a random experiment is called a **Sample Space**.
      * A Sample Space is denoted by $S$.
      * Every element of the sample space is a sample point.

*Example-1:*

  * If A Coin Is Tossed:
      * The Possible Outcomes are Head ($H$) and Tail ($T$).
      * Sample Space is $S = \{H, T\}$.
      * $H$ is a sample point, and $T$ is a sample point.
  * In Throwing A Die:
      * The Possible Outcomes are $1, 2, 3, 4, 5,$ or $6$.
      * Sample Space is $S = \{1, 2, 3, 4, 5, 6\}$.

## Mutual Exclusive Events Or Mutually Disjoint Event

Two Events $A$ and $B$ are said to be **mutually exclusive** or **mutually disjoint** if they **cannot happen at the same time** in a single trial. They have no sample point in common.

  * Mathematically, this means the **intersection** of the two events is the **empty set (Null)**:
    $$A \cap B = \emptyset$$

  * *Example 1:* In Throwing A Die, $S = \{1, 2, 3, 4, 5, 6\}$

      * Event $A = \{2\}$ (Getting a $2$)
      * Event $B = \{5\}$ (Getting a $5$)
      * $A$ and $B$ are mutually disjoint events because $A \cap B = \emptyset$. You cannot roll both a $2$ and a $5$ at the same time.

  * *Example 2:* Tossing A Coin, $S = \{H, T\}$

      * Event $A = \{H\}$
      * Event $B = \{T\}$
      * $A$ and $B$ are mutually disjoint events.

## Independent Or Dependent Events

This concept applies when we consider the occurrence of two or more events, often in separate trials or draws.

  * **Independent Events**: Two events are **Independent** if the happening (or non-happening) of one event **does not affect** the probability of the other event happening.
      * *Ex:* Flipping a coin twice. The result of the first flip (Head or Tail) does not influence the result of the second flip.
      * *Ex:* Box with $5$ Balls. You draw the first ball, **replace** it, and then draw a second ball. The probability of the second draw is unaffected by the first.
  * **Dependent Events**: Events are said to be **Dependent** if the happening (or non-happening) of one event **does affect** the probability of the other event happening.
      * *Ex:* Box with $5$ Balls. You draw the first ball, and it is **Not Replaced**. The result of the second draw depends on the result of the first draw because the total number of balls and the number of balls of a certain type have changed.

## Exhaustive Cases Or Exhaustive Events or Total Number Of Possible Cases

The set of all possible outcomes of a random experiment is called the set of **Exhaustive Cases** or **Exhaustive Events**. This is simply the **Sample Space ($S$)**. The **Total Number** of all possible outcomes is the count of the exhaustive cases, which is the total number of elements in the sample space.

  * *Ex 1:* Tossing A Coin $\rightarrow$ Two Exhaustive Cases: $\{H, T\}$. Total number is $2$.
  * *Ex 2:* In Throwing A Die $\rightarrow$ Six exhaustive Cases: $\{1, 2, 3, 4, 5, 6\}$. Total number is $6$.
  * *Ex 3:* In Throwing Of Two Die $\rightarrow$ Total $36$ Exhaustive Cases (e.g., $(1,1), (1,2), \dots, (6,6)$). Total number is $6 \times 6 = 36$.
  * *Ex 4:* In Drawing Two Cards From A Deck Of $52$ Cards $\rightarrow$ The Total number of Exhaustive Cases is the number of ways to choose $2$ cards from $52$, which is $52_{C_2}$ ways (using combinations).

## Favorable Cases Or Favorable Events

**Favorable Cases** (or Favorable Events) are the outcomes of a random experiment that result in the happening of a **specified event**. They are the outcomes that satisfy the condition we are interested in.

  * *Ex:* In throwing a single die, if the event we are interested in is **"getting an even number"** ($A$), then the favorable cases are the outcomes in the set $A = \{2, 4, 6\}$. The number of favorable cases is $3$.

## Mathematical Or Classical Definition Of Probability

The **Mathematical** or **Classical Definition of Probability** is the simplest way to calculate probability, assuming all possible outcomes are equally likely.

The Probability of the happening of an Event $A$, denoted by $P(A)$, is given by the ratio:

$$\text{Probability of Event } A = P(A) = \frac{\text{Number of favourable cases for Event } A}{\text{Total Number Of Possible cases (Exhaustive Cases)}}$$

Or, using the notation from the definitions:
$$P(A) = \frac{\text{Number of elements in Event } A}{\text{Number of elements in Sample Space } S} = \frac{n(A)}{n(S)}$$

  * *Ex:* What is the probability of getting an **even number** when rolling a single die?
      * Total Possible Cases, $n(S) = 6$ ($\{1, 2, 3, 4, 5, 6\}$).
      * Favorable Cases, $n(A) = 3$ ($\{2, 4, 6\}$).
      * $P(\text{Even Number}) = \frac{3}{6} = \frac{1}{2}$.


Here are two examples demonstrating the calculation of the probability of an event using the Classical Definition of Probability:

$$P(A) = \frac{\text{Number of favourable cases for Event } A}{\text{Total Number Of Possible cases (Exhaustive Cases)}} = \frac{n(A)}{n(S)}$$

---

## Example 1: Drawing a Card

**Experiment:** Drawing one card randomly from a standard deck of $52$ playing cards.

**Event $A$:** The card drawn is a **King**.

### Step 1: Determine the Total Number of Possible Cases ($n(S)$)
* The total number of cards in the deck is $52$.
* Therefore, the **Total Number of Possible Cases ($n(S)$)** is **52**.

### Step 2: Determine the Number of Favorable Cases ($n(A)$)
* We are interested in the event of drawing a King.
* A standard deck has $4$ suits (Clubs, Diamonds, Hearts, Spades), and each suit has one King.
* The **Number of Favorable Cases ($n(A)$)** is **4**.

### Step 3: Calculate the Probability $P(A)$
$$P(\text{King}) = \frac{\text{Number of Kings}}{\text{Total Number of Cards}} = \frac{n(A)}{n(S)}$$
$$P(\text{King}) = \frac{4}{52} = \frac{1}{13}$$

---

## Example 2: Tossing Two Coins

**Experiment:** Tossing two fair coins simultaneously.

**Event $B$:** Getting **exactly one Head**.

### Step 1: Determine the Total Number of Possible Cases ($n(S)$)
* The possible outcomes (Sample Space, $S$) when tossing two coins are:
    $$S = \{(H, H), (H, T), (T, H), (T, T)\}$$
* The **Total Number of Possible Cases ($n(S)$)** is **4**.

### Step 2: Determine the Number of Favorable Cases ($n(B)$)
* We are interested in the event of getting exactly one Head.
* The outcomes with exactly one Head are $(H, T)$ and $(T, H)$.
* The **Number of Favorable Cases ($n(B)$)** is **2**.

### Step 3: Calculate the Probability $P(B)$
$$P(\text{Exactly one Head}) = \frac{\text{Number of outcomes with exactly one Head}}{\text{Total Number of outcomes}} = \frac{n(B)}{n(S)}$$
$$P(\text{Exactly one Head}) = \frac{2}{4} = \frac{1}{2}$$

---

That note provides an excellent summary of the core principles of Classical Probability!

Let's formalize the definitions you provided and then work through the three examples.

---

# 📝 Core Principles of Classical Probability

The following definitions arise from your note where an Event $A$ can happen in $m$ ways and fail in $n$ ways, with all $m+n$ ways being equally likely.

## Probability of an Event Happening

* **Total Number of Possible Cases ($n(S)$):** The total number of ways the experiment can result, which is the sum of ways the event can happen ($m$) and fail ($n$).
    $$n(S) = m + n$$
* **Number of Favorable Cases ($n(A)$):** The number of ways the event $A$ can happen.
    $$n(A) = m$$
* **Probability of Happening ($P(A)$):**
    $$P(A) = \frac{\text{Number of ways } A \text{ can happen}}{\text{Total number of possible ways}} = \frac{m}{m+n}$$

---

## Probability of an Event Not Happening (Complementary Event)

* **Event Not Happening ($\overline{A}$):** The event that $A$ does not occur. This is often called the **Complementary Event** of $A$.
* **Number of ways $\overline{A}$ can happen ($n(\overline{A})$):** The number of ways the event $A$ can fail.
    $$n(\overline{A}) = n$$
* **Probability of Not Happening ($P(\overline{A})$):**
    $$P(\overline{A}) = \frac{\text{Number of ways } A \text{ can fail}}{\text{Total number of possible ways}} = \frac{n}{m+n}$$

* **Relationship:** The probability of an event happening plus the probability of it not happening must equal $1$.
    $$P(A) + P(\overline{A}) = 1 \quad \text{or} \quad P(\overline{A}) = 1 - P(A)$$

---

## Range of Probability

* The probability of any event $A$ must be between $0$ and $1$, inclusive.
    $$0 \le P(A) \le 1$$
* **Impossible Event:** An event that can never occur (e.g., rolling a $7$ on a single die). $P(\text{Impossible Event}) = 0$.
* **Certain Event (Sample Space):** The event that the outcome is any element of the sample space (i.e., *something* happens). $P(S) = 1$.

---
## 🎯 Calculation Examples

### Example 1: Probability of 53 Sundays in a Leap Year

**Question:** What is the chance that a leap year, selected at random will contain $53$ Sundays?

1.  **Understand the Leap Year:** A **Leap Year** has $366$ days.
    $$366 \text{ days} = (52 \times 7) \text{ days} + 2 \text{ days} = 52 \text{ full weeks} + 2 \text{ extra days}$$
2.  **Exhaustive Cases ($n(S)$):** The $52$ full weeks guarantee $52$ Sundays. The probability depends only on the $2$ extra days. The possible combinations for these $2$ consecutive days (the sample space $S$) are:
    $$S = \{\text{(Sun, Mon)}, (\text{Mon, Tue}), (\text{Tue, Wed}), (\text{Wed, Thu}), (\text{Thu, Fri}), (\text{Fri, Sat}), (\text{Sat, Sun})\}$$
    The total number of possible outcomes is $n(S) = 7$.
3.  **Favorable Cases ($n(A)$):** We need a $53^{\text{rd}}$ Sunday. This happens if the $2$ extra days include a Sunday. The favorable outcomes are $A$:
    $$A = \{(\text{Sun, Mon}), (\text{Sat, Sun})\}$$
    The number of favorable cases is $n(A) = 2$.
4.  **Probability $P(A)$:**
    $$P(\text{53 Sundays}) = \frac{n(A)}{n(S)} = \frac{2}{7}$$

---

### Example 2: Three Coins Are Tossed

**Question:** Three coins are tossed. Find the probability of getting **at least 2 Heads**.

1.  **Exhaustive Cases ($n(S)$):** Tossing three coins results in $2 \times 2 \times 2 = 8$ possible outcomes (the sample space $S$):
    $$S = \{HHH, HHT, HTH, THH, HTT, THT, TTH, TTT\}$$
    The total number of possible outcomes is $n(S) = 8$.
2.  **Favorable Cases ($n(A)$):** The event $A$ is "getting at least $2$ Heads." This means $2$ Heads **or** $3$ Heads.
    * Outcomes with $2$ Heads: $\{HHT, HTH, THH\}$
    * Outcomes with $3$ Heads: $\{HHH\}$
    * Favorable cases $A = \{HHT, HTH, THH, HHH\}$
    The number of favorable cases is $n(A) = 4$.
3.  **Probability $P(A)$:**
    $$P(\text{At least 2 Heads}) = \frac{n(A)}{n(S)} = \frac{4}{8} = \frac{1}{2}$$

---

### Example 3: Drawing Balls from a Bag (Combinations)

**Question:** A bag contains $7$ White, $6$ Red, and $5$ Black balls. Two balls are drawn at random. Find the probability that they will **both be White**.

1.  **Total Balls:** $7 + 6 + 5 = 18$ balls.

2.  **Exhaustive Cases ($n(S)$):** We are choosing $2$ balls from a total of $18$. The number of ways to choose $2$ items from $18$ is calculated using the combination formula $nC_k = \frac{n!}{k!(n-k)!}$.
    $$n(S) = 18_{C_2} = \frac{18 \times 17}{2 \times 1} = 9 \times 17 = 153$$
    The total number of possible ways to draw $2$ balls is **153**.

3.  **Favorable Cases ($n(A)$):** The event $A$ is that **both** balls drawn are White. We must choose $2$ balls from the $7$ available White balls.
    $$n(A) = 7_{C_2} = \frac{7 \times 6}{2 \times 1} = 21$$
    The number of ways to draw $2$ White balls is **21**.

4.  **Probability $P(A)$:**
    $$P(\text{Both White}) = \frac{\text{Ways to choose 2 White}}{\text{Ways to choose 2 from 18}} = \frac{n(A)}{n(S)}$$
    $$P(\text{Both White}) = \frac{21}{153}$$
    (Both $21$ and $153$ are divisible by $3$)
    $$P(\text{Both White}) = \frac{21 \div 3}{153 \div 3} = \frac{7}{51}$$

