# Table of Contents
- [Table of Contents](#table-of-contents)
- [Lecture content couples by topics](#lecture-content-couples-by-topics)
  - [Basics](#basics)
  - [Sample basics](#sample-basics)
  - [Binanry special case](#binanry-special-case)
  - [Hypothesis testing](#hypothesis-testing)
    - [Two sided means](#two-sided-means)
    - [One sided means](#one-sided-means)
    - [Two sided beta (both univaraite and multivariate)](#two-sided-beta-both-univaraite-and-multivariate)
    - [Difference in means](#difference-in-means)
    - [Joint hypothesis test](#joint-hypothesis-test)
    - [Testin gsingle restrictions on multiple](#testin-gsingle-restrictions-on-multiple)
  - [p-value](#p-value)
    - [Two sided](#two-sided)
    - [THeyre all well statated in the formula sheet](#theyre-all-well-statated-in-the-formula-sheet)
  - [Confidence interval](#confidence-interval)
    - [bar(y)](#bary)
    - [beta (both univaraite and multivariate)](#beta-both-univaraite-and-multivariate)
  - [Measures of Fit and their relations](#measures-of-fit-and-their-relations)
    - [The variables](#the-variables)
    - [Meassures of Fit relationships](#meassures-of-fit-relationships)
  - [Ideal interpretations](#ideal-interpretations)
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
  - [p-value](#p-value-1)
  - [Estimator of variance Y](#estimator-of-variance-y)
- [Förl 5](#förl-5)
  - [Confidence interval](#confidence-interval-1)
  - [Difference in means](#difference-in-means-1)
    - [Confidence intervals](#confidence-intervals)
    - [Sample covariance and correlation](#sample-covariance-and-correlation)
- [Förl 6](#förl-6)
  - [beta solutions](#beta-solutions)
  - [Meassures of Fit](#meassures-of-fit)
  - [Assumptions](#assumptions)
- [Förl 7](#förl-7)
  - [Bias of beta](#bias-of-beta)
  - [Hypothesis testing on beta](#hypothesis-testing-on-beta)
  - [Confidence interval](#confidence-interval-2)
  - [Homo vs heteroskedaticity](#homo-vs-heteroskedaticity)
  - [Homo and heteroskedality](#homo-and-heteroskedality)
- [Förl 8](#förl-8)
  - [Omitted variable bias](#omitted-variable-bias)
    - [Formula to see what](#formula-to-see-what)
    - [Overcomming bias](#overcomming-bias)
  - [Multivariate model](#multivariate-model)
  - [Measures of fit](#measures-of-fit)
  - [Hypothesis test](#hypothesis-test)
- [Förl 9](#förl-9)
  - [Multivariate OLS assumptins](#multivariate-ols-assumptins)
  - [Imperefect multicollinearity](#imperefect-multicollinearity)
  - [Consistent and unbiased](#consistent-and-unbiased)
  - [Omitted variable bias](#omitted-variable-bias-1)
- [Förl 10](#förl-10)
  - [Hypothesis test](#hypothesis-test-1)
    - [Single variable in multivariatea](#single-variable-in-multivariatea)
    - [Joint hypothesis test](#joint-hypothesis-test-1)
    - [Testin gsingle restrictions on multiple coefficients](#testin-gsingle-restrictions-on-multiple-coefficients)
  - [A lot of yadaa in the end](#a-lot-of-yadaa-in-the-end)
- [Förl 11](#förl-11)
- [Förl 12](#förl-12)



# Lecture content couples by topics
## Basics
* P(X = x givet Y = y) = P(X = x, Y = y)/P(Y = y)

* P(Y) = SUM(p(x)p(Y givet x))

* E(XY) = E(X)E(Y) + Cov(X, Y) = [independence] E(X)E
(Y)

* P(X and Y) = P(X)P(Y)

* var(X) = E(X - E(X)))**2 = E(X^2) - E(X)^2
* var(ax+b) = a^2var(x
* var(X + Y) = Var(X) + Var(Y) + 2Cov(X, Y)

* SD(aX + bY) = sqrt(a^2SD(X)^2 + b^2SD(Y)^2 + 2abCov
(X, Y)

* SQRT(var(a*beta_3 + b*beta_4)) = sqrt(SE(a*beta_3)^2 + SE(b*beta_4)^2 + 2abcov(beta_3, beta_4))
* var(a*beta_3 + b*beta_4) = SE(a*beta_3)^2 + SE(b*beta_4)^2 + 2abcov(beta_3, beta_4)
* SE(aX + bY) = \sqrt(a^2 * SE(X)^2 + b^2 * SE(Y)^2 + 2abCov(X,Y))

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

* Estimated Error Variance = variance of the error = SUM(u_i^2)/(N-2) = SER^2

## Binanry special case
SE can be found:
* beta_0 = bar(Y_m)
* beta_1 = bar(Y_m) - bar(Y_m)

From these we can find the SE and mean of beta_0 and beta_1

## Hypothesis testing
### Two sided means
* H_0: μ = μ_0
* H_A: μ != μ_0

* df = n - 1
  * On two sided, look up the 10% one sided in the normal table

### One sided means
* H_0: μ <= μ_0
* H_A: μ > μ_0

* df = n - 1

### Two sided beta (both univaraite and multivariate)
* H_0: beta = beta_0
* H_A: beta != beta_0

* On two sided, look up the 2.5% one sided in the normal table

* df = n - k - 1

### Difference in means
* H_0: μ_a - μ_b = d_0
* H_A: μ_a - μ_b != d_0

* bar(Y_1) - bar(Y_2) in N(μ_1 - μ_2, σ^2_1/n_1 + 
σ^2_2/n_2)
  * n large enough: bar(Y_1) - bar(Y_2) in N(μ_1 - 
μ_2, s^2_1/n_1 + s^2_2/n_2)
  * Can standardize based this and perform a test

* If assume sigma_1 = sigma_2
  * df = n_1 + n_2 - 2

* If assumed sigma_1 != sigma_2
  * Seems more complicated than it should be??
    * Welch-Satterthwaite formula
      * Keep to the pooled version?
        * so persumably they wont ever ask us for df....



### Joint hypothesis test
* H_0: beta_1 = 0 and beta_2 = 0
* H_A: beta_1 != 0 or beta_2 != 0

* Interpretation:
  * If x_1 and x_2 are two difference school resources, this test would test if the school resources matter at all.

* F-statistic
  * One only holds under homoskedasticity.

* unrestricted
  * Full model

* restricted:
  * the model under the null hypothesis
    * For instance if we are testing if two betas might be zero, we can exclude those terms
    * To find the restricted SSR, s_y gives TSS is RSS since in this case the restricted model is only an intercept, so no variance is explained, i.e. TSS = SSR

* In the homoskedastic case, F-stat is F_(q, inf)
  * q is the number of restriction under the null hypothesis.
  * not the the heteroskedastic cases
    * then the upper limit is df = n - k - 1 i beleive

### Testin gsingle restrictions on multiple 
coefficients
H_0: beta_1 = beta_2
H_1: beta_1 != beta_2
- Make a difference test
  - just make a normal test, seing beta_2 as a constnt even though is an estimate.

* (beta_1 - beta_2)/SE(beta_1 - beta_2)

* SE(beta_1 - beta_2)
  * SE(aX + bY) = \sqrt(a^2 * SE(X)^2 + b^2 * SE(Y)^2 + 2abCov(X,Y))
  * if beta_1 and beta_2 are tested independely, cov is 0****


## p-value
### Two sided
2ZNORM(-abs(t_act)) and then compare this to the confidence level
- literally the same as for critical t but we go one way but not the other


### THeyre all well statated in the formula sheet

## Confidence interval
### bar(y)
* CI = bar(Y) +- t_val*SE(bar(Y))
  * SE(bar(Y)) = s_Y/sqrt(n)
  * t_val is from t-table
    * Note that t_val is for two sided test

* df = n - 1

### beta (both univaraite and multivariate)
* CI = hat(beta) +- t_val*SE(hat(beta))

* df = n - k - 1

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

* adjusted R**2
  * Note this is strictly less than R**2
  * Solves the issue that every time you add a regressor, there will be a better fit. Use only if multiple regressors

* SER
  * The magnitude of a 
typical regression 
residuals with the unit 
of Y


### Meassures of Fit relationships
* TSS = ESS + RSS

* (n-1) S_y**2 = TSS

* (n-k-1) SER^2 = RSS
  * k räknar inte intercept här :// enligt E4.1 

* SSE = SSR = RSS != ESS

* SER gives RSS. RSS with R**2 gives TSS gives SD(Y) ergo s_Y

## Ideal interpretations
* Linear univariate
  * Duh

* Binary regressors
  * Same as linear univariate
  * However, not that off (0) is the value at intercept and on (1) is the slope value. 
  * Slope is the differnce between the two 

* Linear multivariate
  * Holding all other independent variables, a one unit change in x will on average lead to a beta_i increases in y

* log-linear
  * ln(Earnings) for females are, on average, 0.44 lower for men than for women.
    * ja... men approximation would be nice.
      * Tror det är, if one unit increse in th independent variable leads on verge to a beta % increase in dependent
  
* linear-log
  * * a 1% increse in independet variable leads to a 0.01 beta increase in dependent

* log-log
  * a 1% increse in independet variable leads to a beta % increase in dependent



# Förl 2
## Basics
* E(XY) = E(X)E(Y) + Cov(X, Y) = [independence] E(X)E(Y)

* var(X) = E(X - E(X)))**2 = E(X^2) - E(X)^2
* var(ax+b) = a^2var(x)
* var(X + Y) = Var(X) + Var(Y) - 2Cov(X, Y)

* SD(aX + bY) = sqrt(a^2SD(X)^2 + b^2SD(Y)^2 + 2abCov(X, Y)???
* 
* SE(X) = SD(X) / sqrt(n)

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

* df = n - 1

* H_0: μ <= μ_0
* H_A: μ > μ_0
  * One sided

* df = n - 1

* H_0: μ <= μ_0
* H_A: μ != μ_0
  * One sided, and weirdly accceptable

* df = n - 1

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

* df = n - 1

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
1. E(u | X = x) = 0
  * Error averge doesnt depend on X
2. (X_i, Y_i) are idd
  * i.e. collected from a simple random sampling
  * Broken whn we record data from only one entity

3. Large outlier are rare
  * OLS are sensistive to these
  * E(X^4) less than infinity 


# Förl 7
## Bias of beta
* E(hat(b)) = b (unbiased)
* hat(b) -> b (consistent)
  * Convergence as n -> oo


## Hypothesis testing on beta
* H_0: beta = beta_0
* H_A: beta != beta_0
  * Two sided

* df = n - k - 1


## Confidence interval
* CI = hat(beta) +- t_val*SE(hat(beta))

* df = n - k - 1

## Homo vs heteroskedaticity
* Heteroskedacity: variance of the error u is dependent on the independemt variable on the x axis.

* **if n is large, the homo and heteroskedastic formulas coincide**

* Nothing you can do about it without code. So just know the concept for the midterm
  * well... you can use the heteroskedastic formulas but that seems awfully unlikely to happen 


## Homo and heteroskedality
* Homoskedality: Var(u | X) = 0
  * i.e. the variance of the error doesnt depend on X


# Förl 8
## Omitted variable bias
For a variable to lead to OVB, the omitted variable Z must follow **both** of the following.
1. Z needs to be a determinant f Y
   1. I.E. Z is currently a part of u

2. Corr(Z, X) != 0

### Formula to see what 
hat(b) -> b + (sigma_u/sigma_X) * rho_(X,u)

* a meassurment of how biased that hat(b) is compared to b

### Overcomming bias
1. Include Z
2. Remove Corr(X, u) != 0 in the tests by randomly assigning kids bad at english into classes of varying sizes
3. Remove the dependence of Y on Z in the testing.


## Multivariate model
Y = ...
Y + delta(Y) = ...
beta_i = delta(Y)/delta(X_i)

## Measures of fit
* SER, R**2 same defintiosnx
* ajdusted R^2
  * Solves the issue that every time you add a regressor, there will be a better fit. Use only if multiple regressors

## Hypothesis test
TODO. See lab


# Förl 9
## Multivariate OLS assumptins
1. Same as univariate
   1. E(u_i | X_1, ..., X_m) = 0
   2. (X_1i, ..., X_mi, Y_i) are idd
   3. Outliers are rare E(X_ji^4) less than infinity
2. No perfect multicollineariy
   1. When one regressor is a perfect linear function of another regressor
   2. Will be the case if we have male and female and constant as regressors
      1. Dummy variable trap

## Imperefect multicollinearity
When two or more variables are highly correlated
  * atleast one of the variables will be imperfectly estimated
  * The idea: the coefficient on X 1 is the effect of X 1 holding
    X 2 constant; but if X 1 and X 2 are highly correlated, there is
    very little variation in X 1 once X 2 is held constant – so the
    data don’t contain much information about what happens
    when X 1 changes but X 2 doesn’t. If so, the variance of the
    OLS estimator of the coefficient on X 1 will be large.
  
## Consistent and unbiased
* Same as univariate
## Omitted variable bias
* Same as univariate
* 


# Förl 10
## Hypothesis test
### Single variable in multivariatea
* Same as always
* df = n - k - 1


### Joint hypothesis test
* H_0: beta_1 = 0 and beta_2 = 0
* H_A: beta_1 != 0 or beta_2 != 0

* Interpretation:
  * If x_1 and x_2 are two difference school resources, this test would test if the school resources matter at all.

* F-statistic
  * One only holds under homoskedasticity.

* unrestricted
  * Full model

* restricted:
  * the model under the null hypothesis
    * For instance if we are testing if two betas might be zero, we can exclude those terms

* In the homoskedastic case, F-stat is F_(q, inf)
  * q is the number of restriction under the null hypothesis.
  * not the the heteroskedastic cases
    * Then the upper limit is df = n - k - 1 i beleive

### Testin gsingle restrictions on multiple coefficients
H_0: beta_1 = beta_2
H_1: beta_1 != beta_2

df = ...?

## A lot of yadaa in the end
slide 27 and forward skipped
* Nothing of substance imo

# Förl 11

# Förl 12




















