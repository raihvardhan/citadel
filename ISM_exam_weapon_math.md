
# ISM Final Exam Weapon – Full Questions and Solutions (Proper Math)

This version uses **LaTeX math notation** so formulas render correctly in tools like
VS Code (Markdown Preview), Typora, Obsidian, Notion, and GitHub.

Referenced book:
Statistics for Business and Economics (Anderson et al.)

---

# Question 1 – Karl Pearson Correlation

Data

| Temperature | Electricity |
|---|---|
30 | 220 |
32 | 240 |
35 | 260 |
37 | 300 |
33 | 250 |

### Means

$$
\bar{x} = \frac{30+32+35+37+33}{5} = 33.4
$$

$$
\bar{y} = \frac{220+240+260+300+250}{5} = 254
$$

### Formula

$$
r =
\frac{\sum (x_i-\bar{x})(y_i-\bar{y})}
{\sqrt{\sum (x_i-\bar{x})^2 \sum (y_i-\bar{y})^2}}
$$

Final result

$$
r \approx 0.973
$$

Strong positive correlation.

Source: Anderson Chapter 3 and 14

---

# Question 2 – Exponential Smoothing

Demand

|Month|Demand|
|---|---|
Jan|120
Feb|135
Mar|150
Apr|160
May|155
Jun|170

Initial forecast

$$
F_1 = Y_1
$$

Forecast equation

$$
F_{t+1} = \alpha Y_t + (1-\alpha)F_t
$$

Results

$$
\alpha = 0.4 \Rightarrow F_7 \approx 157.53
$$

$$
\alpha = 0.7 \Rightarrow F_7 \approx 165.52
$$

Source: Anderson Chapter 17

---

# Question 3 – Paired t Test

Differences

$$
d_i = \text{After}_i - \text{Before}_i
$$

Mean difference

$$
\bar{d} = \frac{\sum d_i}{n}
$$

Standard deviation

$$
s_d =
\sqrt{
\frac{\sum(d_i-\bar{d})^2}{n-1}
}
$$

Test statistic

$$
t = \frac{\bar{d}}{s_d/\sqrt{n}}
$$

Result

$$
t \approx 13.56
$$

Reject \(H_0\).

Source: Anderson Chapter 9

---

# Question 4 – One Way ANOVA

Between variation

$$
SS_{Tr} =
\sum n_j(\bar{y}_j - \bar{y})^2
$$

Within variation

$$
SSE =
\sum\sum(y_{ij}-\bar{y}_j)^2
$$

Mean squares

$$
MS_{Tr} = \frac{SS_{Tr}}{k-1}
$$

$$
MS_E = \frac{SSE}{N-k}
$$

Test statistic

$$
F = \frac{MS_{Tr}}{MS_E}
$$

Example result

$$
F = 19
$$

Reject \(H_0\).

Source: Anderson Chapter 13

---

# Question 5 – Linear Regression

Model

$$
Y = \beta_0 + \beta_1 X
$$

Slope

$$
\hat{\beta}_1 =
\frac{\sum (x_i-\bar{x})(y_i-\bar{y})}
{\sum (x_i-\bar{x})^2}
$$

Intercept

$$
\hat{\beta}_0 =
\bar{y} - \hat{\beta}_1 \bar{x}
$$

Example regression equation

$$
\hat{Y} = 1.7 + 0.95X
$$

Prediction

$$
\hat{Y}(9) = 10.25
$$

Source: Anderson Chapter 14

---

# Question 6 – Gaussian Mixture Model

Mixture density

$$
f(x) =
0.5\,\phi(x|\mu_1,\sigma_1^2)
+
0.5\,\phi(x|\mu_2,\sigma_2^2)
$$

Normal pdf

$$
\phi(x|\mu,\sigma^2)=
\frac{1}{\sqrt{2\pi\sigma^2}}
\exp\!\left(
-\frac{(x-\mu)^2}{2\sigma^2}
\right)
$$

Observation \(x=25\) is closer to component with \(\mu_1=22\).

Source: Anderson Chapter 6

---

# Question 7 – Confidence Interval

$$
CI =
\bar{x} \pm
t_{\alpha/2,n-1}
\frac{s}{\sqrt{n}}
$$

Example

$$
110 \pm 5.62
$$

Interval

$$
(104.38,\;115.62)
$$

Source: Anderson Chapter 8

---

# Question 8 – Two Proportion Test

Sample proportions

$$
\hat{p}_1 = \frac{x_1}{n_1}
$$

$$
\hat{p}_2 = \frac{x_2}{n_2}
$$

Pooled proportion

$$
\hat{p} =
\frac{x_1+x_2}{n_1+n_2}
$$

Standard error

$$
SE =
\sqrt{
\hat{p}(1-\hat{p})
\left(
\frac{1}{n_1}+\frac{1}{n_2}
\right)
}
$$

Test statistic

$$
z =
\frac{\hat{p}_1-\hat{p}_2}{SE}
$$

Example

$$
z \approx 1.42
$$

Fail to reject \(H_0\).

Source: Anderson Chapter 10

