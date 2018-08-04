# Analysis of COMPAS 

For my senior year thesis, I analyzed multiple academic papers and articles regarding racial bias in a widely used recidivism model called COMPAS. The initial study was published by ProPublica (PP) and the authors made their dataset available for public use.

You can access my thesis paper in my website: http://www.domaghale.com/thesis-paper/

The aim of my study was to help a wider audience to understand the depth and complexity of the topic. There is not just one way of looking at bias and policy choices are crucial to reduce bias. Much of my work was understanding and recreating the analyses in PP’s article and the responses that followed. I wrote a thesis paper describing my theoretical and empirical study on the topic of bias in data and how bias is reflected in models that learn from those data.

I downloaded the dataset from GitHub. The dataset contains information on 18,610 people in Broward County, FL who were scored with COMPAS during years 2013 and 2014. The information includes demographics (race, age, gender), criminal history (prior arrests), COMPAS scores and screening dates. I used RStudio and the R Language as my analysis tool. A large part of the analysis process went into data wrangling and exploratory data analysis because I wanted to test whether people with similar criminal history were assigned different scores.

Accuracy alone does not define fairness of the model. The different types of errors made by a prediction have different implications depending on goal of the model. In case of criminal justice system, we do not want to lock up innocent people hence we must reduce false positive error. I applied five distinct statistical tests to test for bias in the model. For the sample dataset I found that COMPAS model satisfies some fairness criteria and fails to satisfy others. Mathematically, it is not possible to satisfy all criteria for groups that have different base rate (reality).

In theory predictions do not affect the reality, but in practice predictions do affect the reality when decisions such as supervision level, release from custody or length of sentencing are based on those predictions. Therefore the algorithms that assign these scores (no matter the complexity) need to be fully explained so that the decision makers don’t misunderstand or misuse the models output.
