# Customer Accept the Coupon? Practical Assignment 5.1


The Practical assignment aim was to differentiate between customers who accepted a driving coupon and those who didn't, using visualizations and probability distributions.

The dataset for this analysis can be found here: 
[Link to Coupons Dataset](/coupons.csv)


The analysis was conducted using Python programming language and the libraries pandas, seaborn, matplotlib, numpy and Sweetviz 

The specifics of the analysis, including the code, visualizations, comments, and observations, are available in the following Jupyter Notebook.

[Link to Jupyter Notebook](/AIMLPAA_51.jpynb)

## Exploratory Data Analysis:

The Sweetviz library was employed to conduct a thorough analysis of missing data, and the Python library was utilized for preliminary data exploration

[Link to SweetViz Report](/edareport.html)

The following potential data quality issues were identified:

#### Missing Data:
The ‘car’ attribute was dropped from the dataset for analysis because approximately 99% of its values were blank, offering little value. The other columns have less than 2% missing values, which will not have a significant overall impact.

#### Duplicate Data: 
There are 74 duplicate rows, which have been retained. As this is a survey, duplicate responses are expected and we are interested in every response..

## General Data Visualizations
![Image](/images/coupontypedistr.png)

<br>
<br>

![Image](/images/histtemp.png)


## Data Summary Points

#### General:
* A coupon was accepted approximately **57%** of the time.

#### Bar Coupon Specific:
*	Overall acceptance rate: **41%**
*	Acceptance rate for people who go to the bar three or fewer times a month: **53%**
*	Acceptance rate for people who go to the bar more than three times a month: **77%**
*	Acceptance rate for drivers who go to the bar more than once a month and are over 25 years old: **70%**
*	Acceptance rate for drivers who go to the bar more than once a month, have passengers who are not children, and have occupations other than farming, fishing, or forestry: **71%**
*	Acceptance rate for drivers who go to the bar more than once a month, have passengers who are not children, and are not widowed: **71%**
*	Acceptance rate for drivers who go to the bar more than once a month and are under 30 years old: **72%**
* Acceptance rate for drivers who go to cheap restaurants more than 4 times a month and have an income less than 50K: **45%**

## Hypotheses

 Based on the observations, we can hypothesize the following about drivers who accepted the bar coupons:

*	**High Frequency of Bar Visits:** Drivers who frequently visit bars, especially more than 3 times a month, are significantly more likely to accept bar coupons. This suggests a strong correlation between the frequency of bar visits and the likelihood of accepting related coupons, potentially due to a higher value placed on such discounts by regular patrons.
*	**Age Factor:** Younger drivers, particularly those under the age of 30, exhibit a higher acceptance rate for bar coupons. This could indicate that younger demographics are more inclined towards social outings like bar visits and are more receptive to discounts associated with such activities.
*	**Marital Status:** and Occupation: Drivers who are not widowed and have occupations outside of farming, fishing, or forestry are more likely to accept bar coupons. This might reflect lifestyle or social patterns where individuals in certain occupations or marital statuses have more social engagements or value leisure activities differently.
*	**Economic and Dining Preferences:** Drivers with specific economic and dining preferences, such as those who frequent inexpensive restaurants and have an income of less than 50K, have distinct acceptance rates. This could suggest that economic factors and personal dining habits influence the perceived value of bar coupons.
*	**General Acceptance Among Other Drivers:** The relatively lower acceptance rate among "all other drivers" indicates that there are specific demographic and behavioral traits that significantly influence the likelihood of accepting bar coupons. This group likely includes drivers who do not frequently visit bars or do not fit into the specific demographic profiles outlined above.

<br>

## Independent Investigation - Coffee House Coupon Declines

Further analysis focused on drivers who declined Coffee House coupons
<br>
<br>
![Image](/images/coffeehousedeclinebyage.png)

**Age:** The age groups of 21 and 26 years old are the most likely to decline Coffee House Coupons, The most declines for the ages 21 through 31st, delcines 47%. This suggests that younger adults in their early to mid-twenties are more inclined to decline these coupons.
<br>
<br>

![Image](/images/coffeehousedeclinebymaritalstatus.png)

**Marital Status:** Marital Status: The majority of declines come from individuals with a married partner (approximately 39%) and singles (approximately 37%). This indicates that marital status, particularly being married or single, plays a significant role in the likelihood of declining Coffee House coupons.
<br>
<br>

![Image](/images/coffeehousedeclinebyeducation.png)

**Education:** Individuals with a Bachelor's degree are the most likely to decline these coupons, making up approximately 37% of the declines, followed by those with some college but no degree (approximately 33%). This suggests a higher tendency to decline.
<BR>
<BR>
## Recommended Next Steps

Based on the analyses performed and the insights gained about drivers who accept bar coupons and those who decline Coffee House coupons, here are the recommended next steps to further understand the dataset and actions to take as a result of this increased understanding:

* **Segmentation Analysis:** Perform a deeper segmentation analysis to identify more nuanced segments within the dataset. This could involve looking at combinations of factors such as time of day, weather conditions, and location to understand how these variables influence coupon acceptance rates.

* **Predictive Modeling:** Develop predictive models to forecast coupon acceptance rates based on driver demographics, behaviors, and external factors.

* **A/B Testing:** Conduct A/B testing with different coupon designs, offers, and messaging to see which variations lead to higher acceptance rates among different driver segments. This can help refine marketing strategies and improve coupon effectiveness.

* **Economic Impact Analysis:** Assess the economic impact of coupon campaigns on business outcomes such as increased sales, customer retention, and brand loyalty. This analysis could help justify the investment in coupon campaigns and guide budget allocation.
