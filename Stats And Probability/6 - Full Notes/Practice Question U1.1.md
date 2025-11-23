## 1. Arithmetic Mean Basics: Calculation

The **Arithmetic Mean** (or simply the **Average**) is the sum of all values in a dataset divided by the total number of values.
$$\text{Mean} (\bar{x}) = \frac{\sum x_i}{N}$$

### 1A. For a Simple List of Numbers (Individual Data)

**Example 1: Finding the Mean of a Set**

**Problem:** Find the arithmetic mean of the following five numbers: $12, 18, 25, 10, 35$.

| Step | Calculation | Result |
| :--- | :--- | :--- |
| **1. Sum of Values** ($\sum x_i$) | $12 + 18 + 25 + 10 + 35$ | $100$ |
| **2. Total Count** ($N$) | Number of values | $5$ |
| **3. Calculate Mean** ($\bar{x}$) | $\frac{100}{5}$ | $20$ |

The arithmetic mean is **20**.

***

**Example 2: Finding the Mean of Prime Numbers**

**Problem:** Find the arithmetic mean of the first six prime numbers.

| Step | Calculation | Result |
| :--- | :--- | :--- |
| **1. Identify Values** ($x_i$) | The first six prime numbers are $2, 3, 5, 7, 11, 13$. | |
| **2. Sum of Values** ($\sum x_i$) | $2 + 3 + 5 + 7 + 11 + 13$ | $41$ |
| **3. Total Count** ($N$) | Number of values | $6$ |
| **4. Calculate Mean** ($\bar{x}$) | $\frac{41}{6}$ | $6.83$ (approx.) |

The arithmetic mean is $\frac{41}{6}$ or approximately **6.83**.

***

### 1B. For a List with Frequencies (Discrete Data)

The formula for mean with frequency is:
$$\text{Mean} (\bar{x}) = \frac{\sum f_i x_i}{\sum f_i}$$

**Example 3: Direct Method**

**Problem:** The number of books ($x_i$) read by students in a week, along with the frequency ($f_i$) of students who read that number, is given. Find the mean number of books read.

| Number of Books ($x_i$) | Number of Students ($f_i$) | $f_i x_i$ |
| :---: | :---: | :---: |
| 2 | 3 | $2 \times 3 = 6$ |
| 4 | 2 | $4 \times 2 = 8$ |
| 5 | 1 | $5 \times 1 = 5$ |
| 1 | 2 | $1 \times 2 = 2$ |
| **Total** | $\sum f_i = 8$ | $\sum f_i x_i = 21$ |

$$\text{Mean} (\bar{x}) = \frac{\sum f_i x_i}{\sum f_i} = \frac{21}{8} = 2.625$$

The mean number of books read is **2.625**.

***

**Example 4: Shortcut (Assumed Mean) Method**

**Problem:** Find the mean number of siblings using the Assumed Mean Method.

| Siblings ($x_i$) | Households ($f_i$) |
| :---: | :---: |
| 0 | 2 |
| 1 | 3 |
| 2 | 4 |
| 3 | 1 |

* **Assumed Mean ($A$):** Let's choose $A = 1$.
* **Formula:** $\bar{x} = A + \frac{\sum f_i d_i}{\sum f_i}$, where $d_i = x_i - A$.

| $x_i$ | $f_i$ | Deviation $d_i = x_i - 1$ | $f_i d_i$ |
| :---: | :---: | :---: | :---: |
| 0 | 2 | $0 - 1 = -1$ | $2 \times (-1) = -2$ |
| **1** | **3** | $1 - 1 = 0$ | $3 \times 0 = 0$ |
| 2 | 4 | $2 - 1 = 1$ | $4 \times 1 = 4$ |
| 3 | 1 | $3 - 1 = 2$ | $1 \times 2 = 2$ |
| **Total** | $\sum f_i = 10$ | | $\sum f_i d_i = 4$ |

$$\text{Mean} (\bar{x}) = 1 + \frac{4}{10} = 1 + 0.4 = 1.4$$

The mean number of siblings is **1.4**.

***

### 1C. For Data in Ranges (Continuous Data / Grouped Frequency Distribution)

The mean is calculated using the class mark ($x_i$, or midpoint) of each class interval.

**Example 5: Direct Method (for Grouped Data)**

**Problem:** Find the mean marks from the following distribution.

| Marks (Class Interval) | Frequency ($f_i$) |
| :---: | :---: |
| 0-10 | 5 |
| 10-20 | 12 |
| 20-30 | 15 |
| 30-40 | 6 |
| 40-50 | 2 |

* **Formula:** $\bar{x} = \frac{\sum f_i x_i}{\sum f_i}$, where $x_i$ is the class mark (midpoint).

| Marks | $f_i$ | Class Mark $x_i$ | $f_i x_i$ |
| :---: | :---: | :---: | :---: |
| 0-10 | 5 | $\frac{0+10}{2} = 5$ | $5 \times 5 = 25$ |
| 10-20 | 12 | $\frac{10+20}{2} = 15$ | $12 \times 15 = 180$ |
| 20-30 | 15 | $\frac{20+30}{2} = 25$ | $15 \times 25 = 375$ |
| 30-40 | 6 | $\frac{30+40}{2} = 35$ | $6 \times 35 = 210$ |
| 40-50 | 2 | $\frac{40+50}{2} = 45$ | $2 \times 45 = 90$ |
| **Total** | $\sum f_i = 40$ | | $\sum f_i x_i = 880$ |

$$\text{Mean} (\bar{x}) = \frac{880}{40} = 22$$

The mean marks is **22**.

***

**Example 6: Step Deviation Method**

**Problem:** Calculate the mean daily wage (in $\$$) using the Step Deviation Method.

| Daily Wage ($) | Frequency ($f_i$) |
| :---: | :---: |
| 100-120 | 3 |
| 120-140 | 5 |
| 140-160 | 8 |
| 160-180 | 4 |

* **Class Size ($h$):** $120 - 100 = 20$.
* **Assumed Mean ($A$):** Let's choose the class mark of the third interval: $A = 150$.
* **Formula:** $\bar{x} = A + \left(\frac{\sum f_i u_i}{\sum f_i}\right) \times h$, where $u_i = \frac{x_i - A}{h}$.

| Wage | $f_i$ | Class Mark $x_i$ | $d_i = x_i - 150$ | $u_i = d_i/20$ | $f_i u_i$ |
| :---: | :---: | :---: | :---: | :---: | :---: |
| 100-120 | 3 | 110 | $-40$ | $-2$ | $-6$ |
| 120-140 | 5 | 130 | $-20$ | $-1$ | $-5$ |
| **140-160** | **8** | **150** | $0$ | $0$ | $0$ |
| 160-180 | 4 | 170 | $20$ | $1$ | $4$ |
| **Total** | $\sum f_i = 20$ | | | | $\sum f_i u_i = -7$ |

$$\text{Mean} (\bar{x}) = 150 + \left(\frac{-7}{20}\right) \times 20$$
$$\text{Mean} (\bar{x}) = 150 + (-7) = 143$$

The mean daily wage is **$\$$143**.

***

## 2. Special Cases & Other Types of Means

### 2A. Finding a Missing Number

**Example 7: Single Missing Value**

**Problem:** The arithmetic mean of 5 numbers is 45. Four of the numbers are $30, 65, 40,$ and $52$. What is the fifth number?

1.  **Find the Total Sum:** The sum of $N$ numbers is $N \times \text{Mean}$.
    $$\text{Total Sum} = 5 \times 45 = 225$$
2.  **Find the Sum of Known Numbers:**
    $$\text{Sum of Known} = 30 + 65 + 40 + 52 = 187$$
3.  **Find the Missing Number:**
    $$\text{Missing Number} = \text{Total Sum} - \text{Sum of Known}$$
    $$\text{Missing Number} = 225 - 187 = 38$$

The fifth number is **38**.

***

**Example 8: Score in the Last Game**

**Problem:** A cricket player's average score in 8 innings is 58 runs. Their scores in the first 7 innings are $45, 72, 60, 50, 81, 35,$ and $68$. What was the score in the 8th inning?

1.  **Total Runs in 8 Innings:**
    $$\text{Total Runs} = 8 \times 58 = 464$$
2.  **Total Runs in 7 Innings:**
    $$\text{Sum of 7 Scores} = 45 + 72 + 60 + 50 + 81 + 35 + 68 = 411$$
3.  **Score in the 8th Inning:**
    $$\text{Score} = 464 - 411 = 53$$

The score in the 8th inning was **53 runs**.

***

### 2B. Combined Average

The **Combined Average** is the overall average of two or more groups. It is a type of weighted average where the weights are the number of items in each group.
$$\text{Combined Average} = \frac{N_1 \bar{x}_1 + N_2 \bar{x}_2}{N_1 + N_2}$$

**Example 9: Combined Average of Two Classes**

**Problem:** Section A has 30 students ($N_1$) with an average score of 75 ($\bar{x}_1$). Section B has 20 students ($N_2$) with an average score of 85 ($\bar{x}_2$). Find the combined average score of the entire class.

1.  **Total Score of Section A:** $N_1 \bar{x}_1 = 30 \times 75 = 2250$
2.  **Total Score of Section B:** $N_2 \bar{x}_2 = 20 \times 85 = 1700$
3.  **Total Students:** $N_1 + N_2 = 30 + 20 = 50$
4.  **Combined Average:**
    $$\text{Combined Average} = \frac{2250 + 1700}{50} = \frac{3950}{50} = 79$$

The combined average score is **79**.

***

**Example 10: Combined Average Weight**

**Problem:** The average weight of 10 boys ($N_B$) is $40 \text{ kg}$ ($\bar{x}_B$), and the average weight of 5 girls ($N_G$) is $35 \text{ kg}$ ($\bar{x}_G$). What is the average weight of all 15 students?

1.  **Total Weight of Boys:** $10 \times 40 = 400 \text{ kg}$
2.  **Total Weight of Girls:** $5 \times 35 = 175 \text{ kg}$
3.  **Total Students:** $10 + 5 = 15$
4.  **Combined Average:**
    $$\text{Combined Average} = \frac{400 + 175}{15} = \frac{575}{15} \approx 38.33$$

The average weight of all 15 students is approximately **$38.33 \text{ kg}$**.

***

### 2C. Weighted Average

The **Weighted Average** is used when different data points have different degrees of importance (weights, $w_i$).
$$\text{Weighted Average} = \frac{\sum w_i x_i}{\sum w_i}$$

**Example 11: Weighted Grade Point Average (WGPA)**

**Problem:** A student has the following grades ($x_i$): Math (4 credits, $w_i=4$, grade 90), English (3 credits, $w_i=3$, grade 85), and History (2 credits, $w_i=2$, grade 95). Calculate the student's WGPA.

1.  **Calculate Weighted Grade $\sum w_i x_i$**:
    * Math: $4 \times 90 = 360$
    * English: $3 \times 85 = 255$
    * History: $2 \times 95 = 190$
    $$\sum w_i x_i = 360 + 255 + 190 = 805$$
2.  **Total Weight $\sum w_i$**:
    $$\sum w_i = 4 + 3 + 2 = 9$$
3.  **Weighted Average (WGPA):**
    $$\text{WGPA} = \frac{805}{9} \approx 89.44$$

The student's Weighted Grade Point Average is approximately **89.44**.

***

**Example 12: Weighted Average Weight**

**Problem:** A furniture store sells 3 types of chairs: Standard (weight $10 \text{ kg}$, 50 units sold), Premium (weight $15 \text{ kg}$, 30 units sold), and Basic (weight $8 \text{ kg}$, 20 units sold). Find the weighted average weight of a chair sold. (The number of units sold serves as the weight $w_i$).

1.  **Calculate Total Weighted Weight $\sum w_i x_i$**:
    * Standard: $50 \times 10 = 500 \text{ kg}$
    * Premium: $30 \times 15 = 450 \text{ kg}$
    * Basic: $20 \times 8 = 160 \text{ kg}$
    $$\sum w_i x_i = 500 + 450 + 160 = 1110 \text{ kg}$$
2.  **Total Weight (Total Units Sold) $\sum w_i$**:
    $$\sum w_i = 50 + 30 + 20 = 100$$
3.  **Weighted Average Weight:**
    $$\text{Weighted Average} = \frac{1110}{100} = 11.1$$

The weighted average weight of a chair sold is **$11.1 \text{ kg}$**.