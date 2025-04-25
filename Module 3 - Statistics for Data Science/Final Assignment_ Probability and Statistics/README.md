# Methodology for the Final Statistics Project for Data Science

## Objective

Define a topic and conduct a sample survey following the procedures below.

## General Procedures

- Groups will be formed with a minimum of **3** and a maximum of **5 students**;
- Each group will have a representative responsible for posting the names of the members on the Classroom board, where the work must be submitted;
- The evaluation is worth **zero to seven points**;
- The definition of the topic and objectives is the responsibility of each group;
- The **data frame** must contain at least **five fields** and **25 rows**, with at least **two numerical fields**;
- All analyses must be conducted in **Python** and presented during the class on **November 14**;
- The data and the notebook containing the scripts must be submitted **before the first team's presentation**, which should last approximately **10 minutes**;
- The order of presentation will be determined by a **draw**.

## Required Analyses

a) (Worth **1.0 point**) Build appropriate **tables and plots** for each variable in the data frame;  
b) (Worth **1.0 point**) Calculate the **mean**, **median**, **mode**, **standard deviation**, **coefficient of variation**, and **skewness** of the quantitative variables;  
c) (Worth **1.0 point**) Analyze the **normality** of the numeric data and whether there are any **outliers**;  
d) (Worth **1.0 point**) Compare the quantitative variables and describe which one is more **homogeneous**;  
e) (Worth **1.0 point**) Calculate the **95% Confidence Interval** for each field in the data frame;  
f) (Worth **1.0 point**) Compare the mean of a numeric field with a categorical field and assess if there is a **statistical difference at the 5% significance level**;  
g) (Worth **1.0 point**) Cross two categorical fields and assess if there is a **statistical difference at the 5% significance level**.

## Dataset

The dataset consists of official statistical data from the **11,538 athletes** who participated in the **2016 Rio de Janeiro Olympic Games**. It includes:

- Name  
- Nationality (3-digit code)  
- Gender  
- Date of birth  
- Height (in meters)  
- Weight (in kg)  
- Sport discipline  
- Number of gold, silver, and/or bronze medals  

**Source**: [Kaggle](https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Frio2016%2Folympic-games%2F)

### For disciplinary purposes:

- We computed the **age** of each athlete (as of August 2016) from their date of birth, generating a new column `age`;  
- We removed the columns `id`, `name`, and `dob`.
