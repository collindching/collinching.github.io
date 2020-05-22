---
layout: single
title: "Why your regression coefficients have the wrong sign"
subtitle: "Addressing collinearity in practice"
excerpt: "Addressing collinearity in practice"
---

Imagine you build a model for your company's marketing team, and in the stakeholder meeting, you present the following output:

- For this output, create correlated marketing data where sales volume is target variable
- Create two variables that are highly correlated, and also have a similar effect
- Then show outputs

How will your stakeholders react? While your model says this... does it actually make sense? If you do show this result, expect to receive a harsh berating. 

### Suspect collinearity

If you are working on a regression model and

1. Variables that should have positive coefficients are negative (or vice versa),
2. Your coefficients change significantly (i.e. flip signs) as you add/remove predictors
3. Variables that should be significant don't present as significant 

Then you should immediately suspect collinearity. 

At the same time, if the model does not match your intuition, make sure to challenge your assumptions as well. At times, your model may show you counterintuitive information that challenges your beliefs -- but is actually accurate. My suggestion is to always keep your assumptions and beliefs in check, and keep an open mind where possible. 

### Solutions

#### Do you have the option of removing correlated predictors? 

Notes

#### Will regularized regression work in your context? 

Notes

#### Residualize yoru stuff

Notes

#### Merging variables together

Notes

### A recap on the framework for approaching collinearity, and a few additional working example

Here is the framework I would use for 
- Provide minimal working evidence of collinearity issue
- Map potential solutions (ranked from simple to complex)
- Test each solution out, documenting your steps and results for each one




Provide simple evidence that collinearity is in fact the culprit. Do this by presenting a model in which your coefficients make sense, another where they don't, and then show the correlations and VIF for variables that are wrong.





Literature review:
- [Variable selection via clustering](https://web.stanford.edu/class/stats202/content/lec5-condensed.pdf)
- [Oh No! I Got the Wrong Sign! What Should I do?](http://www.stat.columbia.edu/~gelman/stuff_for_blog/oh_no_I_got_the_wrong_sign.pdf)
- [Regression signs that flip after including other predictors](https://stats.stackexchange.com/questions/1580/regression-coefficients-that-flip-sign-after-including-other-predictors)
- [Correlation based feature selection with clustering for high dimensional data](https://www.sciencedirect.com/science/article/pii/S2314717218300059)
- [Choosing the Right Variables for the Right Hand Side](https://www.kellogg.northwestern.edu/faculty/dranove/htm/dranove/coursepages/Mgmt%20469/choosing%20variables.pdf)
- [How to deal with high correlation among predictors in multiple regression](https://stats.stackexchange.com/questions/38093/how-to-deal-with-high-correlation-among-predictors-in-multiple-regression)
- [Multicollinearity](https://statisticsbyjim.com/regression/multicollinearity-in-regression-analysis/)
- [Collapsing two variables into one for analysis](https://stats.stackexchange.com/questions/32472/collapsing-combining-two-variables-into-one-for-analysis)
- [StackExchange](https://stats.stackexchange.com/questions/198271/regression-coefficients-seem-to-have-the-wrong-sign-can-i-force-them-to-have-a)

Scenario walkthrough
- Need to build inferential model
- Signs were not coming out right, and as I added variables they were flipping
- Needed to change the values
- Tested variable of interest 
- Pulled variables out, one at a time, 


Recap 
- Generate a hypothesis for why it's looking different
- Confirm hypothesis by playing with data
- Attempting different solutions 


If you suspect collinearity
- Run a quick correlation table on your input variables
- Look at a scatterplot between the key problem variables
- Test a strategy for 
