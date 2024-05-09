# Assignment 1

---

## 1. Student Background Survey (20 points)

To help tailor and schedule the upcoming lessons for this semester, it's essential to understand your background and preferences. Kindly take a few moments to complete the survey through the provided link: [Student Background Survey](https://docs.google.com/forms/d/e/1FAIpQLScQ5uSQBoUiqZ6abyXdyibioebLrTaOPCUEaRVIthc8mAimAQ/viewform?usp=sf_link)

---

## 2. Interquartile Range (IQR) (10 points)

Explain how to use the IQR to screen for outliers in a data set.

### Answer

The Interquartile Range (IQR) is a measure of statistical dispersion. It represents the range within which the central 50% of the values lie in a data set. It is calculated as the difference between the 75th percentile (Q3) and the 25th percentile (Q1):

$$\text{IQR} = Q3 - Q1 $$

The IQR can be used to screen for outliers by identifying values that lie outside of the "inner fences" defined by the following boundaries:

1. **Lower Boundary:**

$$Q1 - 1.5 \times \text{IQR} $$

2. **Upper Boundary:**

$$Q3 + 1.5 \times \text{IQR} $$

Any data point that falls below the lower boundary or above the upper boundary can be considered an outlier.

## 3. Teaching Assistant Ratings Analysis (12 points)

The table below contains ratings for courses at a university. (_Note_: Only a subset of rows is displayed for brevity.)

| id  | instructor | course | semester | size | rating |
| --- | ---------- | ------ | -------- | ---- | ------ |
| 1   | 3          | 5      | 2        | 15   | 2      |
| 2   | 15         | 17     | 1        | 28   | 3      |
| 3   | 22         | 3      | 3        | 23   | 2      |
| 4   | 5          | 1      | 2        | 12   | 1      |
| 5   | 7          | 21     | 1        | 24   | 3      |
| 6   | 23         | 11     | 2        | 16   | 2      |
| 7   | 3          | 22     | 3        | 29   | 1      |
| 8   | 10         | 3      | 1        | 14   | 3      |
| 9   | 12         | 3      | 3        | 18   | 3      |
| 10  | 15         | 2      | 2        | 25   | 2      |
| 11  | 9          | 11     | 1        | 22   | 3      |
| 12  | 13         | 3      | 3        | 27   | 1      |
| 13  | 11         | 17     | 2        | 20   | 2      |
| 14  | 6          | 21     | 3        | 19   | 3      |
| 15  | 16         | 5      | 1        | 13   | 3      |
| 16  | 6          | 1      | 2        | 26   | 2      |
| 17  | 14         | 17     | 3        | 21   | 3      |
| 18  | 22         | 22     | 1        | 17   | 1      |
| 19  | 11         | 2      | 3        | 11   | 3      |

Classify each attribute as nominal or ordinal (2 points/each):

### Answer

- **id** - Unique identifier for each rating: **nominal**
- **instructor** - ID that identifies the instructor: **nominal**
- **course** - ID identifying the course: **nominal**
- **semester** - 1 = summer, 2 = fall, 3 = winter: **ordinal**
- **size** - Number of students in the class: **numeric** (The points for this question won't be included in your grade).
- **rating** - 1 = low, 2 = medium, 3 = high: **ordinal**

---

## 4. Hospital Age and Body Fat Study (34 points)

A hospital tested age and body fat data for 18 randomly selected adults. The results are presented below:

|  | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Age | 23 | 23 | 27 | 27 | 39 | 41 | 47 | 49 | 50 | 52 | 54 | 54 | 56 | 57 | 58 | 58 | 60 | 61 |
| %fat | 9.5 | 26.5 | 7.8 | 17.8 | 31.4 | 25.9 | 27.4 | 27.2 | 31.2 | 34.6 | 42.5 | 28.8 | 33.4 | 30.2 | 34.1 | 32.9 | 41.2 | 35.7 |

Tasks:

- Compute the min, Q_1 mean, median, Q_3, max, and standard deviation for age and %fat (2 points/each).

|      | min | Q_1 | median | Q_3 | max | mean | standard deviation |
| ---- | --- | --- | ------ | --- | --- | ---- | ------------------ |
| Age  |     |     |        |     |     |      |                    |
| %fat |     |     |        |     |     |      |                    |

- Calculate the covariance and correlation coefficient (Pearson’s) for the two attributes and detail the calculation process. Are these attributes positively or negatively correlated? (10 points/each)

### Answer

#### Basic Statistics

- **Minimum (`min`)**: Smallest value in the dataset.
- **Maximum (`max`)**: Largest value in the dataset.
- **Mean**: The average of the dataset.$\mu = \frac{\sum x}{n}$
- **First Quartile (Q1)**: is defined as the middle number between the smallest number (minimum) and the median of the data set. It is also known as the lower quartile, as 25% of the data is below this point.
- **Median (Q2)**: is the median of a data set; thus 50% of the data lies below this point.
- **Third Quartile (Q3)**: is the middle value between the median and the highest value (maximum) of the data set. It is known as the upper quartile, as 75% of the data lies below this point.
- **Standard Deviation**:$\sigma = \sqrt{\frac{\sum (x - \mu)^2}{n}}$

##### For `age`

- $\min = 23$,
- $\max = 61$,
- $\mu = \frac{sum(age)}{18} = 46.44444444444444$,
- $Q1 = 39$
- $Median = 51$
- $Q3 = 57$
- $\sigma = 12.846193652519204$

##### For `fat`

- $\min = 7.8$,
- $\max = 42.5$,
- $\mu = \frac{sum(fat)}{18} = 28.783333333333328$,
- $Q1 = 26.5$
- $Median = 30.7$
- $Q3 = 34.1$
- $\sigma = 8.993655170915401$

#### Covariance & Correlation

- **Covariance**:

  $$\text{Cov}(X, Y) = \frac{\sum (x_i - \mu_x)(y_i - \mu_y)}{n}$$

- **Correlation Coefficient**:

  $$r = \frac{\text{Cov}(X, Y)}{\sigma_x \times \sigma_y}$$

  - $\text{Cov}(age, fat) = 94.46296296296327$,
  - $r(age, fat) = 0.8176187964565875$,

#### Using python package

```python
import numpy as np

# Data
age = [23, 23, 27, 27, 39, 41, 47, 49, 50, 52, 54, 54, 56, 57, 58, 58, 60, 61]
fat = [
    9.5,
    26.5,
    7.8,
    17.8,
    31.4,
    25.9,
    27.4,
    27.2,
    31.2,
    34.6,
    42.5,
    28.8,
    33.4,
    30.2,
    34.1,
    32.9,
    41.2,
    35.7,
]

# Age
print("Minimum Age:", np.min(age))
print("Maximum Age:", np.max(age))
print("Mean Age:", np.mean(age))
print("Q1 Age:", np.quantile(age, 0.25, method="averaged_inverted_cdf"))
print("Median Age:", np.quantile(age, 0.5, method="averaged_inverted_cdf"))
print("Q3 Age:", np.quantile(age, 0.75, method="averaged_inverted_cdf"))
print("Standard Deviation Age:", np.std(age))

# Fat%
print("Minimum Fat:", np.min(fat))
print("Maximum Fat:", np.max(fat))
print("Mean Fat:", np.mean(fat))
print("Q1 Fat:", np.quantile(fat, 0.25, method="averaged_inverted_cdf"))
print("Median Fat:", np.quantile(fat, 0.5, method="averaged_inverted_cdf"))
print("Q3 Fat:", np.quantile(fat, 0.75, method="averaged_inverted_cdf"))
print("Standard Deviation Fat:", np.std(fat))

# Covariance & Correlation
cov_matrix = np.cov(age, fat, bias=True)
cor_matrix = np.corrcoef(age, fat)

print("Covariance:", cov_matrix[0][1])
print("Correlation Coefficient:", cor_matrix[0][1])
```

##### Output

```bash
Minimum Age: 23
Maximum Age: 61
Mean Age: 46.44444444444444
Q1 Age: 39.0
Median Age: 51.0
Q3 Age: 57.0
Standard Deviation Age: 12.846193652519204
Minimum Fat: 7.8
Maximum Fat: 42.5
Mean Fat: 28.783333333333335
Q1 Fat: 26.5
Median Fat: 30.7
Q3 Fat: 34.1
Standard Deviation Fat: 8.993655170915401
Covariance: 94.46296296296295
Correlation Coefficient: 0.8176187964565875
```

---

## 5. Dissimilarity Computations (24 points)

Briefly outline how to compute the dissimilarity between objects described by the following (6 points/each):

- (a) Nominal attributes
- (b) Asymmetric binary attributes
- (c) Numeric attributes
- (d) Term-frequency vectors

---

### Answer

#### (a) Nominal attributes

For objects described by nominal attributes, a simple method to compute dissimilarity is to use a matching coefficient:

$$d(i, j) = \frac{p - m}{p}$$

Where:

- $d(i, j)$ is the dissimilarity between objects $i$ and $j$.
- $p$ is the total number of attributes.
- $m$ is the number of matching attributes between objects $i$ and $j$.

#### (b) Asymmetric binary attributes

For asymmetric binary attributes, the following method is often used to measure dissimilarity:

$$d(i, j) = \frac{r+s}{q + r + s}$$

Where:

- $q$ is the number of attributes where both objects have a value of 1.
- $r$ is the number of attributes where the first object has a 1 and the second has a 0.
- $s$ is the number of attributes where the first object has a 0 and the second has a 1.

#### (c) Numeric attributes

For numeric attributes, several distance measures are commonly used:

1. Manhattan Distance (L1 norm or City-block distance)

$$d(i, j) = \sum_{k=1}^{p} |x_{ik} - x_{jk}|$$

2. Euclidean Distance (L2 norm)

$$d(i, j) = \sqrt{\sum_{k=1}^{p} (x_{ik} - x_{jk})^2}$$

3. Minkowski Distance (Lp norm)

$$d(i, j) = \left( \sum_{k=1}^{p} |x_{ik} - x_{jk}|^h \right)^{\frac{1}{h}}$$

Where:

- $x_{ik}$ is the value of the $kth$ attribute for the $ith$ object.
- $x_{jk}$ is the value of the $kth$ attribute for the $jth$ object.
- $p$ is the number of attributes.
- $h$ is a parameter that determines the order of the norm. When $h = 1$, it becomes Manhattan distance, and when $h = 2$, it becomes Euclidean distance. The Minkowski distance generalizes these and other norms.

#### (d) Term-frequency vectors

For term-frequency vectors (commonly used in text processing), the cosine similarity is often employed. Dissimilarity can then be derived as:

$$d(i, j) = 1 - \frac{\sum_{k=1}^{p} x_{ik} \times x_{jk}}{\sqrt{\sum_{k=1}^{p} x_{ik}^2} \times \sqrt{\sum_{k=1}^{p} x_{jk}^2}}$$

Where:

- $x_{ik}$ represents the frequency of term $k$ in document $i$.
- $x_{jk}$ represents the frequency of term $k$ in document $j$.
- $p$ is the number of terms.

[test](../assets/data/streamflow.csv) [test1](../assets/data/cars93.csv)
