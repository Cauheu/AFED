# AFED
Analysis of financial and economical data for forecasting.

# Research objectives
The main goal of this work is to learn how to apply data mining techniques to
solving problems of financial and economic data analysis.
Use the Bayesian network apparatus to model probabilistic problems and
predicting probabilistic variables as well as decision trees, regression models for
predict the absolute values of financial characteristics and compare them for
the selected data set. 

# Data description
RowNumber - corresponds to the record number (line) and does not affect the result. <br />
CustomerId - contains random values and does not affect the result.<br />
Surname - the client's last name does not affect his decision to leave the bank.<br />
CreditScore - can affect the outflow of customers because the customer with a higher
credit score is less likely to leave the bank.<br />
Geography - the location of the client can influence his decision
leave the bank.<br />
Gender - it is interesting to investigate whether gender plays a role in the outflow from the bank.<br />
Age is definitely relevant, as older clients are less likely to leave
your bank than younger.<br />
Tenure - means the number of years during which the client was a client of the bank. How
as a rule, older clients are more loyal and less likely to leave the bank.<br />
Balance is also a very good indicator of customer outflow as people from
higher balance on the accounts are less likely to leave the bank compared to those who
has a lower balance.<br />
NumOfProducts - refers to the number of products that the customer has purchased through
bank. <br />
HasCrCard - means whether the customer has a credit card. This count too
relevant because people with a credit card are less likely to leave the bank.<br />
IsActiveMember - active customers are less likely to leave the bank.<br />
EstimatedSalary - as on the balance sheet, people with lower salaries are more likely
leave the bank compared to those who have a higher salary.<br />
Exited - an indicator of whether the client left the bank or not.<br />

# Used models
1) Bayesian Networks
The Greedy Thick Thinning (GTT) structure learning algorithm is based on the Bayesian Search approach and has been described in (Cheng et al., 1997). GTT starts with an empty graph and repeatedly adds the arc (without creating a cycle) that maximally increases the marginal likelihood P(D|S) until no arc addition will result in a positive increase (this is the thickening phase). Then, it repeatedly removes arcs until no arc deletion will result in a positive increase in P(D|S) (this is the thinning phase). It is an approximate but a very fast algorithm that yields quite good structures.
2) Decision trees
**CHAID**. Chi-squared Automatic Interaction Detection. At each step, CHAID chooses the independent (predictor) variable that has the strongest interaction with the dependent variable. Categories of each predictor are merged if they are not significantly different with respect to the dependent variable.

**Exhaustive CHAID.** A modification of CHAID that examines all possible splits for each predictor.

**CRT**. Classification and Regression Trees. CRT splits the data into segments that are as homogeneous as possible with respect to the dependent variable. A terminal node in which all cases have the same value for the dependent variable is a homogeneous, "pure" node.

**QUEST**. Quick, Unbiased, Efficient Statistical Tree. A method that is fast and avoids other methods' bias in favor of predictors with many categories. QUEST can be specified only if the dependent variable is nominal.

3) **Logistic regression** allows the effect of multiple independents on one
binary dependent variable to be tested. It is predominantly used to assess relationships between
the binary dependent variable and each independent variable whilst controlling for the other
independent variables but also produces an equation (model) which can be used for prediction. It is
similar to multiple linear regression but instead of predicting the value of the dependent variable, it
can be used to calculate the probability of an event occurring.
