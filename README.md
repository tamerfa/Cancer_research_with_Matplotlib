# Matplotlib - The Power of Plots

## Background

![Laboratory](Images/Laboratory.jpg)

This project contains data about a fictional pharmaceutical company that specialises in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As per the dataset, 249 mice identified with SCC tumour growth were treated through a variety of drug regimens. Over the course of 45 days, tumour development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. Here I generated all of the tables and figures needed for the technical report of the study, as well as a summary of the study results.

## Steps

* The data consists of two CSV files:
<br/>1-"Mouse_metadata.csv" which contains information about each mouse's age, weight, sex, and the drug used for treating it.
<br/>2-"Study_results.csv" which contains daily information about the tumor size for each mouse.
* Before beginning the analysis, I checked the data for any mouse ID with duplicate time points and removed any data associated with that mouse ID.

* Generated a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumour volume for each drug regimen.

* Generated a bar plot using two methods to show the number of total mice for each treatment regimen throughout the course of the study (Both methods should give identical plots):
 <br/>1- Pandas's `DataFrame.plot()` 
 <br/>2- Matplotlib's `pyplot`

* Generated a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` to show the distribution of female or male mice in the study.


* Calculated the final tumour volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then calculated the quartiles and IQR and quantitatively determined if there are any potential outliers across all four treatment regimens.

* Using Matplotlib, I generated a box and whisker plot of the final tumour volume for all four treatment regimens, and highlighted the potential outliers in the plot by changing their colour and style.

* Selected a mouse that was treated with Capomulin and generated a line plot of tumour volume vs. time point for that mouse.

* Generated a scatter plot of mouse weight versus average tumour volume for the Capomulin treatment regimen.

* Calculated the correlation coefficient and linear regression model between mouse weight and average tumour volume for the Capomulin treatment. Then Plotted the linear regression model on top of the previous scatter plot.