# Using R to Predict the TED Talker's Gender

## Goal of the project
The project aims to apply machine learning techniques to the dataset ted_talks_en.csv for text mining within the context of gender analysis.

## Motivation
The script TextMining_NLP_TED.Rmd borrows heavily from the lecture notes of STAT 471 taught at the Wharton School of Business, University of Pennsylvania, in the spring of 2022.

In modern data mining, we often encounter the situation where a text may contain important, useful information about response of interest. Can we predict how likely a talk is given by a female based on the transript? One simple but effective way of learning from a text is through bag of words to convert raw text data into a numeric matrix. We first turn each text into a vector of frequency of words. The bag of words approach can be extended using the n-gram or k-skip-n-gram techniques to account for the semantics of word ordering. Then we apply existing methods using numerical matrices to extract useful information or carry out predictions. We will extend the regularization technique (LASSO) to classification problems.

## Software
R 4.1.3 with packages dplyr, ggplot2, tm, SnowballC, RColorBrewer, wordcloud, glmnet, randomForest, ranger, data.table, qdap, tidyverse, tidytext, wordcloud, janitor, treemap, radarchart, SnowballC, magrittr, wesanderson, tm, lubridate, plotly, htmlwidgets, IRdisplay, topicmodels, repr, gender, genderdata

More specifically, 
## Packages used

1. Text Mining Packages 
   + [`tm`](https://cran.r-project.org/web/packages/tm/tm.pdf): a popular text mining package
   + Note: Ingo Feinerer created text mining package `tm` in 2008 while he was a phd student at TU Vienna. Users can deploy `Hadoop` to handle large textual data.
   - `SnowballC`: For Stemming 
2. Word Cloud Packages
   - `RColorBrewer`: a package for color palette
   - `wordcloud`: a package for creating wordcloud
3. LASSO and Random Forest packages 
   - `glmnet` 
   - `randomForest` 
   - `ranger`
   - [`stringr`](http://edrub.in/CheatSheets/cheatSheetStringr.pdf): useful string package

My favorite packages: `ggplot2`, `dplyr`, `stringr` (string manipulations), `lubridate` (handling date-time). Most of them are aggregated into `tidyverse`.
  

## Model - LASSO (least absolute shrinkage and selection operator)
In statistics and machine learning, lasso (least absolute shrinkage and selection operator; also Lasso or LASSO) is a regression analysis method that performs both variable selection and regularization in order to enhance the prediction accuracy and interpretability of the resulting statistical model. After turning a text into a vector, we can then use logistic regression models and LASSO to explore the relationship between `gender` and `text`. 

## Takeaway
The takeaway from the project is that males and females have different topics of interests and leverage different sets of words. The differences can be seen in word cloud intuitively, or can be quantitatively evaluated through LASSO regressions.


## Outputs
I output a R markdown file [TextMining_NLP_TED.Rmd](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.Rmd), with its PDF version [TextMining_NLP_TED.pdf](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.pdf) and its html version [TextMining_NLP_TED.html](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.html).





 
