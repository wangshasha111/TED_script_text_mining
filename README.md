# TED_script_text_mining

The project aims at applying machine learning techniques to the dataset ted_talks_en.csv for text mining within the context of gender analysis.

The script TextMining_NLP_TED.Rmd borrows heavily from the lecture notes of STAT 471 taught at Wharton School of Business, University of Pennsylvania in the spring of 2022.

In modern data mining, we often encounter the situation where a text may contain important, useful information about response of interest. Can we predict how likely a talk is given by a female based on the transript? One simple but effective way of learning from a text is through bag of words to convert raw text data into a numeric matrix. We first turn each text into a vector of frequency of words. The bag of words approach can be extended using the n-gram or k-skip-n-gram techniques to account for the semantics of word ordering. Then we apply existing methods that use numerical matrices to either extract useful information or carry out predictions. We will extend the regularization technique (LASSO) to classification problems.

The takeaway from the project is that males and females have different topics of interests and leverage different sets of words. The differences can be seen in word cloud intuitively, or can be quantitatively evaluated through LASSO regressions.

I output a R markdown file [TextMining_NLP_TED.Rmd](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.Rmd), with its PDF version [TextMining_NLP_TED.pdf](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.pdf) and its html version [TextMining_NLP_TED.html](https://github.com/wangshasha111/TED_script_text_mining/blob/main/TextMining_NLP_TED.html).





 
