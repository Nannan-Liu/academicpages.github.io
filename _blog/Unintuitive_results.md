---
title: "When your statistical results are unintuitive or counterintuitive"
excerpt: "This is in response to an interview question."
collection: code
---


> Successful modeling of a complex data set is part science, part statistical methods, and part experience and common sense [(Hosmer, Lemeshow, & Sturdivant, 2013, p. 89)](https://www.wiley.com/en-us/Applied+Logistic+Regression,+3rd+Edition-p-9780470582473).

 1. Individual plots  

    a) Always do dependent variable ~ an independent variable first, use [Yiqing Xu's checklist](https://yiqingxu.org/public/checklist.pdf)  
   
    b) Take a look at outliers---maybe your coding is wrong.  

 3. Model assumptions  

    a)  Normal distribution: Almost all variables in T & I and linguistics, e.g. word legth, dimension scores, and information density, have non-normal distributions, so do Shapiro-Wilk first, and use non-parametric statistics, e.g. Kruskal-Wallis test (not one-way ANOVA) and Spearman's rank correlation (not Pearson's correlation).  
   
    b) Transform your data when needed (see many examples in [Coupé, 2019](https://www.frontiersin.org/articles/10.3389/fpsyg.2018.00513/full))  
   
    c) Adequate number of samples: Use Fisher-Yates exact test when the frequency in one cell is smaller than 5, not Pearson's chi-square test

 4. Variable selection  
 
    a) Always go for multivariate designs---monofactorial studies "have virtually nothing to contribute to corpus linguistics" ([Gries, 2018, p. 295](https://benjamins.com/catalog/jsls.00005.gri)) and linguistics in general. Never go feature shopping!  
   
    b) Choose features that are meaningful in relation to the language system, not the "teddy bears" (Cf. [Type III error](http://web.stanford.edu/group/bps/cgi-bin/wordpress/wp-content/uploads/2015/06/Tate.pdf))  
   
    c) [Omitted variable bias](https://stats.stackexchange.com/questions/157159/logistic-regression-results-coefficients-counterintuitive), which cannot be detected statistically. Gather your independent variables outcome-blindly!  

 5. Model evaluation  

    a) Report effect sizes, aim for "good to excellent" model performances  
   
    b) Check VIFs, try removing interactions that are not absolutely necessary  
    
    