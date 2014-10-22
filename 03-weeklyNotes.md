# Notes: week 3

### Types of Data Science Questions
- Descriptive 
    - Just describe the Data
    - Common in census data
    - Description & interpretation are different steps
    - Descriptions can usually not generalize w/o modeling
- Exploratory analysis
    + good for discovering new connections
    + useful for defining future studies
    + not the final say
    + alone it should not be use for generalizing/predicting
    + **Correlation does not imply Causation**
    + i.e. exploring space images repositories
- Inferential analysis
    + Goal of using a small sample to say something about the bigger picture
    + goal of statistical models
    + involves estimation both the quantity you care about and your uncertainty about your estimate
    + depend heavily on both population and sample scheme
    + i.e. estimation the effects of air pollution on life expectancy
- Predictive Analysis
    + Goal of using the data on some objects to predict values for another object
    + if *X* predicts *Y* it does not mean that *X causes *Y*
    +  Accurate prediction depends heavily on measuring the right variables
    +  More data w/simple models work really well
    +  Prediction is very hard, especially about the future references
- Causal analysis
    + Goal of finding out what happens to one variable when you chance another
    + usually requires randomized studies
        * non-random approaches are complicates
    + relationships are defined as average effects, but may not apply to every subject
    + Causal models are usually the "Gold Standard" for data analysis
- Mechanistic analysis
    + Goal is to understand the exact changes in variables that lead to changes in other variable for individual objects
    + hard to infer, except in simple situations
    + usually models by deterministic set of equations
    + random component of the data is the measurement error
    + if equations are know but the parameter are not, they may be inferred with data analysis

### What is Data
- Wikipedia
    + "Data are values of quantitative variables, belonging to a set of items"
    + **Set of items** sometimes called a population
    + **Variables** a measurement of characteristics of an item
    + **Qualitative** Country or origin, sex, treatment
    + **Quantitative** Height, weight, blood pressure
-   What does data look like
    + Data is usually in the form of massive raw dumps
    + Could be in the from of an API
    + Medical record
    + i.e. text file from which you need to extract information
    + Video or Audio file
    + API or spreadsheet from Government files
    + **Data usually is not neat**
- The Question you are trying to ask
    + The most import aspect of Data Science, behind the data
    + often the data will limit the question
    + Having the data can't save you if you don't have a question
    + **You must be driven by your Question not the fact that you have data**

###What about Big Data
- How much data is there
    + We are producing enormous amounts of data but only and small amount can really be used to answer questions
    + Some Data is so large is can't be stored on a laptop
    + Most *Data* questions don't involve these huge amounts of data
- Why Big Data Now
    + It's now possible to gather and analyze much more data much more quickly, but you must consider if this is really worth it
- Big or Small you need the **Right** data
    + "The data may not contain the answer. The combination of some data and an aching desire for an answer does not ensure that a reasonable answer can be extraction from a given body of data..." **-John Tukey"**
        * No matter how big they are

###Experiential Design
- You should care because bad studies, however exciting, can lead to further work being done based on flawed science or even litigation
- Care about the analysis plan - pay attention to all aspects of the the plan, know the key issuers in the design
- have a plan for data sharing
- Large amounts of data can be shared via a data sharing plan
        *  Leek Group
-  Formulate you question in advance
    +  Question: Dose changing the text on the website determine the donations
- Statistical inference
    + The **Population** is all possible donors
    +  They would select a small sub-set with a **Probability** argument, to show one version or the other
    +  Then calculate **Descriptive Statistics**, i.e. average amount of donation over a certain number of visits
    +  Use **Inferential Statistics** to determine if the results seen in the test subjects would play out in the population
-   Variability
    + You may see widely varying ranges within the results of one variable of the test
    + You may not see little variability within one variable but it still may not be clear if the changing the variable has an effect
    + you hope to see clearly decisive and data with little variability
- Confounding
    + When one variable seem correlated with another but not is not the direct effect
    + i.e Shoe size and literacy
        * the variable age is the confounder for the relationship between shoe size and literacy
    +   You must pay attention to the other variable that may be playing a role
    + **Correlation is not causation** and observed correlation may not be a actual relationship
    + This called **Spurious correlation**
    + You must prove to yourself that you findings are not the result of some variable(s) you didn't measure
- Randomization and blocking - one way to deal with confounders
    + Fix a bunch of variables
    + **Stratify**
        * use all other variables equally with both test variables
    + **Randomization** - *Flip a coin* to assign a subject to a group
        * ensure any test or treatment is given to a random subject and there are no confounder that influenced there group placement
- Prediction
    + Use results learned from past events to build a **Predictive function**
    + Prediction vs. inference
        * for prediction data sets need to be significantly separated
        * Consider the relative size of effects
- Prediction key quantities
    + **Sensitivity** `P( positive test | disease )`
    + **Specificity** `P( negative test | no disease )`
    + **Positive Predictive Value** `P( disease | positive test )`
    + **Negative Predictive Value** `P( no disease | negative test )`
    + **Accuracy**          `P( correct outcome )`
- Be aware of Data Dredging
    + keep digging into each variable of your data to find the result you are looking for
- Summary
    + Good Experiments
        * Have Replication
        * Measure Variability
        * Generalize to the problem you care about
        * Are Transparent
    + Prediction is not inference 
        * both are important
    + Beware of data Dredging