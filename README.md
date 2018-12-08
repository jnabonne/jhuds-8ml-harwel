# Human Activity Recognition (HAR) - Weight Lifting Exercises (WLE) Study

## Context
Using devices such as Jawbone Up, Nike FuelBand, and Fitbit it is now possible to collect a large amount of data about personal activity relatively inexpensively. These type of devices are part of the quantified self movement – a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. One thing that people regularly do is quantify how much of a particular activity they do, but they rarely quantify how well they do it.

## Objectives
This study try to answer this using data from accelerometers on the belt, forearm, arm, and dumbell of 6 participants. They were asked to perform barbell lifts correctly and incorrectly in 5 different ways. More information is available from the WLE section of the [website](http:/groupware.les.inf.puc-rio.br/har) form which comes the datasets.

_Sources: Velloso, E.; Bulling, A.; Gellersen, H.; Ugulino, W.; Fuks, H. Qualitative Activity Recognition of Weight Lifting Exercises._  
_Proceedings of 4th International Conference in Cooperation with SIGCHI (Augmented Human '13) . Stuttgart, Germany: ACM SIGCHI, 2013._

## Method and results
Models have been trained and compared (using cross-validation).  
The best one, random forest, ended-up having excellent result with over 99% accuracy _(out-of-sample error << 1%)_.

## Notes
The dataset files [pml-training.csv](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv) and [pml-testing.csv](https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv) have already been downloaded.

In order to boost caret training processes (especially for decision tree and radom forest), parallel computing is used following instructions found through the forum on [github](https://github.com/lgreski/datasciencectacontent/blob/master/markdown/pml-randomForestPerformance.md)
