# Predicting Obesity with Tree-based Methods
The aim of this project is to predict obesity based on a number of covariables. The performance of a single pruned decision tree, a Random Forest, bagging and boosting are compared using ROC curves and the AUC measure. You can find the code as well as the description of the whole process in obesity.html or obesity.Rmd (depending on your preferences). The dataset can be found at https://www.kaggle.com/datasets/adeniranstephen/obesity-prediction-dataset. 

## Repository Structure
```text
obesity-prediction/
│
├── obesity.Rmd                  # Main RMarkdown analysis file
├── README.md                    # Project documentation
├── data/                        # Data used in the analysis
│   └── [Obesity prediction.csv] # Dataset file
└── obesity.html                 # Rendered report
```

## Data

The dataset used in this project is stored in the `data/` folder.

Please note: the analysis uses relative file paths, so the project should run correctly as long as the repository structure is preserved and you have tidyverse installed.

## Required R Packages
The following packages are used: 

```{r}
library(rpart)
library(rpart.plot)
library(caret)
library(randomForest)
library(ROCR)
library(Metrics)
library(gbm)
library(tidyverse)
```

Install missing packages using install.packages("...").
