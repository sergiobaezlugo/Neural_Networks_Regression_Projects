# Neural Networks Regression Projects
This repository contains a few projects where Neural Networks were used to solve regression problems.

## Life Expectancy Project

### Overview
The [dataset](https://github.com/sergiobaezlugo/Neural_Networks_Regression_Projects/blob/main/life_expectancy.csv) used in this project is from The World Health Organization (WHO)’s Global Health Observatory (GHO) data repository. It contained 22 columns and 2938 entries. Here's a preview of such dataset:

|index|Country|Year|Status|Adult Mortality|infant deaths|Alcohol|percentage expenditure|Hepatitis B|Measles | BMI |under-five deaths |Polio|Total expenditure|Diphtheria | HIV/AIDS|GDP|Population| thinness  1-19 years| thinness 5-9 years|Income composition of resources|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|0|Afghanistan|2015|Developing|263\.0|62|0\.01|71\.27962362|65\.0|1154|19\.1|83|6\.0|8\.16|65\.0|0\.1|584\.2592099999999|33736494\.0|17\.2|17\.3|0\.479|
|1|Afghanistan|2014|Developing|271\.0|64|0\.01|73\.52358168|62\.0|492|18\.6|86|58\.0|8\.18|62\.0|0\.1|612\.696514|327582\.0|17\.5|17\.5|0\.476|
|2|Afghanistan|2013|Developing|268\.0|66|0\.01|73\.21924272|64\.0|430|18\.1|89|62\.0|8\.13|64\.0|0\.1|631\.744976|31731688\.0|17\.7|17\.7|0\.47|
|3|Afghanistan|2012|Developing|272\.0|69|0\.01|78\.18421529999999|67\.0|2787|17\.6|93|67\.0|8\.52|67\.0|0\.1|669\.959|3696958\.0|17\.9|18\.0|0\.4629999999999999|
|4|Afghanistan|2011|Developing|275\.0|71|0\.01|7\.097108703|68\.0|3013|17\.2|97|68\.0|7\.87|68\.0|0\.1|63\.537231000000006|2978599\.0|18\.2|18\.2|0\.4539999999999999|

With the exception of the "Country" variable, all the other variables above were used to perform regression on the "Life Expectancy" variable.

### NN Architecture and Hyperparameters
A simple Feedforward Neural Network with one hidden layer (64 units and ReLu activation function) was used.

Adam optimization was used with a learning_rate = 0.01, batch_size = 1, loss = mean_squarred_error, and epochs = 40.

[Code](https://github.com/sergiobaezlugo/Neural_Networks_Regression_Projects/blob/main/life_expectancy.ipynb)

### Performance
The model achieved a mean_squarred_error = 8.187067985534668 and mean_absolute_error = 2.0607926845550537 on the test data.
