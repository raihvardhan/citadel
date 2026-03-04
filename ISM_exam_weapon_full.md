
# ISM Final Exam Weapon – Full Questions and Solutions

Based on patterns from ISM exams and methods from the Anderson textbook.

Referenced Book:
Statistics for Business and Economics (Anderson et al.)

Chapter references:
- Ch 3: Descriptive Statistics & Correlation
- Ch 6: Continuous Probability Distributions
- Ch 8: Confidence Intervals
- Ch 9: Hypothesis Testing
- Ch 10: Two-Population Inference
- Ch 13: ANOVA
- Ch 14: Regression
- Ch 17: Time Series Forecasting

---

# Question 1 – Karl Pearson Correlation

Temperature vs Electricity data

| Temperature | Electricity |
|---|---|
30 | 220 |
32 | 240 |
35 | 260 |
37 | 300 |
33 | 250 |

Mean temperature = 33.4
Mean electricity = 254

Formula

r = Sum[(x - x_bar)(y - y_bar)] / sqrt( Sum[(x - x_bar)^2] * Sum[(y - y_bar)^2] )

Final result

r ≈ 0.973

Interpretation: very strong positive correlation.

---

# Question 2 – Exponential Smoothing

Demand data

|Month|Demand|
|---|---|
Jan|120
Feb|135
Mar|150
Apr|160
May|155
Jun|170

Initial forecast = 120

Formula

F(t+1) = alpha*Yt + (1-alpha)*Ft

Forecast July

alpha = 0.4 → 157.53

alpha = 0.7 → 165.52

---

# Question 3 – Paired t Test

Before vs After scores

|Student|Before|After|
|---|---|---|
1|60|65
2|62|66
3|58|63
4|64|67
5|59|63
6|61|65

Differences = 5,4,5,3,4,4

Mean difference = 4.167

t ≈ 13.56

Reject H0 → improvement confirmed.

---

# Question 4 – ANOVA

|A|B|C|
|---|---|---|
5|8|10
6|9|11
4|7|9

F statistic = 19

Reject H0 → fertilizers differ.

---

# Question 5 – Regression

|X|Y|
|---|---|
2|4
4|5
6|7
8|10
10|11

Regression equation

Y = 1.7 + 0.95X

Prediction at X=9 → 10.25

---

# Question 6 – Gaussian Mixture

Component 1 mean = 22 variance = 12
Component 2 mean = 40 variance = 15

Observation x=25 → component 1 more likely.

---

# Question 7 – Confidence Interval

n = 20
mean = 110
sd = 12

CI = (104.38 , 115.62)

---

# Question 8 – Two Proportion Test

City A = 180/300 = 0.60
City B = 135/250 = 0.54

z ≈ 1.42

Fail to reject H0.
