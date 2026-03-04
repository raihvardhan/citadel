
# ISM Final Exam Weapon — Q1–Q8 (Clean Markdown with Proper Math)

---

# Q1 — Karl Pearson’s coefficient of correlation

## Question

Temperature vs electricity usage:

| Temperature X (°C) | Electricity Y (kWh) |
|---|---|
|30|220|
|32|240|
|35|260|
|37|300|
|33|250|

---

## Compute means

$$
\bar{x} =
\frac{30+32+35+37+33}{5}
=
33.4
$$

$$
\bar{y} =
\frac{220+240+260+300+250}{5}
=
254
$$

---

## Deviation table

| x | y | x- x̄ | y- ȳ | (x-x̄)(y-ȳ) | (x-x̄)^2 | (y-ȳ)^2 |
|---|---|---|---|---|---|---|
|30|220|-3.4|-34|115.6|11.56|1156|
|32|240|-1.4|-14|19.6|1.96|196|
|35|260|1.6|6|9.6|2.56|36|
|37|300|3.6|46|165.6|12.96|2116|
|33|250|-0.4|-4|1.6|0.16|16|

Totals

$$
\sum (x-\bar{x})(y-\bar{y}) = 312
$$

$$
\sum (x-\bar{x})^2 = 29.2
$$

$$
\sum (y-\bar{y})^2 = 3520
$$

---

## Pearson correlation

$$
r =
\frac{\sum (x-\bar{x})(y-\bar{y})}
{\sqrt{\sum (x-\bar{x})^2 \sum (y-\bar{y})^2}}
$$

$$
r =
\frac{312}
{\sqrt{29.2 \times 3520}}
$$

$$
29.2 \times 3520 = 102784
$$

$$
\sqrt{102784} \approx 320.807
$$

$$
r =
\frac{312}{320.807}
\approx
0.973
$$

Interpretation: very strong positive correlation.

---

# Q2 — Simple Exponential Smoothing

Demand data

|Month|Demand|
|---|---|
|Jan|120|
|Feb|135|
|Mar|150|
|Apr|160|
|May|155|
|Jun|170|

Initial forecast

$$
F_1 = Y_1 = 120
$$

Forecast formula

$$
F_{t+1} = \alpha Y_t + (1-\alpha)F_t
$$

---

## Case 1: α = 0.4

$$
F_2 = 0.4(120)+0.6(120)=120
$$

$$
F_3 = 0.4(135)+0.6(120)=126
$$

$$
F_4 = 0.4(150)+0.6(126)=135.6
$$

$$
F_5 = 0.4(160)+0.6(135.6)=145.36
$$

$$
F_6 = 0.4(155)+0.6(145.36)=149.216
$$

$$
F_7 = 0.4(170)+0.6(149.216)=157.53
$$

Forecast July ≈ **157.53**

---

## Case 2: α = 0.7

$$
F_2 = 120
$$

$$
F_3 = 0.7(135)+0.3(120)=130.5
$$

$$
F_4 = 0.7(150)+0.3(130.5)=144.15
$$

$$
F_5 = 0.7(160)+0.3(144.15)=155.245
$$

$$
F_6 = 0.7(155)+0.3(155.245)=155.07
$$

$$
F_7 = 0.7(170)+0.3(155.07)=165.52
$$

Forecast July ≈ **165.52**

Higher α responds faster to spikes.

---

# Q3 — Paired t Test

|Student|Before|After|
|---|---|---|
|1|60|65|
|2|62|66|
|3|58|63|
|4|64|67|
|5|59|63|
|6|61|65|

Differences

$$
d = [5,4,5,3,4,4]
$$

Sample size

$$
n = 6
$$

Mean difference

$$
\bar{d} = \frac{25}{6} = 4.167
$$

Standard deviation

$$
s_d = 0.753
$$

Test statistic

$$
t =
\frac{\bar{d}}{s_d/\sqrt{n}}
\approx
13.56
$$

Reject \(H_0\). Strategy improves performance.

---

# Q4 — One‑Way ANOVA

|A|B|C|
|---|---|---|
|5|8|10|
|6|9|11|
|4|7|9|

Group means

A = 5  
B = 8  
C = 10

Grand mean

$$
\bar{y} = 7.667
$$

Between variation

$$
SS_{Tr} = 38
$$

Within variation

$$
SSE = 6
$$

Mean squares

$$
MS_{Tr} = 19
$$

$$
MS_E = 1
$$

F statistic

$$
F = 19
$$

Reject \(H_0\). Fertilizers differ.

---

# Q5 — Linear Regression

|X|Y|
|---|---|
|2|4|
|4|5|
|6|7|
|8|10|
|10|11|

Means

$$
\bar{x}=6,\quad \bar{y}=7.4
$$

Slope

$$
\hat{\beta}_1 =
\frac{38}{40}
=
0.95
$$

Intercept

$$
\hat{\beta}_0 =
1.7
$$

Regression model

$$
\hat{Y}
=
1.7 + 0.95X
$$

Prediction for \(X=9\)

$$
\hat{Y}=10.25
$$

Coefficient of determination

$$
R^2 \approx 0.97
$$

---

# Q6 — Gaussian Mixture Model

Component 1

$$
\mu_1=22,\quad \sigma_1^2=12
$$

Component 2

$$
\mu_2=40,\quad \sigma_2^2=15
$$

Mixture density

$$
f(x)=0.5\phi(x|\mu_1,\sigma_1^2)+0.5\phi(x|\mu_2,\sigma_2^2)
$$

Observation \(x=25\) is closer to \(22\), so it likely belongs to **Component 1**.

---

# Q7 — Confidence Interval

Given

$$
n=20,\quad \bar{x}=110,\quad s=12
$$

Formula

$$
CI =
\bar{x}
\pm
t_{\alpha/2,n-1}
\frac{s}{\sqrt{n}}
$$

Standard error

$$
SE = \frac{12}{\sqrt{20}} = 2.683
$$

Margin

$$
2.093 \times 2.683 = 5.62
$$

Confidence interval

$$
110 \pm 5.62
$$

$$
(104.38,\;115.62)
$$

---

# Q8 — Two‑Proportion z Test

City A

$$
\hat{p}_1 = \frac{180}{300} = 0.60
$$

City B

$$
\hat{p}_2 = \frac{135}{250} = 0.54
$$

Pooled proportion

$$
\hat{p} =
\frac{315}{550}
=
0.573
$$

Standard error

$$
SE \approx 0.04236
$$

Test statistic

$$
z =
\frac{0.60-0.54}{0.04236}
\approx
1.42
$$

Since

$$
|z| < 1.96
$$

Fail to reject \(H_0\).

Conclusion: vaccination rates are not significantly different.

