# Comparing Teenage Birth Rates in Baltimore, MD and Charleston, SC Based on Average Household Income
## Background
The teenage birth rate is the fraction of women who gave birth to a child while they were between the ages of 13-19. Many social scientists view a high teenage birth rate as indicative of gender inequality, as teen pregnancies can [stifle women's educational and professional opportunities](https://www.mcser.org/journal/index.php/jesr/article/viewFile/542/567). The issue was especially prevalent in my culturally conservative hometown of Charleston, South Carolina. I wanted to see how Charleston's statistics on teenage birth rates compared to Baltimore with regard to other factors like household income. Prior to my data collection, I hypothesized that lower household income would be directly proportional to teenage birth rates and that Charleston would have a higher teenage birth rate in tracts with similar household incomes to Baltimore due to factors like cultural stigma against women's reproductive care.
## Question
Is there an association between household income and teenage birth rates in Charleston, SC and Baltimore, MD? 
## Data Sources
I derived all of my data from Opportunity Atlas. The data is categorized as follows:
- [Average Household Income by Population Tract in Baltimore](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Baltimore_Income_Data.xlsx)
- [Average Household Income by Population Tract in Charleston](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Charleston_Income_Data.xlsx)
- [Teenage Birth Rates by Population Tract in Baltimore](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/baltimore_teen_pregnancy.xls)
- [Teenage Birth Rates by Population Tract in Charleston](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/charleston_teen_pregnancy.xltx)
## Data Analysis
Using the aforementioned metrics, I compared household income data in each of the cities' documented population tracts with the same tracts' teenage birth rate. For the teenage birth rate, I used the average rate for all income levels within a tract. For the income data, I used the average household income within a tract. 

The following chart is from my original mini-project #1. The graph's x axis lists the population tracts in Charleston, SC from highest to lowest average household income. The blue line models this arrangement of tracts by household income, while the red line graphs the population tracts' corresponding teenage birth rate. 

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Income_Birth_Correlation_Charleston.png)

This chart, also taken from my original mini-project, models the association between household income and teenage birth rates in Baltimore, MD:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/eb208fa0d8972fdad16272bd8874958a39c09db4/Income_Birth_Correlation_Baltimore.png)

Both charts indicate that, on average, population tracts with lower household incomes have higher teenage birth rates. The fact that household income is calculated based on parental income also indicates that girls in poorer households are more likely to become pregnant. The data does not, however, provide conclusive insight into whether or not teenage pregnancies reduce a woman's income. 

On average, Charleston had lower teenage birthrates and higher average household incomes than Baltimore. However, population tracts in Baltimore with a similar average household income to tracts in Charleston featured higher teenage birthrates. Baltimore's highest earning tract ($27,936) had a teenage birthrate of 45%, whereas Charleston's lowest earning tract ($27,207) had a teenage birthrate of 30%. 

My updated graphs for mini-project #4 exhibit similar trends in the data. The following graph, made in plotly express, illustrates teenage birth rates by the household incomes of each tract in Charleston, SC. 

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Proj%204%20Charleston%20Graph.png)

This plotly graph models the association between teenage birth rates and household income in Baltimore, MD:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Proj%204%20Baltimore%20Graph.png)

## Key Takeaways 
My data analysis indicates that population tracts with lower household incomes have higher teenage birth rates in both Baltimore and Charleston. However, the data refuted my hypothesis that Charleston would have a higher teenage birth rate than Baltimore in tracts with equivalent incomes due to factors like stigma against women's reproductive care. 

Baltimore's higher-on-average teenage birthrates suggest that other factors might influence the metric. [In my midterm project](https://github.com/John-Frye/evaluating_teen_pregnancy_policy_in_baltimore), my partner and I concluded that child poverty, domestic violence, and low access to prenatal care were heavily concentrated in Baltimorean population tracts with high teenage birth rates. We therefore devised a policy suggestion that advocated for the targeted funding of domestic violence shelters and prenatal care services in these tracts. However, data for child poverty, domestic violence, and low access to prenatal care needs to be collected and analyzed to determine their statistical significance in Charleston. Perhaps better access to prenatal and domestic violence care in Charleston accounts for why its teenage birth rate is lower than Baltimore's in similar income tracts. This could be an interesting research project, as it might actually demonstrate that Charleston has better access to prenatal care, despite my own pre-conceptions of its stigma against women's reproductive health. Until such data can be researched, though, we cannot conclusively say why Charleston's teenage birth rate is lower on average. 

### Analysis with Python
The use of plotly visuals did not necessarily change my interpretation of the data. However, I thought the visuals in plotly presented the association between income and teen birth rates much more clearly than the excel graphs. In Excel, I needed to create a graph with two y axes to visualize the data, as excel's pivot tables would not allow me to use household income as the x axis; I had to create a numbered list of population tracts by household income in order to create the visual. In plotly, I was able to create the visual I had always wanted to make in excel. Readers need only to look at one clear trendline to understand that, on average, higher household incomes are associated with lower teenage pregnancy rates. As we discussed in class, clear visualizations can communicate data more clearly to relevant decision makers. The plotly graphs might be more useful to bring to each city's government in order to convince policy-makers of the income-pregnancy association and inform their decisions to address it. 

## Error Analysis
The following issues could have impacted the data collection for this analysis:
- Many tracts in both Baltimore and Charleston lacked sufficient data on teenage birthrates, meaning that some tracts were not included in the dataset
- Charleston was subdivided into fewer population tracts than Baltimore, so there was less information on Charleston's teenage birthrates. This also made it difficult to graphically compare Baltimore and Charleston's datasets.
## Step-by-Step Instructions
Step-by-step instructions for how I manipulated the excel data [can be accessed here.](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Instructions_Baltimore_Charleston_Teen_Pregnancy_Rate_Comparison.xlsx) 

Step-by-step instructions for my Python analysis [can be accessed here.](https://colab.research.google.com/drive/1nwqTRTdjc9mr1Ek-vtUdSv8DJLHZzsvV#scrollTo=cHaCMo0viK69)

