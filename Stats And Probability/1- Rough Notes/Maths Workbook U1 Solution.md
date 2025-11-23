## 11\. Compute the quartile deviation for the following data: 10, 30, 5, 12, 20, 40, 25, 15, 18.

The **Quartile Deviation (QD)** is calculated using the formula:
$$\text{QD} = \frac{Q_3 - Q_1}{2}$$

**Step 1: Sort the data.**
The sorted data is: $5, 10, 12, 15, 18, 20, 25, 30, 40$.
The number of observations is $n=9$.

**Step 2: Calculate the First Quartile ($Q_1$).**
Using the position formula $\text{Position of } Q_k = \frac{k(n+1)}{4}$, the position of $Q_1$ is $\frac{1(9+1)}{4} = 2.5\text{-th term}$.
$$Q_1 = \text{2nd term} + 0.5 \times (\text{3rd term} - \text{2nd term}) = 10 + 0.5 \times (12 - 10) = \mathbf{11}$$
*(Alternatively, using the $25^{th}$ percentile definition: $Q_1 = 12$. We will proceed with the textbook formula for a small, discrete set).*

**Step 3: Calculate the Third Quartile ($Q_3$).**
The position of $Q_3$ is $\frac{3(9+1)}{4} = 7.5\text{-th term}$.
$$Q_3 = \text{7th term} + 0.5 \times (\text{8th term} - \text{7th term}) = 25 + 0.5 \times (30 - 25) = 25 + 2.5 = \mathbf{27.5}$$

**Step 4: Compute the Quartile Deviation.**
$$\text{QD} = \frac{Q_3 - Q_1}{2} = \frac{27.5 - 11}{2} = \frac{16.5}{2} = \mathbf{8.25}$$

**The quartile deviation is $8.25$.**

-----

## 12\. The standard deviation of $n$ observations is $\sigma$. If each observation is multiplied by a constant $k$, what is the new standard deviation? Also, if a constant $c$ is added to each observation instead, what happens to the standard deviation?

### Effect of Multiplication

If each observation is multiplied by a constant $k$, the new standard deviation ($\sigma_{\text{new}}$) is the absolute value of $k$ times the original standard deviation ($\sigma$).
$$\sigma_{\text{new}} = |k|\sigma$$
The standard deviation is a measure of dispersion, and multiplication by $k$ changes the scale of dispersion by a factor of $|k|$.

### Effect of Addition

If a constant $c$ is added to each observation, the new standard deviation ($\sigma_{\text{new}}$) **remains the same** as the original standard deviation ($\sigma$).
$$\sigma_{\text{new}} = \sigma$$
Adding a constant only shifts the entire data set, but it does not change the spread or dispersion of the data around the mean.

-----

## 13\. Calculate the median of the following data that relates to the monthly salaries of employees (in thousand rupees): 110, 115, 108, 112, 120, 116, 140, 135, 128, 132.

The median is the middle-most value of a sorted data set.

**Step 1: Sort the data.**
The sorted salaries (in thousand rupees) are:
$$108, 110, 112, 115, 116, 120, 128, 132, 135, 140$$
The number of observations is $n=10$ (an even number).

**Step 2: Calculate the median.**
For an even number of observations, the median is the average of the two middle terms: the $\frac{n}{2}\text{-th}$ term and the $(\frac{n}{2} + 1)\text{-th}$ term.

  * $\frac{10}{2} = 5\text{-th term} = 116$
  * $(\frac{10}{2} + 1) = 6\text{-th term} = 120$

$$\text{Median} = \frac{5\text{-th term} + 6\text{-th term}}{2} = \frac{116 + 120}{2} = \frac{236}{2} = \mathbf{118}$$

**The median salary is 118 thousand rupees.**

-----

## 14\. In a frequency distribution, the coefficient of skewness based on the quartiles is 0.6. If the sum of the upper and the lower quartile is 100 and the median is 38, determine the values of the upper and the lower quartiles.

The formula for the **Quartile Coefficient of Skewness** (Bowley's coefficient) is:
$$S_k = \frac{Q_3 + Q_1 - 2Q_2}{Q_3 - Q_1}$$

We are given:

  * $S_k = 0.6$
  * $Q_3 + Q_1 = 100$
  * Median ($Q_2$) $= 38$

**Step 1: Substitute the given values into the formula to find the difference of the quartiles.**
$$0.6 = \frac{100 - 2(38)}{Q_3 - Q_1}$$
$$0.6 = \frac{100 - 76}{Q_3 - Q_1}$$
$$0.6 = \frac{24}{Q_3 - Q_1}$$

Rearrange to solve for $(Q_3 - Q_1)$:
$$Q_3 - Q_1 = \frac{24}{0.6} = \mathbf{40}$$

**Step 2: Solve the system of two linear equations.**
We have:

1.  $Q_3 + Q_1 = 100$
2.  $Q_3 - Q_1 = 40$

Add Equation (1) and Equation (2):
$$(Q_3 + Q_1) + (Q_3 - Q_1) = 100 + 40$$
$$2Q_3 = 140$$
$$Q_3 = \mathbf{70}$$

Substitute $Q_3 = 70$ back into Equation (1):
$$70 + Q_1 = 100$$
$$Q_1 = 100 - 70$$
$$Q_1 = \mathbf{30}$$

**The upper quartile ($Q_3$) is $70$ and the lower quartile ($Q_1$) is $30$.**

-----

## 15\. The standard deviation of a symmetric distribution is 4. Calculate the value of $\mu_4$ so that the distribution must be mesokurtic.

A distribution is defined as **mesokurtic** if its coefficient of kurtosis ($\beta_2$) is equal to 3.

The relationship between the fourth central moment ($\mu_4$) and the second central moment ($\mu_2$) is:
$$\beta_2 = \frac{\mu_4}{\mu_2^2}$$

We are given:

  * Standard deviation ($\sigma$) $= 4$.
  * For a mesokurtic distribution, $\beta_2 = 3$.

**Step 1: Calculate the second central moment ($\mu_2$).**
The second central moment is the variance ($\sigma^2$).
$$\mu_2 = \sigma^2 = 4^2 = 16$$

**Step 2: Calculate $\mu_4$ for $\beta_2 = 3$.**
$$3 = \frac{\mu_4}{\mu_2^2}$$
$$3 = \frac{\mu_4}{16^2}$$
$$3 = \frac{\mu_4}{256}$$
$$\mu_4 = 3 \times 256 = \mathbf{768}$$

**The value of $\mu_4$ must be $768$ for the distribution to be mesokurtic.**

-----

## 16\. A bus runs at a speed of 60 kph over 50 kilometers; the next 30 kilometers at a speed of 40 kph; the next 20 kilometers at a speed of 30 kph; and the final run of 50 kilometers at a speed of 25 kph. Find the average speed in kilometers per hour.

The **average speed** is calculated by the formula:
$$\text{Average Speed} = \frac{\text{Total Distance}}{\text{Total Time}}$$

**Step 1: Calculate the Total Distance.**
$$\text{Total Distance} = 50 + 30 + 20 + 50 = \mathbf{150} \text{ km}$$

**Step 2: Calculate the Total Time.**
Time is calculated as $\text{Time} = \frac{\text{Distance}}{\text{Speed}}$.

  * $T_1 = \frac{50 \text{ km}}{60 \text{ kph}} = \frac{5}{6} \text{ hours}$
  * $T_2 = \frac{30 \text{ km}}{40 \text{ kph}} = \frac{3}{4} \text{ hours}$
  * $T_3 = \frac{20 \text{ km}}{30 \text{ kph}} = \frac{2}{3} \text{ hours}$
  * $T_4 = \frac{50 \text{ km}}{25 \text{ kph}} = 2 \text{ hours}$

$$\text{Total Time} = T_1 + T_2 + T_3 + T_4 = \frac{5}{6} + \frac{3}{4} + \frac{2}{3} + 2$$
To sum the fractions, use the common denominator $12$:
$$\text{Total Time} = \frac{10}{12} + \frac{9}{12} + \frac{8}{12} + \frac{24}{12} = \frac{10 + 9 + 8 + 24}{12} = \frac{\mathbf{51}}{\mathbf{12}} \text{ hours}$$

**Step 3: Compute the Average Speed.**
$$\text{Average Speed} = \frac{150 \text{ km}}{\frac{51}{12} \text{ hours}} = 150 \times \frac{12}{51}$$
$$\text{Average Speed} = \frac{1800}{51}$$

Simplify the fraction by dividing the numerator and denominator by their greatest common divisor, 3:
$$\text{Average Speed} = \frac{1800 \div 3}{51 \div 3} = \frac{\mathbf{600}}{\mathbf{17}} \text{ kph}$$

As a decimal, this is approximately:
$$\text{Average Speed} \approx 35.29 \text{ kph}$$

**The average speed is $\frac{600}{17}$ kph (or approximately $35.29$ kph).**


---


## 17\. Moments About the Mean, Skewness, and Kurtosis

This problem requires converting the moments about an arbitrary point (working mean) to moments about the actual mean, and then calculating the measures of skewness ($\beta_1$) and kurtosis ($\beta_2$).

### Given Data

  * Working Mean ($A$) = $28.5$
  * Moments about $A$ ($\mu'_k$):
      * $\mu'_1 = c = 0.294$
      * $\mu'_2 = 7.144$
      * $\mu'_3 = 42.409$
      * $\mu'_4 = 454.98$

-----

### Part 1: Moments About the Mean ($\mu_k$)

We use the conversion formulas, where $c = \mu'_1 = 0.294$.

#### 1\. First Moment ($\mu_1$)

The first moment about the mean is always zero.
$$\mu_1 = 0$$

#### 2\. Second Moment ($\mu_2$)

$$\mu_2 = \mu'_2 - c^2$$
$$\mu_2 = 7.144 - (0.294)^2$$
$$\mu_2 = 7.144 - 0.086436 = \mathbf{7.057564}$$
*($\mu_2$ is the **Variance**).*

#### 3\. Third Moment ($\mu_3$)

$$\mu_3 = \mu'_3 - 3\mu'_2 c + 2c^3$$
$$\mu_3 = 42.409 - 3(7.144)(0.294) + 2(0.294)^3$$
$$\mu_3 = 42.409 - 6.295488 + 0.050800 \approx \mathbf{36.164312}$$
*(Using the exact intermediate result from the calculation: $\mu_3 \approx 36.158816$)*

#### 4\. Fourth Moment ($\mu_4$)

$$\mu_4 = \mu'_4 - 4\mu'_3 c + 6\mu'_2 c^2 - 3c^4$$
$$\mu_4 = 454.98 - 4(42.409)(0.294) + 6(7.144)(0.294)^2 - 3(0.294)^4$$
$$\mu_4 = 454.98 - 49.882488 + 3.682390 - 0.023533 \approx \mathbf{408.756369}$$
*(Using the exact intermediate result from the calculation: $\mu_4 \approx 408.789595$)*

| Moment about the Mean | Value |
| :---: | :---: |
| $\mu_1$ | **0** |
| $\mu_2$ | **7.0576** |
| $\mu_3$ | **36.1588** |
| $\mu_4$ | **408.7896** |

-----

### Part 2: Measures of Skewness

The measure of skewness is given by $\beta_1$ (or its square root, $\gamma_1$).

$$\beta_1 = \frac{\mu_3^2}{\mu_2^3}$$
$$\beta_1 = \frac{(36.158816)^2}{(7.057564)^3} = \frac{1307.458}{351.464} \approx \mathbf{3.7193}$$

**Interpretation:** Since $\beta_1 > 0$, the distribution is **positively skewed**.

-----

### Part 3: Measures of Kurtosis

The measure of kurtosis is given by $\beta_2$.

$$\beta_2 = \frac{\mu_4}{\mu_2^2}$$
$$\beta_2 = \frac{408.789595}{(7.057564)^2} = \frac{408.789595}{49.809226} \approx \mathbf{8.2071}$$

**Interpretation:** Since $\beta_2 > 3$, the distribution is **leptokurtic** (more peaked and heavier-tailed than a normal distribution).

| Measure | Value |
| :---: | :---: |
| Skewness ($\beta_1$) | **3.7193** |
| Kurtosis ($\beta_2$) | **8.2071** |


## 18\. Find the First Four Moments About the Origin

This problem requires calculating the first four moments about the origin ($\mu'_k$) using the given mean, variance, and measures of skewness ($\gamma_1$) and kurtosis ($\beta_2$).

### Given Data

  * Mean ($\bar{X}$) = $\mathbf{10}$
  * Variance ($\mu_2$) = $\mathbf{16}$
  * Skewness ($\gamma_1$) = $\mathbf{1}$
  * Kurtosis ($\beta_2$) = $\mathbf{4}$

### Step 1: Calculate $\mu'_1$

The first moment about the origin is equal to the mean.
$$\mu'_1 = \bar{X} = \mathbf{10}$$

-----

### Step 2: Calculate $\mu_3$ and $\mu_4$ (Moments about the Mean)

We need the third ($\mu_3$) and fourth ($\mu_4$) moments about the mean before converting them to moments about the origin.

#### A. Third Moment ($\mu_3$)

The skewness coefficient $\gamma_1$ is related to $\mu_3$ and $\mu_2$ by:
$$\gamma_1 = \frac{\mu_3}{\sqrt{\mu_2^3}} \quad \implies \quad \mu_3 = \gamma_1 \cdot (\mu_2)^{3/2}$$
$$\mu_3 = 1 \cdot (16)^{3/2} = 1 \cdot (\sqrt{16})^3 = 1 \cdot 4^3 = \mathbf{64}$$

#### B. Fourth Moment ($\mu_4$)

The kurtosis coefficient $\beta_2$ is related to $\mu_4$ and $\mu_2$ by:
$$\beta_2 = \frac{\mu_4}{\mu_2^2} \quad \implies \quad \mu_4 = \beta_2 \cdot \mu_2^2$$
$$\mu_4 = 4 \cdot (16)^2 = 4 \cdot 256 = \mathbf{1024}$$

-----

### Step 3: Calculate $\mu'_2, \mu'_3, \mu'_4$ (Moments about the Origin)

We use the conversion formulas where $c = \mu'_1 = 10$.

#### A. Second Moment ($\mu'_2$)

$$\mu'_2 = \mu_2 + (\mu'_1)^2$$
$$\mu'_2 = 16 + (10)^2 = 16 + 100 = \mathbf{116}$$

#### B. Third Moment ($\mu'_3$)

$$\mu'_3 = \mu_3 + 3\mu_2\mu'_1 + (\mu'_1)^3$$
$$\mu'_3 = 64 + 3(16)(10) + (10)^3$$
$$\mu'_3 = 64 + 480 + 1000 = \mathbf{1544}$$

#### C. Fourth Moment ($\mu'_4$)

$$\mu'_4 = \mu_4 + 4\mu_3\mu'_1 + 6\mu_2(\mu'_1)^2 + (\mu'_1)^4$$
$$\mu'_4 = 1024 + 4(64)(10) + 6(16)(10)^2 + (10)^4$$
$$\mu'_4 = 1024 + 2560 + 9600 + 10000 = \mathbf{23184}$$

-----

### Summary of Moments About the Origin

The first four moments about the origin are:

|  Moment  |   Value   |
| :------: | :-------: |
| $\mu'_1$ |  **10**   |
| $\mu'_2$ |  **116**  |
| $\mu'_3$ | **1544**  |
| $\mu'_4$ | **23184** |

## Question 19: Calculate the Mode using Grouping

| Size of Items ($X$) | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 |
| :---: | :-: | :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| No. of Items ($f$) | 5 | 6 | 8 | 7 | 9 | 8 | 9 | 6 |

---

### Step 1: Prepare the Grouping Table

We create five additional columns to group the frequencies:
* **Col 2:** Grouping frequencies in twos (starting from the first frequency).
* **Col 3:** Grouping frequencies in twos (starting from the second frequency).
* **Col 4:** Grouping frequencies in threes (starting from the first frequency).
* **Col 5:** Grouping frequencies in threes (starting from the second frequency).
* **Col 6:** Grouping frequencies in threes (starting from the third frequency).

| $X$ | $f$ (Col 1) | Col 2 | Col 3 | Col 4 | Col 5 | Col 6 |
| :-: | :---: | :---: | :---: | :---: | :---: | :---: |
| 8 | 5 | $\mathbf{11}$ (5+6) | | $\mathbf{19}$ (5+6+8) | | |
| 9 | 6 | | $\mathbf{14}$ (6+8) | | $\mathbf{21}$ (6+8+7) | |
| 10 | 8 | $\mathbf{15}$ (8+7) | | | | $\mathbf{24}$ (8+7+9) |
| 11 | 7 | | $\mathbf{16}$ (7+9) | $\mathbf{24}$ (7+9+8) | | |
| **12** | $\mathbf{9}$ | $\mathbf{17}$ (9+8) | | | $\mathbf{26}$ (9+8+9) | |
| 13 | 8 | | $\mathbf{17}$ (8+9) | | | $\mathbf{23}$ (8+9+6) |
| **14** | $\mathbf{9}$ | $\mathbf{15}$ (9+6) | | $\mathbf{23}$ (9+6) | | |
| 15 | 6 | | | | | |

*The largest sum in each column is **bolded**.*

---

### Step 2: Prepare the Analysis Table

We record which items ($X$ values) contributed to the largest sum in each column.

| Column | Largest Sum | Items Covered |
| :---: | :---: | :---: |
| 1 ($f$) | **9** | **12, 14** |
| 2 (2s from 1st) | **17** | **12, 13** |
| 3 (2s from 2nd) | **17** | **13, 14** |
| 4 (3s from 1st) | **24** | **11, 12, 13** |
| 5 (3s from 2nd) | **26** | **12, 13, 14** |
| 6 (3s from 3rd) | **24** | **10, 11, 12** |

---

### Step 3: Count the Highest Frequency

We count how many times each item appears as a component of the largest group sums.

| Item ($X$) | 8 | 9 | 10 | 11 | **12** | 13 | 14 | 15 | Total Tally |
| :---: | :-: | :-: | :-: | :-: | :---: | :-: | :-: | :-: | :---: |
| Col 1 | | | | | 1 | | 1 | | 2 |
| Col 2 | | | | | 1 | 1 | | | 2 |
| Col 3 | | | | | | 1 | 1 | | 2 |
| Col 4 | | | | 1 | 1 | 1 | | | 3 |
| Col 5 | | | | | 1 | 1 | 1 | | 3 |
| Col 6 | | | 1 | 1 | 1 | | | | 3 |
| **Total Tally** | **0** | **0** | **1** | **2** | **5** | **4** | **3** | **0** | |

The item with the highest total tally is the mode.

* The item $\mathbf{12}$ has the highest tally of **5**.

### Conclusion

The mode calculated using the grouping method is $\mathbf{12}$.

**Note on Bimodality:** The initial inspection suggested bimodality (12 and 14). However, the grouping method consolidates the frequencies and shows that the item $\mathbf{12}$ is involved in more high-frequency groupings (5 tallies) than the item $\mathbf{14}$ (3 tallies). Therefore, the actual mode is **12**.

## 20. Mode and Standard Deviation for Grouped Data 📊

This problem asks for the **Mode** and the **Standard Deviation ($\sigma$)** for the given inclusive grouped data.

| Marks | No. of Candidates ($f$) |
| :---: | :---: |
| 1-10 | 3 |
| 11-20 | 16 |
| 21-30 | 26 |
| 31-40 | 31 |
| 41-50 | 16 |
| 51-60 | 8 |
| **Total** | **$N=100$** |

---

### Part 1: Calculation of the Mode ($Z$)

Since the data is inclusive, we first convert the limits to **exclusive** limits by applying a continuity correction of $0.5$.

#### 1. Identify the Modal Class and Parameters
* The **highest frequency** is $\mathbf{31}$, corresponding to the class $\mathbf{31-40}$.
* $L$ (Lower Boundary of exclusive class) $= 31 - 0.5 = \mathbf{30.5}$
* $h$ (Class Width) $= 40.5 - 30.5 = \mathbf{10}$
* $f_1$ (Modal Frequency) $= \mathbf{31}$
* $f_0$ (Preceding Frequency) $= \mathbf{26}$
* $f_2$ (Succeeding Frequency) $= \mathbf{16}$

#### 2. Apply the Mode Formula
$$\text{Mode } (Z) = L + \frac{f_1 - f_0}{2f_1 - f_0 - f_2} \times h$$
$$Z = 30.5 + \frac{31 - 26}{2(31) - 26 - 16} \times 10$$
$$Z = 30.5 + \frac{5}{62 - 42} \times 10$$
$$Z = 30.5 + \frac{5}{20} \times 10$$
$$Z = 30.5 + \frac{1}{4} \times 10 = 30.5 + 2.5 = \mathbf{33.0}$$

**The Mode is 33.0 marks.**

---

### Part 2: Calculation of Standard Deviation ($\sigma$)

We use the **step-deviation method** for efficiency. Let the assumed mean $A$ be the midpoint of the modal class: $A = 35.5$.

| Marks | $f$ | Midpoint ($x$) | $d' = \frac{x - 35.5}{10}$ | $fd'$ | $f(d')^2$ |
| :---: | :-: | :---: | :---: | :---: | :---: |
| 1-10 | 3 | 5.5 | -3 | -9 | 27 |
| 11-20 | 16 | 15.5 | -2 | -32 | 64 |
| 21-30 | 26 | 25.5 | -1 | -26 | 26 |
| **31-40** | **31** | **35.5 (A)** | **0** | **0** | **0** |
| 41-50 | 16 | 45.5 | 1 | 16 | 16 |
| 51-60 | 8 | 55.5 | 2 | 16 | 32 |
| **Total** | $\mathbf{N=100}$ | | | $\sum fd' = -35$ | $\sum f(d')^2 = 165$ |

#### 1. Apply the Standard Deviation Formula
$$\sigma = \sqrt{\frac{\sum f(d')^2}{N} - \left(\frac{\sum fd'}{N}\right)^2} \times h$$
$$\sigma = \sqrt{\frac{165}{100} - \left(\frac{-35}{100}\right)^2} \times 10$$
$$\sigma = \sqrt{1.65 - 0.1225} \times 10$$
$$\sigma = \sqrt{1.5275} \times 10$$
$$\sigma \approx 1.2359 \times 10 = \mathbf{12.36}$$

**The Standard Deviation is 12.36 marks** (rounded to two decimal places).

## 21. Check the Skewness of the Following Two Series 

Skewness measures the degree to which a distribution is asymmetrical. We'll use **Pearson's First Coefficient of Skewness ($S_k$)** to check the skewness:

$$S_k = \frac{\text{Mean} - \text{Mode}}{\text{S.D.}} \quad \text{OR (often used as an approximation)}$$
$$S_k \approx \frac{3 (\text{Mean} - \text{Median})}{\text{S.D.}}$$

We will use the second formula since the median is given.

---

### Series (a)

| Measure | Value |
| :---: | :---: |
| Mean | 32 |
| Median | 34 |
| S.D. | 20 |

**Calculate Skewness:**
$$S_k = \frac{3 (\text{Mean} - \text{Median})}{\text{S.D.}} = \frac{3 (32 - 34)}{20}$$
$$S_k = \frac{3 (-2)}{20} = \frac{-6}{20} = -\mathbf{0.3}$$

**Conclusion for Series (a):**
Since the coefficient of skewness ($S_k$) is **negative** ($-0.3$), the distribution of Series (a) is **Negatively Skewed** (or skewed to the left).

---

### Series (b)

| Measure | Value |
| :---: | :---: |
| Mean | 32 |
| Median | 36 |
| S.D. | 25 |

**Calculate Skewness:**
$$S_k = \frac{3 (\text{Mean} - \text{Median})}{\text{S.D.}} = \frac{3 (32 - 36)}{25}$$
$$S_k = \frac{3 (-4)}{25} = \frac{-12}{25} = -\mathbf{0.48}$$

**Conclusion for Series (b):**
Since the coefficient of skewness ($S_k$) is **negative** ($-0.48$), the distribution of Series (b) is also **Negatively Skewed**.

---

### Summary
* **Series (a):** Negatively Skewed ($S_k = -0.3$)
* **Series (b):** Negatively Skewed ($S_k = -0.48$)

## 22. First Four Moments About the Mean and Skewness 📈

This problem requires calculating the first four moments about the mean ($\mu_k$) and the measure of skewness ($\beta_1$) for the given discrete frequency distribution.

| $X$ | 2 | 3 | 4 | 5 | 6 |
| :-: | :-: | :-: | :-: | :-: | :-: |
| $f$ | 1 | 3 | 7 | 3 | 1 |

### Step 1: Calculate the Mean ($\bar{X}$)

To find the moments about the mean, we first need to calculate the mean.

$$\bar{X} = \frac{\sum fX}{\sum f}$$

| $X$ | $f$ | $fX$ |
| :-: | :-: | :-: |
| 2 | 1 | 2 |
| 3 | 3 | 9 |
| 4 | 7 | 28 |
| 5 | 3 | 15 |
| 6 | 1 | 6 |
| **Total** | $\sum f = 15$ | $\sum fX = 60$ |

$$\bar{X} = \frac{60}{15} = \mathbf{4}$$

---

### Step 2: Calculate Moments About the Mean ($\mu_k$)

The central moment formula is: $\mu_k = \frac{\sum f(X - \bar{X})^k}{\sum f}$.
Here, the deviation $d = X - 4$.

| $X$ | $f$ | $d = X - 4$ | $fd$ | $fd^2$ | $fd^3$ | $fd^4$ |
| :-: | :-: | :---: | :-: | :---: | :---: | :---: |
| 2 | 1 | -2 | -2 | 4 | -8 | 16 |
| 3 | 3 | -1 | -3 | 3 | -3 | 3 |
| 4 | 7 | 0 | 0 | 0 | 0 | 0 |
| 5 | 3 | 1 | 3 | 3 | 3 | 3 |
| 6 | 1 | 2 | 2 | 4 | 8 | 16 |
| **Total** | $\mathbf{N=15}$ | | $\mathbf{0}$ | $\mathbf{14}$ | $\mathbf{0}$ | $\mathbf{38}$ |

**1. First Moment ($\mu_1$):**
$$\mu_1 = \frac{\sum fd}{N} = \frac{0}{15} = \mathbf{0}$$
*(This is always true for the first moment about the mean).*

**2. Second Moment ($\mu_2$):**
$$\mu_2 = \frac{\sum fd^2}{N} = \frac{14}{15} \approx \mathbf{0.9333}$$

**3. Third Moment ($\mu_3$):**
$$\mu_3 = \frac{\sum fd^3}{N} = \frac{0}{15} = \mathbf{0}$$

**4. Fourth Moment ($\mu_4$):**
$$\mu_4 = \frac{\sum fd^4}{N} = \frac{38}{15} \approx \mathbf{2.5333}$$

---

### Step 3: Calculate $\beta_1$ and Check for Symmetry

The measure of skewness is $\beta_1$:

$$\beta_1 = \frac{\mu_3^2}{\mu_2^3}$$
$$\beta_1 = \frac{(0)^2}{(14/15)^3} = \mathbf{0}$$

**Conclusion on Skewness:**
Since $\mu_3 = 0$ and consequently $\beta_1 = 0$, the distribution is **symmetrical**. This is also confirmed by the frequencies being symmetrical around the mean (the frequencies 1, 3, 7, 3, 1 are symmetric about $X=4$).

---

### Summary of Results

| Moment | Value |
| :---: | :---: |
| $\mu_1$ | **0** |
| $\mu_2$ | **14/15 $\approx$ 0.9333** |
| $\mu_3$ | **0** |
| $\mu_4$ | **38/15 $\approx$ 2.5333** |
| $\beta_1$ | **0** |

**Is it a symmetrical distribution?** **Yes**, because $\mu_3 = 0$ and $\beta_1 = 0$.

I see you're ready for question **23** now!

## 23. Moments About the Mean and the Origin

This problem involves converting moments from an arbitrary value ($A=2$) to the **mean** ($\mu_k$) and then to the **origin** ($\mu'_k$).

### Given Data
* Arbitrary value ($A$) = **2**
* Moments about $A$ ($\mu'_k$):
    * $\mu'_1 (\text{about } 2) = c = \mathbf{1}$
    * $\mu'_2 (\text{about } 2) = \mathbf{2.5}$
    * $\mu'_3 (\text{about } 2) = \mathbf{5.5}$
    * $\mu'_4 (\text{about } 2) = \mathbf{16}$

---

### Part 1: Moments About the Mean ($\mu_k$)

We use the conversion formulas, where $c = \mu'_1 = 1$.

#### 1. First Moment ($\mu_1$)
$$\mu_1 = 0$$

#### 2. Second Moment ($\mu_2$)
$$\mu_2 = \mu'_2 - c^2$$
$$\mu_2 = 2.5 - (1)^2 = 2.5 - 1 = \mathbf{1.5}$$

#### 3. Third Moment ($\mu_3$)
$$\mu_3 = \mu'_3 - 3\mu'_2 c + 2c^3$$
$$\mu_3 = 5.5 - 3(2.5)(1) + 2(1)^3$$
$$\mu_3 = 5.5 - 7.5 + 2 = \mathbf{0}$$

#### 4. Fourth Moment ($\mu_4$)
$$\mu_4 = \mu'_4 - 4\mu'_3 c + 6\mu'_2 c^2 - 3c^4$$
$$\mu_4 = 16 - 4(5.5)(1) + 6(2.5)(1)^2 - 3(1)^4$$
$$\mu_4 = 16 - 22 + 15 - 3 = \mathbf{6}$$

| Moments about the Mean | Value |
| :---: | :---: |
| $\mu_1$ | **0** |
| $\mu_2$ | **1.5** |
| $\mu_3$ | **0** |
| $\mu_4$ | **6** |

---

### Part 2: Moments About the Origin ($\mu'_k$)

The origin is the value $0$. The first moment about the origin is the mean ($\bar{X}$).

#### 1. Mean ($\bar{X}$)
The mean is calculated from the first moment about the arbitrary point $A$:
$$\bar{X} = A + \mu'_1 = 2 + 1 = \mathbf{3}$$
Therefore, $\mu'_1 (\text{about } 0) = \mathbf{3}$.

#### 2. Second Moment ($\mu'_2$)
We use the formula $\mu'_2 = \mu_2 + \bar{X}^2$:
$$\mu'_2 = 1.5 + (3)^2 = 1.5 + 9 = \mathbf{10.5}$$

#### 3. Third Moment ($\mu'_3$)
We use the formula $\mu'_3 = \mu_3 + 3\mu_2\bar{X} + \bar{X}^3$:
$$\mu'_3 = 0 + 3(1.5)(3) + (3)^3$$
$$\mu'_3 = 0 + 13.5 + 27 = \mathbf{40.5}$$

#### 4. Fourth Moment ($\mu'_4$)
We use the formula $\mu'_4 = \mu_4 + 4\mu_3\bar{X} + 6\mu_2\bar{X}^2 + \bar{X}^4$:
$$\mu'_4 = 6 + 4(0)(3) + 6(1.5)(3)^2 + (3)^4$$
$$\mu'_4 = 6 + 0 + 6(1.5)(9) + 81$$
$$\mu'_4 = 6 + 81 + 81 = \mathbf{168}$$

| Moments about the Origin |  Value   |
| :----------------------: | :------: |
|         $\mu'_1$         |  **3**   |
|         $\mu'_2$         | **10.5** |
|         $\mu'_3$         | **40.5** |
|         $\mu'_4$         | **168**  |

I'll solve Question **24** first, which requires calculating the **moment coefficient of skewness** ($\gamma_1$) and **moment coefficient of kurtosis** ($\gamma_2$).

## 24. Moment Coefficients of Skewness and Kurtosis 📈

The data is a discrete frequency distribution. We will use the **step deviation method** to calculate the first four moments about the mean ($\mu_k$).

| Height ($X$) | $f$ |
| :---: | :---: |
| 59 | 0 |
| 61 | 2 |
| 63 | 6 |
| 65 | 20 |
| 67 | 40 |
| 69 | 20 |
| 71 | 8 |
| 73 | 2 |
| 75 | 2 |
| **Total** | **$N=100$** |

### Step 1: Prepare the Calculation Table and Find Moments about an Assumed Mean

Let the Assumed Mean $A$ be the central value, $A = 67$.
The common difference (step size) $h$ is $2$.
Let $d' = \frac{X - A}{h} = \frac{X - 67}{2}$.

| $X$ | $f$ | $d'$ | $fd'$ | $fd'^2$ | $fd'^3$ | $fd'^4$ |
| :---: | :-: | :---: | :---: | :---: | :---: | :---: |
| 59 | 0 | -4 | 0 | 0 | 0 | 0 |
| 61 | 2 | -3 | -6 | 18 | -54 | 162 |
| 63 | 6 | -2 | -12 | 24 | -48 | 96 |
| 65 | 20 | -1 | -20 | 20 | -20 | 20 |
| **67 (A)** | **40** | **0** | **0** | **0** | **0** | **0** |
| 69 | 20 | 1 | 20 | 20 | 20 | 20 |
| 71 | 8 | 2 | 16 | 32 | 64 | 128 |
| 73 | 2 | 3 | 6 | 18 | 54 | 162 |
| 75 | 2 | 4 | 8 | 32 | 128 | 512 |
| **Total** | $\mathbf{N=100}$ | | $\mathbf{6}$ | $\mathbf{164}$ | $\mathbf{144}$ | $\mathbf{1100}$ |

#### Moments about the Assumed Mean ($A$)
$$\mu'_k (\text{in } d') = \frac{\sum fd'^k}{N}$$

* $\mu'_1 = \frac{6}{100} = 0.06$
* $\mu'_2 = \frac{164}{100} = 1.64$
* $\mu'_3 = \frac{144}{100} = 1.44$
* $\mu'_4 = \frac{1100}{100} = 11.00$

---

### Step 2: Convert to Moments about the Mean ($\mu_k$)

We use the conversion formulas, where $c = \mu'_1 = 0.06$.

#### 1. Second Moment ($\mu_2$)
$$\mu_2 = h^2 [\mu'_2 - c^2]$$
$$\mu_2 = 2^2 [1.64 - (0.06)^2] = 4 [1.64 - 0.0036]$$
$$\mu_2 = 4 \times 1.6364 = \mathbf{6.5456}$$

#### 2. Third Moment ($\mu_3$)
$$\mu_3 = h^3 [\mu'_3 - 3\mu'_2 c + 2c^3]$$
$$\mu_3 = 2^3 [1.44 - 3(1.64)(0.06) + 2(0.06)^3]$$
$$\mu_3 = 8 [1.44 - 0.2952 + 0.000432]$$
$$\mu_3 = 8 \times 1.145232 \approx \mathbf{9.161856}$$

#### 3. Fourth Moment ($\mu_4$)
$$\mu_4 = h^4 [\mu'_4 - 4\mu'_3 c + 6\mu'_2 c^2 - 3c^4]$$
$$\mu_4 = 2^4 [11.00 - 4(1.44)(0.06) + 6(1.64)(0.06)^2 - 3(0.06)^4]$$
$$\mu_4 = 16 [11.00 - 0.3456 + 0.035424 - 0.00003888]$$
$$\mu_4 = 16 \times 10.689785 \approx \mathbf{171.03656}$$

---

### Step 3: Calculate the Moment Coefficients

#### 1. Moment Coefficient of Skewness ($\gamma_1$)
We use the measure $\beta_1$ and $\gamma_1 = \sqrt{\beta_1}$.
$$\beta_1 = \frac{\mu_3^2}{\mu_2^3}$$
$$\beta_1 = \frac{(9.161856)^2}{(6.5456)^3} = \frac{83.9406}{280.4578} \approx 0.2993$$
$$\gamma_1 = \sqrt{\beta_1} \approx \sqrt{0.2993} \approx \mathbf{0.5471}$$

#### 2. Moment Coefficient of Kurtosis ($\gamma_2$)
We use the measure $\beta_2$ and $\gamma_2 = \beta_2 - 3$.
$$\beta_2 = \frac{\mu_4}{\mu_2^2}$$
$$\beta_2 = \frac{171.03656}{(6.5456)^2} = \frac{171.03656}{42.84539} \approx 3.9918$$
$$\gamma_2 = \beta_2 - 3 = 3.9918 - 3 \approx \mathbf{0.9918}$$

### Final Answer:

| Measure | Value | Conclusion |
| :---: | :---: | :---: |
| Moment Coefficient of Skewness ($\gamma_1$) | **0.5471** | **Positively Skewed** |
| Moment Coefficient of Kurtosis ($\gamma_2$) | **0.9918** | **Leptokurtic** ($\beta_2 > 3$) |

## 25. Mean, Median, and Quartiles for a Cumulative Frequency Distribution 📊

The given data is a **"Less Than" cumulative frequency (c.f.) distribution**. We must first convert it into a simple frequency distribution with class intervals.

### Step 1: Convert to Simple Frequency Distribution

| Marks (Exclusive Class) | No. of Students (c.f.) | Frequency ($f$) |
| :---: | :---: | :---: |
| 0-10 | 15 | 15 |
| 10-20 | 35 | $35 - 15 = 20$ |
| 20-30 | 60 | $60 - 35 = 25$ |
| 30-40 | 84 | $84 - 60 = 24$ |
| 40-50 | 94 | $94 - 84 = 10$ |
| 50-60 | 127 | $127 - 94 = 33$ |
| 60-70 | 198 | $198 - 127 = 71$ |
| 70-80 | 249 | $249 - 198 = 51$ |
| **Total** | | $\mathbf{N=249}$ |

---

### Step 2: Calculate the Mean ($\bar{X}$)

We use the mid-point ($x$) method, taking the Assumed Mean $A=35$ for calculation simplicity.

| Class | $f$ | Midpoint ($x$) | $d' = \frac{x - 35}{10}$ | $fd'$ |
| :---: | :-: | :---: | :---: | :---: |
| 0-10 | 15 | 5 | -3 | -45 |
| 10-20 | 20 | 15 | -2 | -40 |
| 20-30 | 25 | 25 | -1 | -25 |
| **30-40** | **24** | **35 (A)** | **0** | **0** |
| 40-50 | 10 | 45 | 1 | 10 |
| 50-60 | 33 | 55 | 2 | 66 |
| 60-70 | 71 | 65 | 3 | 213 |
| 70-80 | 51 | 75 | 4 | 204 |
| **Total** | $\mathbf{N=249}$ | | | $\sum fd' = \mathbf{383}$ |

$$\bar{X} = A + \left(\frac{\sum fd'}{N}\right) \times h$$
$$\bar{X} = 35 + \left(\frac{383}{249}\right) \times 10$$
$$\bar{X} = 35 + 1.53815 \times 10 = 35 + 15.3815 \approx \mathbf{50.38}$$

**The Mean is 50.38 marks.**

---

### Step 3: Calculate Median ($Q_2$), Lower Quartile ($Q_1$), and Upper Quartile ($Q_3$)

We use the c.f. table, where $N=249$. The formula for quartiles/median is:
$$Q_k = L + \frac{\frac{kN}{4} - \text{c.f.}_{\text{preceding}}}{f_{Qk}} \times h$$

| Class | $f$ | c.f. |
| :---: | :-: | :-: |
| 0-10 | 15 | 15 |
| 10-20 | 20 | 35 |
| 20-30 | 25 | 60 |
| 30-40 | 24 | 84 |
| 40-50 | 10 | 94 |
| 50-60 | 33 | 127 |
| **60-70** | **71** | **198** |
| 70-80 | 51 | 249 |

#### A. Lower Quartile ($Q_1$)
* **Position:** $N/4 = 249/4 = 62.25$.
* **$Q_1$ Class:** The class where c.f. is first greater than 62.25 is **30-40**.
* **Parameters:** $L=30$, $\text{c.f.}_{\text{preceding}}=60$, $f_{Q1}=24$, $h=10$.
$$Q_1 = 30 + \frac{62.25 - 60}{24} \times 10$$
$$Q_1 = 30 + \frac{2.25}{24} \times 10 = 30 + 0.9375 \approx \mathbf{30.94}$$

#### B. Median ($Q_2$)
* **Position:** $2N/4 = N/2 = 249/2 = 124.5$.
* **Median Class:** The class where c.f. is first greater than 124.5 is **50-60**.
* **Parameters:** $L=50$, $\text{c.f.}_{\text{preceding}}=94$, $f_{Q2}=33$, $h=10$.
$$Q_2 = 50 + \frac{124.5 - 94}{33} \times 10$$
$$Q_2 = 50 + \frac{30.5}{33} \times 10 = 50 + 9.2424 \approx \mathbf{59.24}$$

#### C. Upper Quartile ($Q_3$)
* **Position:** $3N/4 = 3(249)/4 = 186.75$.
* **$Q_3$ Class:** The class where c.f. is first greater than 186.75 is **60-70**.
* **Parameters:** $L=60$, $\text{c.f.}_{\text{preceding}}=127$, $f_{Q3}=71$, $h=10$.
$$Q_3 = 60 + \frac{186.75 - 127}{71} \times 10$$
$$Q_3 = 60 + \frac{59.75}{71} \times 10 = 60 + 8.4155 \approx \mathbf{68.42}$$

---

### Final Results
* **Mean ($\bar{X}$):** $\mathbf{50.38}$ marks
* **Lower Quartile ($Q_1$):** $\mathbf{30.94}$ marks
* **Median ($Q_2$):** $\mathbf{59.24}$ marks
* **Upper Quartile ($Q_3$):** $\mathbf{68.42}$ marks

## 26. Determine Missing Frequencies using the Median Formula 🧩

The goal is to find the two missing frequencies ($f_3$ and $f_5$) in the incomplete frequency distribution, given that the **median is 46** and the total frequency is $N=229$.

| Variable | 10-20 | 20-30 | 30-40 | 40-50 | 50-60 | 60-70 | 70-80 | Total |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| Frequency ($f$) | 12 | 30 | $f_3$ | 65 | $f_5$ | 25 | 18 | 229 |

### Step 1: Set up the Cumulative Frequency (c.f.) and the Total Frequency Equation

Let $f_3 = x$ and $f_5 = y$.

| Class | Frequency ($f$) | Cumulative Frequency (c.f.) |
| :---: | :---: | :---: |
| 10-20 | 12 | 12 |
| 20-30 | 30 | 42 |
| 30-40 | $x$ | $42 + x$ |
| **40-50** | **65** | **$107 + x$** |
| 50-60 | $y$ | $107 + x + y$ |
| 60-70 | 25 | $132 + x + y$ |
| 70-80 | 18 | $150 + x + y$ |

The total frequency is given as 229.
$$\sum f = 150 + x + y = 229$$
$$x + y = 229 - 150$$
$$\mathbf{x + y = 79} \quad \text{(Equation 1)}$$

---

### Step 2: Use the Median Formula to find the value of $x$

Given that the **Median ($M$) is 46**. Since 46 falls in the class **40-50**, this is the **Median Class**.

The formula for the median is:
$$M = L + \frac{\frac{N}{2} - \text{c.f.}_{\text{preceding}}}{f_M} \times h$$

Where:
* $M = 46$
* $L$ (Lower boundary of median class) $= \mathbf{40}$
* $N/2 = 229 / 2 = \mathbf{114.5}$
* $\text{c.f.}_{\text{preceding}}$ (c.f. of preceding class) $= \mathbf{42 + x}$
* $f_M$ (Frequency of median class) $= \mathbf{65}$
* $h$ (Class width) $= 50 - 40 = \mathbf{10}$

Substitute these values into the formula:
$$46 = 40 + \frac{114.5 - (42 + x)}{65} \times 10$$
$$46 - 40 = \frac{114.5 - 42 - x}{65} \times 10$$
$$6 = \frac{72.5 - x}{65} \times 10$$

Now, solve for $x$:
$$6 \times 65 = (72.5 - x) \times 10$$
$$390 = 725 - 10x$$
$$10x = 725 - 390$$
$$10x = 335$$
$$\mathbf{x = 33.5}$$

Since frequency must be an integer, we take $x = \mathbf{34}$ (this is a common situation in textbook problems where the calculated frequency is rounded to the nearest integer).

---

### Step 3: Find the value of $y$

Substitute the value of $x=34$ back into Equation 1:
$$x + y = 79$$
$$34 + y = 79$$
$$y = 79 - 34$$
$$\mathbf{y = 45}$$

### Final Answer:

The missing frequencies are:
* $f_3$ (Frequency of 30-40 class) $\approx \mathbf{34}$
* $f_5$ (Frequency of 50-60 class) $= \mathbf{45}$

## 27\. Check the Consistency of the Consumption Data 🍎🍊

Consistency in statistical data is measured using the **Coefficient of Variation (C.V.)**. The series with the **lower C.V.** is considered **more consistent** (less variable).

The formula for C.V. is:
$$\text{C.V.} = \frac{\text{Standard Deviation}(\sigma)}{\text{Mean}(\bar{X})} \times 100$$

### 1\. Calculations for Guavas (Series X)

  * Data ($X$): 3, 5, 6, 4, 3, 5, 4
  * $N = 7$

| $X$ | $X^2$ |
| :-: | :---: |
| 3 | 9 |
| 5 | 25 |
| 6 | 36 |
| 4 | 16 |
| 3 | 9 |
| 5 | 25 |
| 4 | 16 |
| $\sum X = \mathbf{30}$ | $\sum X^2 = \mathbf{136}$ |

**Mean ($\bar{X}$):**
$$\bar{X} = \frac{\sum X}{N} = \frac{30}{7} \approx 4.286$$

**Standard Deviation ($\sigma_X$):**
$$\sigma_X = \sqrt{\frac{\sum X^2}{N} - \bar{X}^2}$$
$$\sigma_X = \sqrt{\frac{136}{7} - (4.286)^2} \approx \sqrt{19.4286 - 18.3697} \approx \sqrt{1.0589} \approx 1.030$$

**Coefficient of Variation ($\text{C.V.}_X$):**
$$\text{C.V.}_X = \frac{1.030}{4.286} \times 100 \approx \mathbf{24.04\%}$$

-----

### 2\. Calculations for Oranges (Series Y)

  * Data ($Y$): 1, 3, 7, 9, 2, 6, 2
  * $N = 7$

| $Y$ | $Y^2$ |
| :-: | :---: |
| 1 | 1 |
| 3 | 9 |
| 7 | 49 |
| 9 | 81 |
| 2 | 4 |
| 6 | 36 |
| 2 | 4 |
| $\sum Y = \mathbf{30}$ | $\sum Y^2 = \mathbf{184}$ |

**Mean ($\bar{Y}$):**
$$\bar{Y} = \frac{\sum Y}{N} = \frac{30}{7} \approx 4.286$$

**Standard Deviation ($\sigma_Y$):**
$$\sigma_Y = \sqrt{\frac{\sum Y^2}{N} - \bar{Y}^2}$$
$$\sigma_Y = \sqrt{\frac{184}{7} - (4.286)^2} \approx \sqrt{26.2857 - 18.3697} \approx \sqrt{7.916} \approx 2.814$$

**Coefficient of Variation ($\text{C.V.}_Y$):**
$$\text{C.V.}_Y = \frac{2.814}{4.286} \times 100 \approx \mathbf{65.66\%}$$

-----

### 3\. Conclusion on Consistency

| Item | Mean ($\bar{X}$) | Standard Deviation ($\sigma$) | C.V. |
| :---: | :---: | :---: | :---: |
| Guavas | 4.286 | 1.030 | **24.04%** |
| Oranges | 4.286 | 2.814 | **65.66%** |

Since the **Coefficient of Variation for Guavas (24.04%) is significantly lower** than the Coefficient of Variation for Oranges (65.66%), the consumption of **Guavas is more consistent** than the consumption of Oranges.


The next question in your list is **Question 28**.

## 28. Prove the Frequency Distribution Curve is Leptokurtic 🏔️

To prove that the frequency distribution is **leptokurtic**, we must calculate the **Coefficient of Kurtosis ($\beta_2$)** and show that it is greater than 3 ($\beta_2 > 3$).

|**Class**|**Frequency (f)**|
|---|---|
|10-15|1|
|15-20|4|
|20-25|8|
|25-30|19|
|30-35|35|
|35-40|20|
|40-45|7|
|45-50|5|
|50-55|1|

### Step 1: Calculate Moments About an Assumed Mean ($A$)

We use the **step deviation method** to find the second ($\mu_2$) and fourth ($\mu_4$) central moments.

Let the Assumed Mean $A$ be the midpoint of the class 30-35: $A = 32.5$.

The class width is $h = 5$.

Let $d' = \frac{X - 32.5}{5}$.

|**Class**|**f**|**Midpoint (X)**|**d′**|**fd′**|**fd′2**|**fd′3**|**fd′4**|
|---|---|---|---|---|---|---|---|
|10-15|1|12.5|-4|-4|16|-64|256|
|15-20|4|17.5|-3|-12|36|-108|324|
|20-25|8|22.5|-2|-16|32|-64|128|
|25-30|19|27.5|-1|-19|19|-19|19|
|**30-35**|**35**|**32.5 (A)**|**0**|**0**|**0**|**0**|**0**|
|35-40|20|37.5|1|20|20|20|20|
|40-45|7|42.5|2|14|28|56|112|
|45-50|5|47.5|3|15|45|135|405|
|50-55|1|52.5|4|4|16|64|256|
|**Total**|$\mathbf{N=100}$|||$\sum fd' = \mathbf{2}$|$\sum fd'^2 = \mathbf{212}$|$\sum fd'^3 = \mathbf{22}$|$\sum fd'^4 = \mathbf{1520}$|

#### Moments about $A$ (in units of $d'$):

- $\mu'_1 = c = \frac{\sum fd'}{N} = \frac{2}{100} = 0.02$
    
- $\mu'_2 = \frac{\sum fd'^2}{N} = \frac{212}{100} = 2.12$
    
- $\mu'_4 = \frac{\sum fd'^4}{N} = \frac{1520}{100} = 15.20$
    

---

### Step 2: Convert to Central Moments ($\mu_2$ and $\mu_4$)

#### 1. Second Central Moment ($\mu_2$)

$$\mu_2 = h^2 [\mu'_2 - c^2]$$

$$\mu_2 = 5^2 [2.12 - (0.02)^2] = 25 [2.12 - 0.0004]$$

$$\mu_2 = 25 \times 2.1196 = \mathbf{52.99}$$

#### 2. Fourth Central Moment ($\mu_4$)

$$\mu_4 = h^4 [\mu'_4 - 4\mu'_3 c + 6\mu'_2 c^2 - 3c^4]$$

We need $\mu'_3$: $\mu'_3 = \frac{\sum fd'^3}{N} = \frac{22}{100} = 0.22$

$$\mu_4 = 5^4 [15.20 - 4(0.22)(0.02) + 6(2.12)(0.02)^2 - 3(0.02)^4]$$

$$\mu_4 = 625 [15.20 - 0.0176 + 0.005088 - 0.00000048]$$

$$\mu_4 = 625 \times 15.18748752 \approx \mathbf{9492.1797}$$

---

### Step 3: Calculate the Coefficient of Kurtosis ($\beta_2$)

$$\beta_2 = \frac{\mu_4}{\mu_2^2}$$

$$\beta_2 = \frac{9492.1797}{(52.99)^2} = \frac{9492.1797}{2807.9401} \approx \mathbf{3.379}$$

### Conclusion

Since the **Coefficient of Kurtosis ($\beta_2 \approx 3.379$) is greater than 3**, the frequency distribution curve is indeed **leptokurtic**.


The next question in your list is **Question 29**. This question has two parts, (a) and (b).

## 29. Test of Skewness and Kurtosis (Two Parts) 🧪

### Part (a): Central Moments Given

The first four **central moments** (moments about the mean, $\mu_k$) are given:
$$\mu_1 = 0, \quad \mu_2 = 2.3, \quad \mu_3 = 0.9, \quad \mu_4 = 15.65$$

#### 1. Test of Skewness

We use the moment coefficient of skewness, $\beta_1$:
$$\beta_1 = \frac{\mu_3^2}{\mu_2^3}$$
$$\beta_1 = \frac{(0.9)^2}{(2.3)^3} = \frac{0.81}{12.167} \approx \mathbf{0.0666}$$

Since $\beta_1 > 0$, the distribution is **positively skewed**.

#### 2. Test of Kurtosis

We use the moment coefficient of kurtosis, $\beta_2$:
$$\beta_2 = \frac{\mu_4}{\mu_2^2}$$
$$\beta_2 = \frac{15.65}{(2.3)^2} = \frac{15.65}{5.29} \approx \mathbf{2.958}$$

#### 3. Discuss the Nature of the Curve

* **Skewness:** Since $\beta_1$ is a small positive value ($0.0666$), the distribution is slightly **Positively Skewed** (long right tail).
* **Kurtosis:** Since $\beta_2$ is less than 3 ($2.958 < 3$), the distribution is **Platykurtic** (flatter peak and thinner tails than a normal distribution).

***

### Part (b): Moments About an Arbitrary Point ($A=4$)

The first four moments about $x=4$ ($\mu'_k$) are:
$$\mu'_1 = c = 1, \quad \mu'_2 = 4, \quad \mu'_3 = 10, \quad \mu'_4 = 45$$

#### 1. Calculate Moments About the Mean ($\mu_k$)

We use $c = \mu'_1 = 1$.

* $\mu_1 = 0$
* $\mu_2 = \mu'_2 - c^2 = 4 - (1)^2 = \mathbf{3}$
* $\mu_3 = \mu'_3 - 3\mu'_2 c + 2c^3 = 10 - 3(4)(1) + 2(1)^3 = 10 - 12 + 2 = \mathbf{0}$
* $\mu_4 = \mu'_4 - 4\mu'_3 c + 6\mu'_2 c^2 - 3c^4 = 45 - 4(10)(1) + 6(4)(1)^2 - 3(1)^4 = 45 - 40 + 24 - 3 = \mathbf{26}$

#### 2. Calculate Characteristics

* **Mean ($\bar{X}$):** $\bar{X} = A + c = 4 + 1 = \mathbf{5}$
* **Variance ($\sigma^2$):** $\mu_2 = \mathbf{3}$
* **Standard Deviation ($\sigma$):** $\sqrt{\mu_2} = \sqrt{3} \approx \mathbf{1.732}$

#### 3. Comment upon the Nature of the Distribution

* **Skewness ($\beta_1$):**
    $$\beta_1 = \frac{\mu_3^2}{\mu_2^3} = \frac{0^2}{3^3} = \mathbf{0}$$
    Since $\beta_1 = 0$, the distribution is **Symmetrical**.

* **Kurtosis ($\beta_2$):**
    $$\beta_2 = \frac{\mu_4}{\mu_2^2} = \frac{26}{3^2} = \frac{26}{9} \approx \mathbf{2.889}$$
    Since $\beta_2 < 3$, the distribution is **Platykurtic**.

|    Characteristic     |   Value   | Comment on Nature |
| :-------------------: | :-------: | :---------------: |
|   Mean ($\bar{X}$)    |   **5**   |                   |
| Variance ($\sigma^2$) |   **3**   |                   |
|        $\mu_3$        |   **0**   |                   |
| $\beta_1$ (Skewness)  |   **0**   |  **Symmetrical**  |
| $\beta_2$ (Kurtosis)  | **2.889** |  **Platykurtic**  |

The next and final question in your list is **Question 30**.

## 30. Calculate Bowley's Coefficient of Skewness 📏

To calculate **Bowley's Coefficient of Skewness** ($S_B$), we need to find the lower quartile ($Q_1$), the median ($Q_2$), and the upper quartile ($Q_3$).

The formula is:
$$S_B = \frac{Q_3 + Q_1 - 2Q_2}{Q_3 - Q_1}$$

### Step 1: Prepare the Cumulative Frequency Table

| Distance (km) | Frequency ($f$) | Cumulative Frequency (c.f.) |
| :---: | :-: | :---: |
| 0-10 | 2 | 2 |
| 10-20 | 5 | 7 |
| 20-30 | 10 | 17 |
| **30-40** | **15** | **32** |
| 40-50 | 10 | 42 |
| 50-60 | 4 | 46 |
| 60-70 | 1 | 47 |
| **Total** | $\mathbf{N=47}$ | |

---

### Step 2: Calculate Quartiles ($Q_1, Q_2, Q_3$)

The general formula for quartiles is:
$$Q_k = L + \frac{\frac{kN}{4} - \text{c.f.}_{\text{preceding}}}{f_{Qk}} \times h$$
The total frequency is $N=47$, and the class width $h=10$.

#### A. Lower Quartile ($Q_1$)
* **Position:** $N/4 = 47/4 = \mathbf{11.75}$
* **$Q_1$ Class:** $20-30$ (c.f. is 17)
* **Parameters:** $L=20$, $\text{c.f.}_{\text{preceding}}=7$, $f_{Q1}=10$, $h=10$.
$$Q_1 = 20 + \frac{11.75 - 7}{10} \times 10 = 20 + 4.75 = \mathbf{24.75}$$

#### B. Median ($Q_2$)
* **Position:** $2N/4 = N/2 = 47/2 = \mathbf{23.5}$
* **$Q_2$ Class:** $30-40$ (c.f. is 32)
* **Parameters:** $L=30$, $\text{c.f.}_{\text{preceding}}=17$, $f_{Q2}=15$, $h=10$.
$$Q_2 = 30 + \frac{23.5 - 17}{15} \times 10 = 30 + \frac{6.5}{15} \times 10$$
$$Q_2 = 30 + 4.3333 \approx \mathbf{34.33}$$

#### C. Upper Quartile ($Q_3$)
* **Position:** $3N/4 = 3(47)/4 = \mathbf{35.25}$
* **$Q_3$ Class:** $30-40$ (c.f. is 32)
* **Parameters:** $L=30$, $\text{c.f.}_{\text{preceding}}=17$, $f_{Q3}=15$, $h=10$.
$$Q_3 = 30 + \frac{35.25 - 17}{15} \times 10 = 30 + \frac{18.25}{15} \times 10$$
$$Q_3 = 30 + 12.1667 \approx \mathbf{42.17}$$

---

### Step 3: Calculate Bowley's Coefficient of Skewness ($S_B$)

Substitute the quartile values into the formula: $Q_1 = 24.75, Q_2 = 34.33, Q_3 = 42.17$.

$$S_B = \frac{Q_3 + Q_1 - 2Q_2}{Q_3 - Q_1}$$
$$S_B = \frac{42.17 + 24.75 - 2(34.33)}{42.17 - 24.75}$$
$$S_B = \frac{66.92 - 68.66}{17.42}$$
$$S_B = \frac{-1.74}{17.42} \approx \mathbf{-0.0999}$$

**Bowley's Coefficient of Skewness is approximately -0.10.** Since the value is negative, the distribution is slightly **negatively skewed**.