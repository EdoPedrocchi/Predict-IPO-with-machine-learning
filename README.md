# predict-IPO-with-machine-learning

When a company decides to make an IPO is a crucial moment.
Success or failure? life or death?

What if it were possible to develop a machine learning model that could predict what will happen after the IPO?

I tried to create it. could i have succeeded?

## BEFORE START

This is a build in public project.
What it means?
I'm at the start of my journey and i want to improve my skill constantly.
I created a first model with various strengths and weaknesses and as time goes by I will improve my skills by creating an ever better models.
Each model created will remain published in this repository to document my growth and the growth of this project.

WHY THIS PROJECT?

1. improve my coding skill in Python
2. improve my data science and machine learning skill
3. apply the financial analysis skills learned during my studies
4. understand how to automate the  financial statements analysis with python
5. more important: understand if it is possible to predict success or failure of a company IPO

technology used: Python,YahooFinance Api

If you are interested in more information about the project, want to contribute or want to give me advice, please contact me.

[Click here](https://github.com/EdoPedrocchi/Predict-IPO-with-machine-learning/blob/main/Code) to copy the code, after this you can easly paste and launch it on your IDE and view the magic!

In alternative, [click here](https://github.com/EdoPedrocchi/Predict-IPO-with-machine-learning/blob/main/code.with.results.pdf) to view the code and the results of it remaining on Github

Ok, I'm done. Now we can start with the description of the project

## TABLE OF CONTENTS
### - Dataset
### - EDA
### - Machine learning models
### - Conclusion

## Dataset used
the dataset is compsoed by companies that made an IPO that was either a success or a failure.
Of these companies, I analyzed the financial statements for the year prior to the IPO and calculated indicators that are commonly used in financial analysis.
The indicators used are as follows:

-ROI

-ROS

-Capital turnover

-Ebitda analysis

-DSO

-IPO (0=fail, 1=success)

the goal is thus to understand whether companies that succeed or fail in IPOs are accumulated by the same financial value.

Before continuing: the dataset consists of only 17 companies, which means that the ML models developed will not be very accurate.
Finding these kinds of companies and analyzing their financial statements takes time.
So the number of data will increase over time, stay tuned.

##EDA

The datasets were analyzed separately:
-a df for successful companies.
-a df for the unsuccessful companies

**Visualizations:**

  - **Histograms:** This visualization method is employed to showcase the distribution of each variable. Histograms are effective in providing an overview of the frequency and concentration of data points within different ranges of financial ratios.

  - **Boxplots:** The use of boxplots is directed at identifying outliers. Boxplots offer a clear representation of the spread of data, highlighting any extreme values or anomalies that may impact the analysis.

**Correlation Analysis:**

This phase involves exploring the relationships between different financial ratios

- **Correlation Matrix:** By creating a correlation matrix, the project aims to quantify and visualize the degree of association between various financial variables. This matrix can reveal patterns of correlation or dependence, aiding in the identification of key factors influencing IPO success(or failure).

- **Scatter Plots:** To complement the correlation matrix, scatter plots are used to visually represent pairwise relationships between specific variables.These plots offer a more intuitive understanding of how two variables interact, providing additional insights.

Want to see the graphs obtained? [click here](https://github.com/EdoPedrocchi/Predict-IPO-with-machine-learning/blob/main/code.with.results.pdf)

## Machine learning models

first data were divided into training and test dataset. After, I trained 2 different models and compared the results.

### Random forest

This model obtained an accuracy of 0.6.
To view the confusion matrix [click here](https://github.com/EdoPedrocchi/Predict-IPO-with-machine-learning/blob/main/code.with.results.pdf)

According to the random forest the most significant variables are (in order from most significant to least significant):

1.capital turnover

2.EBITDA analysis

3.ROS

4.DSO

5.ROI

### SVM

This model obtained an accuracy of 0.4.
To view the confusion matrix [click here](https://github.com/EdoPedrocchi/Predict-IPO-with-machine-learning/blob/main/code.with.results.pdf)

## Conclusion

Too early to talk about the optimal model or parameters to be improved.
Currently, the first goal of the project is to enlarge the dataset.
Then new models will have to be developed, financial parameters added.

above all, it will be necessary to start considering other variables, such as macroeconomic situation, geographical location, sector.

see you soon
