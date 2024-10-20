* Coeffidence interval ger för en one unit change.
  * Om vi vill ha flera unit change, multiplicera med antal units

* was there a statistically significant change n beta_1 compared to old beta_1?
  * H0: beta_1 = old_beta_1
  * Kan inte bara beta_1 = old_beta_1_värdet eftersom det finns osäkerhet i oldbeta värdet

* p-value är altenativet till att använda kritiska värden

* Discrete prob dist
  * ANswer like P(X = 1) = 0.3, P(X = 2) = 0.2, P(X = 3) = 0.5

* om jag kollar up 1.96 i normal distributed så får jag 2.5%, vilket är onesided. Om jag även kollar -1.96 så får jag 2.5% till. Det är two sided. 

* c.i använder 2 sided.

* confidence interval:
  * Contains true value with 95% probability

* standard error of a proportin (e.g. percentage) SE(p hat) = p(1-p)/n

* does one class have more than another:
  * hypotestest som jämför means mean_a - mean_b = 0 vs mean_a - mean_b not = 0
  * Här är SE(both) = root(a/b + c/d) sakn. note inte dela på root n. Står i formelblad vad SE(both) är. Det är lika med sigma för någon anledningsnng. Det faktum att vi har root n där i red hina att v kan skippa dem. OOooooooo det är för att n/root n = root n. WOW!

* om vi har en regression och vi vill veta sample mean averge av 100, bara ta value bar*beta hat.
  * Mean av smple averge av hundrre är value bar. Mer intuitivt än vad jag får det att låta.

* Sample standard deviation of 100 test scores.

* 5.3)
  * 1.5 height difference. SE 0.31. Coefficient 3.94.
  * Create a 99% for the difference btween their heights
    * Easy to create one for a one unit difference
      * (3.94 +- 2.58 0.31)
        * So for a 1.5 unit change: 1.5(3.94 +- 2.58 0.31)
  * GÖR OM DENNA FRÅGA

* Gör utan tvekan om 7.3

* k does not include the intecept in the 
  
* F-statistic är det vi har fått ut från tester

* 7.9 är väsentlig
  * Men det är bara vad jag naturally gör. Lägg allt på en sid och testa Testin gsingle restrictions on multiple från README.md

* ln(new) - ln(old) \approx (new-old)/old. ERGO we can apprixmate the difference between two ln as a procentage change. 

* intercept does not count as a regressor

* F-test är väldigt dependent på att du använder rätt tal


* state it as mu_a - mu_b = 0 inte mu_a = mu_b
  * Bra men inte jätteviktigt 
  * Min känsla på att man inte ska dela med root n här är rätt, men oklar varför

* Stat. Indp. P(X and Y) = P(X)P(Y)

* Sample correlation is not consisten

* Correlation = S_XY / (S_X S_Y)
  * OFC för det är ju den som är standardiserad
    * Den som står vi beta more or less

* Before and after is used when analyzing how a unit change in X, changes Y
  * "What is the predicted change in test scores associated with a change in district income of $1000, based on the estimated quadratic regression function in Equation (8.2)?"


* Why is E(u_i|X) = 0 in our model?
  * Because u_i is independent on X. 
  * E(u_i | X) = E(u_i)
    * Therefore we also require that E(u_i) = 0
      * and since u_i represents devitons frm the averge, this essentally always the cse.
