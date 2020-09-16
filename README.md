# Comparing Teenage Birth Rates in Baltimore, MD and Charleston, SC Based on Average Household Income
## Background
The teenage birth rate is the fraction of women who gave birth to a child while they were between the ages of 13-19. Many social scientists view a high teenage birth rate as indicative of gender inequality, as teen pregnancies can [stifle women's educational and professional opportunities](https://www.mcser.org/journal/index.php/jesr/article/viewFile/542/567). The issue was especially prevalent in my culturally conservative hometown of Charleston, South Carolina. I wanted to see how Charleston's statistics on teenage birth rates compared to Baltimore with regard to other factors like household income. Prior to my data collection, I hypothesized that lower household income would be directly proportional to teenage birth rates and that Charleston would have a higher teenage birth rate in tracts with similar household incomes to Baltimore due to factors like cultural stigma against women's reproductive care.
## Question
Is lower household income positively correlated to teenage birth rates in both Baltimore, MD and Charleston, SC?
## Data Sources
I derived all of my data from Opportunity Atlas. The data is categorized as follows:
- [Average Household Income by Population Tract in Baltimore](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Baltimore_Income_Data.xlsx)
- [Average Household Income by Population Tract in Charleston](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Charleston_Income_Data.xlsx)
- [Teenage Birth Rates by Population Tract in Baltimore](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/baltimore_teen_pregnancy.xls)
- [Teenage Birth Rates by Population Tract in Charleston](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/charleston_teen_pregnancy.xltx)
## Data Analysis
Using the aforementioned metrics, I compared household income data in each of the cities' documented population tracts with the same tracts' teenage birth rate. For the teenage birth rate, I used the average rate for all income levels within a tract. For the income data, I used the average household income within a tract. 

The following chart models the relationship between household income and teenage birth rates in Charleston, SC:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Income_Birth_Correlation_Charleston.png)

This chart models the relationship between household income and teenage birth rates in Baltimore, MD:

![alt_text](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/eb208fa0d8972fdad16272bd8874958a39c09db4/Income_Birth_Correlation_Baltimore.png)

Both charts indicate that, on average, teenage birth rates are positively correlated to lower household incomes. The fact that household income is calculated based on parental income also indicates that girls in poorer households are more likely to become pregnant. The data does not, however, provide conclusive insight into whether or not teenage pregnancies reduce a woman's income. 

On average, Charleston had lower teenage birthrates and higher average household incomes than Baltimore. However, population tracts in Baltimore with a similar average household income to tracts in Charleston featured higher teenage birthrates. Baltimore's highest earning tract ($27,936) had a teenage birthrate of 45%, whereas Charleston's lowest earning tract ($27,207) had a teenage birthrate of 30%. 
## Key Takeaways 
My data analysis confirmed that teenage birth rates are positively correlated to lower household income. However, the data refuted my hypothesis that Charleston would have a higher teenage birth rate than Baltimore in tracts with equivalent incomes due to factors like stigma against women's reproductive care. While the data set is too limited to draw any conclusions about the latter, it leads me to believe that social stigma about women's reproductive care has less of an impact on teenage birthrates than I initially thought. 

Baltimore's higher-on-average teenage birthrates suggest that other factors might influence the metric. For example, racial disparities in healthcare access might inflate Baltimore's teenage birthrate. One should note that [Charleston's population is around 70% white](https://www.charleston-sc.gov/DocumentCenter/View/25665/FAST-FACTS-2020), while [Baltimore's is around 30% white](https://www.census.gov/quickfacts/fact/table/baltimorecitymarylandcounty/AGE295219). An additional analysis would need be done on tracts by race to determine if racial inequity is a contributing factor to teenage birthrate. 
## Error Analysis
The following issues could have impacted the data collection for this analysis:
- Many tracts in both Baltimore and Charleston lacked sufficient data on teenage birthrates, meaning that some tracts were not included in the dataset
- Charleston was subdivided into fewer population tracts than Baltimore, so there was less information on Charleston's teenage birthrates. This also made it difficult to graphically compare Baltimore and Charleston's datasets.
## Step-by-Step Instructions
Step-by-step instructions for how I manipulated the excel data [can be accessed here.](https://github.com/John-Frye/baltimore-charleston-comparing-teen-pregnancy-rates/blob/master/Instructions_Baltimore_Charleston_Teen_Pregnancy_Rate_Comparison.xlsx) 

