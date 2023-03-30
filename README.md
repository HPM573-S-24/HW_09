# Homework Assignment 9

**Note**: For this homework, feel free to use any part of the code in 
the [Lab_Calibration](https://github.com/HPM573/Lab_Calibration) repository. 

**Overview**:  Many clinical studies last for a limited number of years and hence, 
cannot produce statistics on patient survival time. 
Instead, they report the percentage of participants who survived beyond, for example, 5 years. 
In this homework, we would like to calibrate our survival model using the results of 
a clinical study that followed a cohort of 573 patients over 5 years. 

**Problem 1: Five-Year Survival (Weight 1)**. 
Modify the survival model so that you can get the 
"percentage of patients survived beyond 5 years" after simulating a cohort. 

**Problem 2: Likelihood Assumption (Weight 1)**. 
If the probability of 5-year survival is _q_, what probability distribution 
"the number of participants that survived beyond 5 years in a cohort of _N_ participants" would follow? 
Make sure to also specify the parameters of this distribution. 
_Hint_: Review section 11.3 of class notes.

**Problem 3: Likelihood Calculation (Weight 1)**: 
If our survival model represents the reality, then the 
"percentage of patients survived beyond 5 years" (calculated in Problem 1) 
will represent the true probability of 5-year survival (_q_ in Problem 2). 
Write a Python statement to calculate the likelihood that 
a clinical study reports 400 of 573 participants survived at the end of the 5-year study period 
if 55% of the patients in our simulated cohort survived beyond 5 years?
_Hint_: Review the list of discrete probability distributions available in Python 
[here](https://docs.scipy.org/doc/scipy/reference/stats.html). 
Use the pmf method (which returns probability mass function) on the distribution you selected in Problem 2. 

**Problem 4: Calibration (Weight 3)**. 
Calibrate the survival model (with patient cohort size of 1,000) 
using the results of the clinical study described above 
(i.e. 400 of 573 participants survived at the end of the 5-year study period). 

**Problem 5: Projection and Parameter Estimation (Weight 3)**. 
Use the calibrated model to estimate the mean survival time (and the 95% projection interval) of the cohort of size 1,000. 
Report the estimated annual mortality probability and the 95% credible interval. 

**Problem 6: Projection (Weight 1)**. 
Recalibrate the model against a clinical study that reports 800 of 1146 participants 
survived at the end of the 5-year study period. 
What changes do you observe in the credible interval of the estimated annual mortality probability 
and in the projection interval of the mean survival time? 
