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
Using the aforementioned metrics, I compared household income data in each of the cities' documented population tracts with the same tracts' teenage birth rate. For the teenage birth rate, I used the average rate for all income levels within a tract. For the income data, I used the average household income within a tract. To make this comparison, I filtered the data in both Charleston and Baltimore to include only datapoints for population tracts within each city proper. I then used VLOOKUP to create merged datasets for Baltimore and Charleston respectively. 

I undertook a similar analysis for Python. I filtered the datasets to include only tracts within each city, merged the datsets, and then created plotly visuals for each.

The following chart is an updated version of the chart in my original mini-project #1. The graph's x axis lists the population tracts in Charleston, SC from highest to lowest average household income. The red line models this arrangement of tracts by household income, while the green line graphs the population tracts' corresponding teenage birth rate. 

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/ExcelBaltimoreGraph.png)

This chart, also taken from my original mini-project, models the association between household income and teenage birth rates in Baltimore, MD:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/ExcelCharlestonGraph.png)

Both charts indicate that, on average, population tracts with lower household incomes have higher teenage birth rates. The fact that household income is calculated based on parental income also indicates that girls in poorer households are more likely to become pregnant. The data does not, however, provide conclusive insight into whether or not teenage pregnancies reduce a woman's income. 

Teenage pregnancy has a stronger negative correlation (-0.78) with household income in Charleston than in Baltimore (-0.66). This indicates that, as household incomes rise in Charleston, teenage pregnancy rates decrease to a greater extent than in Baltimore. This contradicts my findings from mini-project #2, as I will discuss in my Error Analysis section. 

My updated graphs for mini-project #4 exhibit similar trends in the data. The following graph, made in plotly express, illustrates teenage birth rates by the household incomes of each tract in Charleston, SC. 

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Proj%204%20Charleston%20Graph.png)

This plotly graph models the association between teenage birth rates and household income in Baltimore, MD:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Proj%204%20Baltimore%20Graph.png)

## Key Takeaways 
My data analysis indicates that population tracts with lower household incomes have higher teenage birth rates in both Baltimore and Charleston.  The tendency of lower income tracts to exhibit higher teenage pregnancies means that governments should target all programs aimed at teen pregnancy reduction (i.e. prenatal care access, aid to childhood poverty, domestic violence care, improved sexual health education, etc.) to lower income areas, particularly in Charleston.  

Baltimore's weaker correlation between income and teenage birth rates suggest that other factors, aside from income, strongly influence the metric. [In my midterm project](https://github.com/John-Frye/evaluating_teen_pregnancy_policy_in_baltimore), my partner and I concluded that child poverty, domestic violence, and low access to prenatal care were heavily concentrated in Baltimorean population tracts with high teenage birth rates. We therefore devised a policy suggestion that advocated for the targeted funding of domestic violence shelters and prenatal care services in these tracts. However, data for child poverty, domestic violence, and low access to prenatal care needs to be collected and analyzed to determine their statistical significance in Charleston. Perhaps Charleston's low income communities have even less access to prenatal and domestic violence care than communities in Baltimore, which could account for the former's strong negative correlation between income and teen pregnancy. If it is found that Charleston lacks such healthcare facilities, and that these facilities reduce teenage birth rates, then my hypothesis on Charleston's social stigma towards women's reproductive health could be supported. Until research on those metrics in Charleston is conducted, though, I am unable to draw any conclusions. 

Another key area of research I need to re-investigate is the correlation between race and teenage pregnancy in Baltimore and Charleston. If my previous analysis of the metric was flawed, as was the case of income in this mini-project, then I might come to different conclusions about the impact of racial disparities on teenage birth rates in both cities. Note that my conclusion in mini-project #2 was that household income had a stronger negative correlation in Baltimore and race a stronger positive correlation to teen pregnancy in Charleston. However, this project has demonstrated a stronger correlation between income and teenage pregnancy in Charleston. 

### Analysis with Python
The visuals in plotly presented the association between income and teen birth rates much more clearly than the excel graphs. In Excel, I needed to create a graph with two y axes to visualize the data, as excel's pivot tables would not allow me to use household income as the x axis; I had to create a numbered list of population tracts by household income in order to create the visual. In plotly, I was able to create the visual I had always wanted to make in excel. Readers need only to look at one clear trendline to understand that, on average, higher household incomes are associated with lower teenage pregnancy rates. As we discussed in class, clear visualizations can communicate data more clearly to relevant decision makers. The plotly graphs might be more useful to bring to each city's government in order to convince policy-makers of the income-pregnancy association and the corresponding necessity to target programs at lower income communities. 

Another benefit of my analysis with Python is that it eliminated the human error that contributed to mini-project #1's flawed results. While more time intensive, the merger process in Python does not require users to manually highlight table arrays from other datasets or select look up values, which introduce the possibility of error, as explained in my error analysis. 

## Error Analysis
The following minor issues could have impacted the data collection for this analysis:
- Many tracts in both Baltimore and Charleston lacked sufficient data on teenage birthrates, meaning that some tracts were not included in the dataset
- Charleston was subdivided into fewer population tracts than Baltimore, so there was less information on Charleston's teenage birthrates. This also made it difficult to graphically compare Baltimore and Charleston's datasets.

A major issue with my original mini-project occured during the data merger process on excel. I did not expand the width of the tract numbers' cells, which I used as the lookup value in VLOOKUP. This meant that many population tracts would simply be recounted as 4059100000 instead of 4095135278 during the merger, for example. When a population tract did not contain data on teenage pregnancies, I deleted it from the data analysis. Therefore, multiple population tracts were recorded as having no data on teenage pregnancies when I attempted to merge datasets. This eventually led me to discard many otherwise viable datapoints. When I created graphs or calculated correlations for the merged datasets, this lack of data understated the correlation between income and teenage pregnancy in Charleston. 

## Step-by-Step Instructions
Step-by-step instructions for how I manipulated the excel data [can be accessed here.](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Baltimore_Data_Analysis_Proj_4.xlsx) 

Step-by-step instructions for my Python analysis [can be accessed here.](https://colab.research.google.com/drive/1nwqTRTdjc9mr1Ek-vtUdSv8DJLHZzsvV#scrollTo=cHaCMo0viK69)

