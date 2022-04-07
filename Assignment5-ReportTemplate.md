**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:       | 30  |
|-----------------|---|
| Student Names:  | Agam Aulakh  |
|                 | Melanie Nguyen  |
|                 | Jeff Roszell  |
|                 | Heidi Schaefer  |

# Introduction
The purpose of this lab was to familiarize ourselves with different methods of reliability testing. Reliability growth testing was performed using ________ (SRTAT CASRE C-SFRAT SwEET). Reliability demonstration charts were used to check if MTTF is sufficient for the system's needs. The same hypothetical SUT was analyzed for each section.

# 

# Assessment Using Reliability Growth Testing 
### Reliability Growth Prediction - All Points (SRTAT)
![](media/reliability-growth-all-points.png)

To select the model that would provide the best fit for the project data, SRTAT was used to test each column of time data (execution time, failure identification work in person hours, computer time failure identification) using all available models (Geometric, Jelinski/Moranda De-Eutrophication, Littlewood and Varral's Bayesian Reliability, John Musa's Basic Execution Time, John Musa's Logarithmic Poisson, and Non-homogeneous Poisson). This method was used because CASRE provided no models to use for model ranking. Most models in SRTAT threw various errors when a prediction was attempted; however, we found that Littlewood and Varral's Bayesian Reliability model fit the execution time data best.

### Laplace Test (CASRE)
![](media/rdc-laplace-casre.png)

In order to determine the range of useful data, a Laplace test was conducted using CASRE. Execution time in hours was used for hours since last failure, and failure count was used for severity, as there was no severity ranking given. From the Laplace test, successive data points with Laplace Test Value between -2 and +2 were chosen as valid points. These data points were on time intervals 15-31. The reliability growth prediction was tested again with the new data points as shown below.

### Reliability Growth Prediction - Points Selected from Laplace Test (SRTAT)
![](media/reliability-growth-selected-points.png)

As shown in both reliability growth predictions (all points and selected points), as time increases, the number of failures increases more slowly. This shows that the SUT is becoming more reliable as time goes on.

# Assessment Using Reliability Demonstration Chart 

# 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques
Reliability growth testing allows for graphical representation of reliability trends. Different models can be used to determine a best fit graph for the data. These graphs can show whether reliability is increasing, decreasing, or stable. The sample size must be quite large to allow for an accurate trend to be determined.

Reliability demonstration charts are used to determine whether the SUT is acceptable to the developer and customer using risk probabilities and failure intensity estimation. One benefit is that different levels of risk and failure intensities can easily be experimented with, as shown in the results above. However, it does not calculate the reliability of the system, only whether or not the system is acceptable to the developer and customer. The sample size does not need to be as large as the sample size for reliability growth testing.

# How the team work/effort was divided and managed

# 

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
