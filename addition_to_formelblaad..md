var(ax+b) = a^2var(x)

var(X + Y) = Var(X) + Var(Y) - 2Cov(X, Y)

P(A och B) = P(A)/P(B givet A)

När vi har en sådan tabell. Discrete:
    * P(X = x, Y = y) i varje cell
    * **P(y) summeera bara upp raden eller kolumnen. Då får vi p(Y = y) = SUM(P(X = x, Y = y) for all x possble) rimligt, men ej en formel**
    * vill ha E(Y). Räkna bara SUM(y P(Y = y)) See above för den. 
    *** Variansen, använd Var(X) = E(X^2) - E(X)^2.**
    * Calc probability density given x = 6. P(Y = y givet X = 6) = P(X = 6, Y = y)/P(X = 6). DO this for all possoble y, thas your distroy
    * Condional expectation E(Y givet X = x) = SUM(y P(Y = y givet X = x))
Total probablility_:P(Y) = SUM(p(x)p(Y givet x))

Bayes formula

conditoonal probablility formula
P(X = x givet Y = y) = P(X = x, Y = y)/P(Y = y)


SE(aX + bY) = sqrt(a^2SE(X)^2 + b^2SE(Y)^2 + 2abCov(X, Y)

SE(X) = sqrt(Var(X)/n) = sigma/sqrt(n)

* generellt c.i = estimate +- t_val*SE(estimat)). Estmat är p hat eller b hat eller whatever
  * e.g. x bar +- z sigma/sqrt(n), for large n.  


* SSE = SSR (synomer)

* Notera relationen mellan SER och RSS. (n-k-1) SER^2 = RSS
  * Så den är användbar för att räkna R^2 
  * Notera att detta kopplar ser till rss som är kopplat till ess och tss
* notera ävnen S_y = TSS/n-1


* TSS = RSS + SSR = RSS + SSE???

TSS är the variance of the dependent variable.


