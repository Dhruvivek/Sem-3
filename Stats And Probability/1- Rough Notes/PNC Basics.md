# Permutation vs. Combination: The Core Difference

The difference between Permutation and Combination boils down to **order**.

|**Concept**|**What is it?**|**Does Order Matter?**|**When to Use?**|
|---|---|---|---|
|**Permutation**|The number of ways to arrange objects.|**YES**|Arranging people, assigning positions (President, VP), locking a combination (which is actually a permutation!)|
|**Combination**|The number of ways to choose objects.|**NO**|Selecting a team, picking lottery numbers, choosing toppings for a pizza.|

## 1. Permutation (Order Matters)

A permutation is the number of ways to arrange $k$ items selected from a set of $n$ distinct items.

### The Formula

The number of permutations of $n$ objects taken $k$ at a time is denoted by $P(n, k)$ or ${}_n P_k$:

$$P(n, k) = \frac{n!}{(n-k)!}$$

Where $n!$ (**$n$ factorial**) is the product of all positive integers less than or equal to $n$ ($n! = n \times (n-1) \times \dots \times 1$).

### Solved Example: Arranging People

**Problem:** Four people are running a race. In how many different ways can the **1st, 2nd, and 3rd place prizes** be awarded?

1. **Identify $n$ and $k$:**
    
    - $n$ (Total number of people) = **4**
        
    - $k$ (Number of positions to fill) = **3**
        
2. **Does Order Matter?** Yes, because getting 1st place is different from getting 2nd place. It is an arrangement.
    
3. Apply the Formula:
    
    $$P(4, 3) = \frac{4!}{(4-3)!} = \frac{4!}{1!} = \frac{4 \times 3 \times 2 \times 1}{1} = 24$$
    

There are **24** different ways to award the three prizes.

---

## 2. Combination (Order Does Not Matter)

A combination is the number of ways to select $k$ items from a set of $n$ distinct items where the order of selection is irrelevant.

### The Formula

The number of combinations of $n$ objects taken $k$ at a time is denoted by $C(n, k)$, ${}_n C_k$, or $\binom{n}{k}$:

$$C(n, k) = \frac{n!}{k! (n-k)!}$$

Notice that the combination formula is the permutation formula divided by $k!$. This division removes the arrangements (order) that are considered the same in a combination.

### Solved Example: Selecting a Team

**Problem:** A basketball team has a roster of 12 players. How many different **5-player starting lineups** can the coach select?

1. **Identify $n$ and $k$:**
    
    - $n$ (Total number of players) = **12**
        
    - $k$ (Number of players to choose) = **5**
        
2. **Does Order Matter?** No. A starting lineup consisting of (Alice, Bob, Carol, David, Eve) is the same team as (Bob, Alice, Carol, Eve, David). It is a selection.
    
3. Apply the Formula:
    
    $$C(12, 5) = \frac{12!}{5! (12-5)!} = \frac{12!}{5! 7!}$$
    
4. Calculate:
    
    $$C(12, 5) = \frac{12 \times 11 \times 10 \times 9 \times 8 \times 7!}{5 \times 4 \times 3 \times 2 \times 1 \times 7!} = \frac{12 \times 11 \times 10 \times 9 \times 8}{5 \times 4 \times 3 \times 2 \times 1}$$
    
    (We can cancel $5 \times 2 = 10$ and $4 \times 3 = 12$ from the denominator with the numerator)
    
    $$C(12, 5) = 11 \times 1 \times 9 \times 8 = 792$$
    

The coach can select **792** different starting lineups.

---

# Mixed Problem Solving Strategy

When you face a word problem, ask yourself one crucial question first:

## **Q: If I swap the position of two selected items, is the resulting outcome considered different?**

|**Answer**|**Action**|
|---|---|
|**YES**|Use **Permutation** (Order matters).|
|**NO**|Use **Combination** (Order doesn't matter).|

### Complex Example: Combining Selection and Arrangement

**Problem:** A committee of **4 people** is to be selected from a group of 5 men and 6 women. If the committee must consist of **exactly 2 men and 2 women**, how many different committees can be formed?

1. **Analyze the task:** This is a two-part **selection** problem (Combination), as the order you pick the people doesn't matter, but we must choose men and women separately.
    
2. **Select the Men:**
    
    - Choose $2$ men from $5$.
        
    - Ways to choose men: $C(5, 2) = \frac{5!}{2! 3!} = \frac{5 \times 4}{2 \times 1} = 10$
        
3. **Select the Women:**
    
    - Choose $2$ women from $6$.
        
    - Ways to choose women: $C(6, 2) = \frac{6!}{2! 4!} = \frac{6 \times 5}{2 \times 1} = 15$
        
4. Combine the Selections (Multiplication Principle): Since the selection of men and the selection of women are independent tasks that form one complete committee, we multiply the results.
    
    $$\text{Total Committees} = (\text{Ways to choose men}) \times (\text{Ways to choose women})$$
    
    $$\text{Total Committees} = 10 \times 15 = 150$$
    

There are **150** different committees that can be formed.

Do you want to try one more problem, or should we move on to the next statistics topic?