# OutlierDetection

An outlier is an observation point that is distant from other observations in statistics. An outlier may be due to variability in the measurement or it may indicate the experimental error. An outlier can cause serious problems in statistical analyses and affect the analysis results. 

This project will use two methods to examine the outliers: standard deviation methods and interquartile range method.

The standard deviation methods suggest within one standard deviation of the mean will cover 68% of the data, two Standard Deviations from the Mean: 95% and Standard Deviations from the Mean: 99.7%. A value that falls outside 3 standard deviations is a rare observation. 

As the standard deviation method could be used in the normal distribution, the interquartile range method could deal with a non-Gaussian distribution sample. The interquartile range  equals to the difference between 75th and 25th percentiles, or between upper and lower quartiles. The IQR can be used to identify outliers by defining limits on the sample values that are a factor k of the IQR below the 25th percentile or above the 75th percentile.

Below is the overall framework of this project:

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/Outlier%20Detection%20Framework.png" height="400" width="900">


# Parametric methods: Univariate 

## Create a dummy data frame with normal distribution 

For the parametric methods, create a dummy data frame where features have normal distributions.

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/dummydf.png" height="350" width="550">

## Show normal distribution of the dummy dataframe

Use histograms to show the normal distribution of all 4 features. 

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/normal%20distrobution%20dummy%20df.png" height="500" width="550">

## Test Outliers according to the Standard Deviation

Identify the outliers that falls outside 3 standard deviations and visualize them in the histogram. 

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/Feature%200%20Distribution.png" height="500" width="550">

## Compare Standard Deviation and Interquartile Range

Compare the standard deviation method and interquartile range method using a heat map. Identify the outliers at 2 ,3, 4 standard deviations and 1.5 , 2.5 ,3.5 IQR. 

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/Heatmap%20show%20outliers%20at%20different%20sd.png" height="500" width="900">

## Display the distribution of Feature 0 in Dummy Data Frame ( different SD level)

Select the feature 0 from the dummy data frame and make a detailed visualization at different standard deviation level, where there red area suggests the data fall outside 2 standard deviations, green area suggests the data outside 3 standard deviations and yellow area suggests the data outrside 4 standard deviations.

<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/feature%200%20histogram%20at%20different%20sd.png" height="400" width="600">

# Non parametric Methods : Univariate
 For this part, use a new dataset descrbing the housing market in Melbourne.
 
### Data Desciption
 <img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/housingdes.png" height="250" width="900">

### Histogram 
<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/housinghis.png" height="500" width="700">

## Isolation Forest
<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/isolation%20forest.png" height="400" width="750">

# Parametric Methods : Multivariate (Using Elliptic Envelope)
<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/elliptic%20envelope.png" height="400" width="600">

# Non parametric Methods : Multivariate 
## DBSCAN
<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/dbscan.png" height="450" width="600">

## Local Outlier Factor
<img src="https://github.com/rliu49/OutlierDetection/blob/master/Imgs/local%20outlier%20factor.png" height="450" width="600">


