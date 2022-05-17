# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Background

Historically, standardised tests scores such as American College Testing (ACT) and Scholastic Aptitude Test (SAT) feature strongly in the admissions process for US colleges. Most US colleges required results from at least one of these tests for applicants to be considered for admission. However, there has been increasing public opinion that such tests are not fair and should be removed. Combined with the inherent difficulties of taking such large-scale tests due to the Covid-19 pandemic, numerous US Colleges have opted to be flexible with their admissions requirements; making standardised scores optional for the next few years. However, if students DO include these results, a large number of schools will still take them into consideration.

---

### Problem Statement
You are part of the academic staff of a **NEW** public high school in **New York**, and have been tasked to assess if standardized test should be adopted in your school.

---

### Methods

#### Datasets
Aggregate SAT and ACT scores and participation rates were extracted for year 2017, 2018 and 2019. Another dataset with US Colleges and their requirements for standardised test results were also retrieved. (See table below for data dictionary)

|DataSet|Feature|Type|Description|
|:---|:---|:---|:---|
|act_sat|participation|float|Participation rate of the US state for ACT or SAT tests in that year.|
|act_sat|state|string|US State|
|act_sat|composite|float|Average ACT test scores of the respective US state in that year.|
|act_sat|total|integer|Average SAT test scores of the respective US state in that year.|
|admission|school|string|Name of school|
|admission|test_optional|string|Yes: Test Optional and Test flexible schools <br/> No: Schools which require SAT/ACT, and schools which <br/> have specific conditions if applicants do not submit SAT/ACT <br/> TB: Test Blind, rests will not be considered even if submitted

Note: For the act_sat dataset, each feature is suffixed with the year that the data represents

#### Analysis performed
Summary statistics for all variables were computed. Data distributions were visualised using boxplots and histograms. Relationships between the two tests for participation rates, and test scores were explored using scatter plots. A heat map was also generated to obtain a high level view of the relationship across all variables.
Aggregate data was computed to understand the tolerance of US Colleges if no standardised tests were taken. General performance of New York in standardised tests was assessed through its relative performance to other states.

---

### Key findings
**Distributions:**
Distributions of participation rates for both tests are similar across the years. They cover the entire range of possible values, with clusters at the 0% and 100% participation rates. Participation rates for a specific test and state, is generally consistent across the years.

**Relationships between variables:**
There is a general trend that states with high participation rates in one test has low participation rates in the other test. This is **expected** as students are not likely to take both tests.

**College test policy:**
At least for 2021, almost 90% of colleges will allow applications without standardised test scores unconditionally. However, most of these colleges are not test blind, and will still consider standardised test scores if submitted. As such, students will still have many university options even if they have not taken standardised tests.

**Performance of New York in standardised tesets:**
At least for 2021, almost 90% of colleges will allow applications without standardised test scores unconditionally. However, most of these colleges are not test blind, and will still consider standardised test scores if submitted.

---

### Conclusion and recommendations
While online opinion and preliminary moves from colleges support the notion that standardised testing may be less consequential next time, it is clear that colleges still currently factor in standardised test results. Since the test scores are relevant and New York generally performs well in ACT, I recommend to incorporate ACT preparations in the school curriculum.
