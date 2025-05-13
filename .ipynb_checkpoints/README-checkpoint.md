![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Advanced Tableau Visualization

https://public.tableau.com/app/profile/claudio.do.prado/viz/lab-tableau-advanced_17471305779260/CustomerDataAnalysisDashboard?publish=yes

### Trend Lines Model

A linear trend model is computed for sum of Income given sum of Customer Lifetime Value.  The model may be significant at p <= 0.05.

 - Model formula:	( Customer Lifetime Value + intercept )
 - Number of modelled observations:	9134
 - Number of filtered observations:	0
 - Model degrees of freedom:	2
 - Residual degrees of freedom (DF):	9132
 - SSE (sum squared error):	8.42419e+12
 - MSE (mean squared error):	9.22492e+08
 - R-Squared:	0.0005937
 - Standard error:	30372.5
 - p-value (significance):	0.0198749

### Individual trend lines:

 - Panes -	                                  - Line - 	                  - Coefficients - 
 - Row - 	      - Column -                  - p-value - 	 - DF - 	    - Term -                 - Value - 	     - StdErr - 	- t-value -  - p-value - 
  Income	      Customer Lifetime Value	   0.0198749	  9132	   Customer Lifetime Value	      0.107732	     0.0462548	      2.32911	  0.0198749
	                                                                       intercept	                36795	       487.948	      75.4077	  < 0.0001

### Key Findings:

Model Significance:
The p-value for the overall model is approximately 0.0199, which is less than 0.05, indicating the model is statistically significant. This suggests that Income is a meaningful predictor of Customer Lifetime Value.

### Coefficient (Slope):

The coefficient for Income is approximately 0.108, meaning that for every additional unit (e.g., dollar) of income, the Customer Lifetime Value increases by about $0.108 on average.

### Intercept:

The intercept value is roughly 36,795, which represents the estimated Customer Lifetime Value when Income is zero (though this may not have practical meaning depending on data context).


### Model Fit (R-Squared):

The R-squared is very low (~0.0006), indicating that Income explains only a tiny portion of the variability in Customer Lifetime Value. Therefore, while the relationship is statistically significant, Income alone is a weak predictor of Customer Lifetime Value.

### Implication:

Since the model is statistically significant but explains very little variation, there might be other stronger factors influencing Customer Lifetime Value that are not included here.

### Summary:

The analysis indicates a significant but weak relationship between Income and Customer Lifetime Value. While higher income is associated with higher CLV, the effect size is small, and income alone doesn't account for much of the variability in CLV. For better predictive accuracy, consider including additional variables.

### Learning Outcomes

Upon completion of this lab, you will be able to:

- Create a Choropleth map to analyze geographical data.
- Construct and interpret a regression plot to understand the relationship between two quantitative variables.
- Utilize boxplots to compare distributions and identify outliers in the context of vehicle size categories.
- Assemble a comprehensive dashboard that incorporates a variety of chart types.
- Craft a story in Tableau that summarizes your analytical findings.

### Instructions

Continue your exploration of Tableau's advanced visualization capabilities using the `tableau-lab.tbwx` from the previous lab.

1. **Choropleth Map**: Design a Choropleth map sheet to display the distribution of customers across different **States**. Utilize color density to represent the number of customers, providing an at-a-glance view of regional customer bases.

2. **Regression Plot**: Develop a regression plot sheet that examines the relationship between **Customer Lifetime Value** and **Income**. Interpret the regression line to understand how these variables correlate.

3. **Boxplot Analysis**: Create a boxplot sheet that relates **Total Claim Amount** to **Vehicle Size**. Use this visualization to assess the spread of claim amounts and identify any outliers by vehicle size category.

4. **Dashboard Creation**: Combine the above charts into a unified dashboard. Ensure that the dashboard is organized and allows for interactive exploration of the data.

5. **Story**: Synthesize your analysis into a Tableau story. Construct a narrative that guides viewers through your key findings, providing context and insights drawn from the visualizations.
