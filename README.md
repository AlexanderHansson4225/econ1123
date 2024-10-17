# Table of Contents
- [Table of Contents](#table-of-contents)
- [Topics](#topics)
  - [Basics](#basics)
  - [Sample basics](#sample-basics)
  - [Hypothesis testing](#hypothesis-testing)
    - [Two sided](#two-sided)
    - [One sided](#one-sided)
    - [Difference in means](#difference-in-means)
  - [Confidence intervals](#confidence-intervals)
  - [Measures of Fit and their relations](#measures-of-fit-and-their-relations)
    - [The variables](#the-variables)
    - [Meassures of Fit relationships](#meassures-of-fit-relationships)
- [Förl 2](#förl-2)
  - [Basics](#basics-1)
  - [Means](#means)
  - [Normal](#normal)
- [Förl 3](#förl-3)
  - [LoLN](#loln)
  - [Consistent and non-biased](#consistent-and-non-biased)
  - [Central Limit Theorem](#central-limit-theorem)
- [Förl 4](#förl-4)
  - [Hypothesis testing](#hypothesis-testing-1)
  - [p-value](#p-value)
  - [Estimator of variance Y](#estimator-of-variance-y)
- [Förl 5](#förl-5)
  - [Confidence interval](#confidence-interval)
  - [Difference in means](#difference-in-means-1)
    - [Confidence intervals](#confidence-intervals-1)
    - [Sample covariance and correlation](#sample-covariance-and-correlation)
- [Förl 6](#förl-6)
  - [beta solutions](#beta-solutions)
  - [Meassures of Fit](#meassures-of-fit)
  - [Assumptions](#assumptions)
- [Förl 7](#förl-7)
  - [Bias of beta](#bias-of-beta)
  - [Hypothesis testing on beta](#hypothesis-testing-on-beta)



# Topics
## Basics
* E(XY) = E(X)E(Y) + Cov(X, Y) = [independence] E(X)E
(Y)

* var(X) = E(X - E(X)))**2 = E(X^2) - E(X)^2
* var(ax+b) = a^2var(x
* var(X + Y) = Var(X) + Var(Y) - 2Cov(X, Y)

* SD(aX + bY) = sqrt(a^2SD(X)^2 + b^2SD(Y)^2 + 2abCov
(X, Y)???

* Skewness = E(X - E(X))^3/SD(X)^(3)
  * Positiv skewness betyder att det är mer data till 
vänster om medelvärdet
* Kurtosis = E(X - E(X))^4/SD(X)^(4)
  * Kurtosis = 3 för normalfördelning
  * A kurtosis > 3 betyder att det är mer data i 
svansen

* cov(X, Y) = E(X - E(X))(Y - E(Y)) = E(XY) - E(X)E(Y)
* cov(X, X) = var(X)

* corr(X, Y) = cov(X, Y)/SD(X)SD(Y)

## Sample basics
* S_XY = (1/n-1) SUM(X_i - bar(X)(Y_i - bar(Y)))
* r_XY = S_XY / S_X S_Y
* s_y^2 = SUM(Y_i - bar(Y))^2/(n-1)

## Hypothesis testing
### Two sided
* H_0: μ = μ_0
* H_A: μ != μ_0

### One sided
* H_0: μ <= μ_0
* H_A: μ > μ_0
  * One sided

### Difference in means
* H_0: μ_a - μ_b = d_0
* H_A: μ_a - μ_b != d_0

* bar(Y_1) - bar(Y_2) in N(μ_1 - μ_2, σ^2_1/n_1 + 
σ^2_2/n_2)
  * n large enough: bar(Y_1) - bar(Y_2) in N(μ_1 - 
μ_2, s^2_1/n_1 + s^2_2/n_2)
  * Can standardize based this and perform a test

## Confidence intervals
* CI = bar(Y) +- t_val*SE(bar(Y))
  * SE(bar(Y)) = s/sqrt(n)
  * t_val is from t-table
    * Note that t_val is for two sided tests

## Measures of Fit and their relations
### The variables
* TSS
  * Total sum of squares
  * The toal variation of the observed data

* sum of squares due to regression (SSR) or explained sum of squares (ESS) or 
  * Explained sum of squares
  * The amount of variation explained by the model

* RSS
  * Residual sum of squares
  * The amount of variation not explained by the model

* R^2
  * How much of the 
variance does the model 
explain
  * Given the definitions of ESS and TSS, makes full senses why R**2 is ESS/TSS

* SER
  * The magnitude of a 
typical regression 
residuals with the unit 
of Y


### Meassures of Fit relationships
* TSS = ESS + RSS

* (n-1) S_y**2 = TSS

* (n-k-1) SER^2 = RSS

* SSE = SSR = ESS
  * https://canvas.harvard.edu/courses/138520/discussion_topics/1085306
    * SSE = SSR
  * https://en.wikipedia.org/wiki/Explained_sum_of_squares
    * SSR = ESS
      * First sentence


# Förl 2
## Basics
* E(XY) = E(X)E(Y) + Cov(X, Y) = [independence] E(X)E(Y)

* var(X) = E(X - E(X)))**2 = E(X^2) - E(X)^2
* var(ax+b) = a^2var(x
* var(X + Y) = Var(X) + Var(Y) - 2Cov(X, Y)

* SD(aX + bY) = sqrt(a^2SD(X)^2 + b^2SD(Y)^2 + 2abCov(X, Y)???

* Skewness = E(X - E(X))^3/SD(X)^(3)
  * Positiv skewness betyder att det är mer data till vänster om medelvärdet
* Kurtosis = E(X - E(X))^4/SD(X)^(4)
  * Kurtosis = 3 för normalfördelning
  * A kurtosis > 3 betyder att det är mer data i svansen

* cov(X, Y) = E(X - E(X))(Y - E(Y)) = E(XY) - E(X)E(Y)
* cov(X, X) = var(X)

* corr(X, Y) = cov(X, Y)/SD(X)SD(Y)

## Means
* E(X̣|Y = y) = 
  * Discrete: SUM(xP(X = x|Y = y))
  * Continuous: ∫x f(x|Y = y)dx

## Normal
* n in N(μ, σ^2) = (n - mean)/SD(n)
* P(X <= a) = P(Z <= z_a) = phi(z_a)
* P(b < X <=  a)P(z_ b< Z <= z_a) = phi(z_a) - phi(z_b)
* P(b < X) = 1 - P(X <= b) = phi(z_b)


# Förl 3

## LoLN
* bar(Y) = SUM(Y_i); Y_i idd
  * E(bar(Y)) = E(Y_i)
  * Var(bar(Y)) = Var(Y)/n

## Consistent and non-biased
Skipped, slide and 5, 14 and 15

## Central Limit Theorem
Summing idd Y_i and then standarizing will give a N(0,1) distribution.
* bar(Y) in N(E(Y_i), Var(Y)/n)
* Standardizing this gives N(0,1)


# Förl 4
## Hypothesis testing
* H_0: μ = μ_0
* H_A: μ != μ_0
  * Two sided

* H_0: μ <= μ_0
* H_A: μ > μ_0
  * One sided

* H_0: μ <= μ_0
* H_A: μ != μ_0
  * One sided, and weirdly accceptable

## p-value
Skipped, slide 3, 4, 5, 7, 8, 9

## Estimator of variance Y
* s_y^2 = SUM(Y_i - bar(Y))^2/(n-1)
  * E(s^2) = σ^2
  * Note 

# Förl 5
## Confidence interval
* CI = bar(Y) +- t_val*SE(bar(Y))
  * SE(bar(Y)) = s/sqrt(n)
  * t_val is from t-table
    * Note that t_val is for two sided test

## Difference in means
* H_0: μ_a - μ_b = d_0
* H_A: μ_a - μ_b != d_0
  
* bar(Y_1) - bar(Y_2) in N(μ_1 - μ_2, σ^2_1/n_1 + σ^2_2/n_2)
  * n large enough: bar(Y_1) - bar(Y_2) in N(μ_1 - μ_2, s^2_1/n_1 + s^2_2/n_2)
  * Can standardize based this and perform a test

### Confidence intervals
* bar(Y_1) - bar(Y_2) +- t_val*sqrt(s^2_1/n_1 + s^2_2/n_2)

### Sample covariance and correlation
* S_XY = (1/n-1) SUM(X_i - bar(X)(Y_i - bar(Y)))
* r_XY = S_XY / S_X S_Y

# Förl 6
* OLS is based on the least squares solution

## beta solutions
* se formelblad

## Meassures of Fit
* R^2
  * How much of the variance does the model explain

* SER
  * The magnitude of a typical regression residuals with the unit of Y

## Assumptions
* Skipped slide 21, 22, 23, 24, 25, 26

# Förl 7
## Bias of beta
* Skipped, slide 4

## Hypothesis testing on beta
* 































