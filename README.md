# Machine Learning Tasks

This repository contains solutions to four maching learning tasks as part of the assessment in the Machine Learning and Statistics module for the Higher Diploma in Data Analytics with Galway-Mayo Institute of Technology.

## About this Repository

The repository can be accessed [here](https://github.com/jennifer-ryan/machine-learning-tasks). Clicking the 'clone or download' button will allow you to download the repository to your machine. Use the 'git clone' command followed by the repository link in your machine's command line to create a local copy for review. Navigate to the folder containing the notebook with command prompt and type "jupyter notebook" to open file. 

The contents of this repository are:

1. A **README** file that outlines the project.
2. A **Jupyter Notebook** that contains the solutions to each of the tasks.
3. An **Excel Document** used in part for the standard deviation task along with **JPG files** containing screenshots of the Excel file in use.

## Python Libraries

For this project I use the following Python libraries:

- **pandas** to create and use dataframes.
- **numpy** to create and use numerical arrays.
- **scipy.stats** to access Chi Squared Test.
- **matplotlib.pyplot** and **seaborn** for plotting and visualisation.
- **sklearn** to access the Iris data set, K-Means Clustering algorithm and metrics.

## Tasks

1. Write a Python function called sqrt2 that calculates and prints to the screen the square root of 2 to 100 decimal places. Your code should
not depend on any module from the standard library1 or otherwise. You should research the task first and include references and a description of your algorithm.

2. The Chi-squared test for independence is a statistical hypothesis test like a t-test. It is used to analyse whether two categorical variables are independent. The Wikipedia article gives the table below as an example, stating the Chi-squared value based on it is approximately 24.6. Use scipy.stats to verify this value and calculate the associated p value. You should include a short note with references justifying your analysis in a markdown cell.

<center>
|   |A   |B   |C   |D   |Total   |
|---|---|---|---|---|---|
|White Collar   |90   |60   |104   |95   |349   |
|Blue Collar   |30   |50   |51   |20   |151   |
|No Collar   |30   |40   |45   |35   |150   |
|Total   |150   |150   |200   |150   |650   |
</center>
    
3. The standard deviation of an array of numbers x is calculated using numpy as np.sqrt(np.sum((x - np.mean(x))^2)/len(x)). However, Microsoft Excel has two different versions of the standard deviation calculation, STDEV.P and STDEV.S . The STDEV.P function performs the above calculation but in the STDEV.S calculation the division is by len(x)-1 rather than len(x) . Research these Excel functions, writing a note in a Markdown cell about the difference between them. Then use numpy to perform a simulation demonstrating that the STDEV.S calculation is a better estimate for the standard deviation of a population when performed on a sample. Note that part of this task is to figure out the terminology in the previous sentence.

4. Use scikit-learn to apply k-means clustering to Fisher’s famous Iris data set. You will easily obtain a copy of the data set online. Explain in a Markdown cell how your code works and how accurate it might be, and then explain how your model could be used to make predictions of species of iris. 
**Note**: This task was later updated to state that it should have been K-Nearest Neighbours rather than K-Means Clustering. The task had already been completed at the time so was not adjusted. 