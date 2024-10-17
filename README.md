# Förl 2
## Theoretical
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















