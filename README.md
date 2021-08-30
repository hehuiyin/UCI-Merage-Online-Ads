# UCI-Merage-Online-Ads

## Background

Established in 1965, UCI’s Paul Merage School of Business offers a wide range of academic degrees from undergraduate, graduate, to doctorate. While the school offers programs for varying tiers of education, this project will focus on the following Master’s programs: Fully Employed MBA (FEMBA) and Full Time MBA (FTMBA). Considering its respectable ranking, Merage can still find ways to improve its online presence and outreach to prospective students.

## Dataset

Our datasets observe social platform performance and lead source information from 2016 to 2020. The social platform dataset overviews the metrics of advertising campaigns from LinkedIn, Google, and Facebook, whereas the lead source dataset records the time of the initial inquiry of prospective students, application status, last time modified, and the source the lead is from.

## Goal

Our objectives for this project are to answer the below two questions:

  * Which online advertising mechanism has a higher quality lead?
  * How to better allocate spend on each online advertising social platform?

## Exploratory Data Analysis

<img width="197" alt="Screen Shot 2021-08-30 at 14 21 36" src="https://user-images.githubusercontent.com/73683982/131407270-88b03adc-6945-4747-baeb-58f2ad73cbeb.png">

From the above graph, the lead source data consists of information of where a prospective student is in the marketing funnel, along with the last time modified and the source the lead is from. The time range for this dataset is the end of 2018 to the beginning of 2020.

<img width="553" alt="Screen Shot 2021-08-30 at 14 20 11" src="https://user-images.githubusercontent.com/73683982/131407117-fd309666-1643-4d72-868a-7ff2d90fc121.png">

From the Sankey diagram above, we can see that a majority of the applicants do not apply but instead submit an inquiry to learn more about the programs offered.

From our dataset, out of the 6,285 people, 81% inquired but less than 20% actually apply. Among those who applied, 35% of the applications are archived meaning the application process is complete. Of those who submitted an application, half of them were denied, 20% declined the school’s offer, while 30% enrolled into the program. We also observed that only 2% of those who inquired will also enroll into the program.

<img width="669" alt="Screen Shot 2021-08-30 at 14 24 30" src="https://user-images.githubusercontent.com/73683982/131407601-4e2a7509-a30c-4303-8c75-d2582fe85a6a.png">

We observed the duration of time applicants took to apply. The bar chart shows the number of days it took to apply versus the frequency of applicants. Because most of the data points fall between Day 100 and Day 400, we focused on that specific time range. Our dataset contains a significant amount of NA values but the number of NA values drop significantly after Day 175. We assume that this is because applicants will consider whether to apply for five months before they drop it completely.

<img width="664" alt="Screen Shot 2021-08-30 at 14 25 44" src="https://user-images.githubusercontent.com/73683982/131407759-0a68aae3-9199-4ef3-87ea-d7e8abc15a5e.png">

The bar chart portrays when students first fill out an inquiry form. We can see that there is an increase of people seeking information on the Merage website from September to January. From a marketing standpoint, we can conclude that the best time for Merage to launch their marketing campaign is during September to January where there is a five month window to persuade a prospect to apply.

## Social Platform Analytics

### Cross-Platform Analytics

<img width="599" alt="Screen Shot 2021-08-30 at 14 31 17" src="https://user-images.githubusercontent.com/73683982/131408435-4983270e-8eda-4764-ab4d-42b2e66affc4.png">

Merage spent most of their advertising budget on LinkedIn and Google Ads. From these campaigns, Google Search Ads and LinkedIn Sponsored InMail generated the most advertising spend. According to Merage's marketing team, we were informed that more money is spent towards LinkedIn for advertising MBA programs because of the higher quality conversion rate, meaning that more candidates are admitted from LinkedIn.

<img width="616" alt="Screen Shot 2021-08-30 at 14 32 08" src="https://user-images.githubusercontent.com/73683982/131408540-93c72e5f-7329-40e8-bf2b-2e4a92212764.png">

The click-through-rate (CTR) measures the percentage of people who view and click on Merage’s ads. Using the CTR to evaluate the social platform’s performance, we found that LinkedIn has an extremely high CTR of 65% thanks to LinkedIn Sponsored InMail.

However, after researching the actual metric definition of InMail, the CTR is actually calculated as the number of messages opened by a user divided by the total number of InMail sent. Users are naturally curious about what is being sent to their inbox therefore they are more inclined to open the message. Users must click on the InMail to view the actual content of the advertisement. Because InMail measures its CTR based on if a user clicks on the message but not if they click on the link within, we proceeded to calculate the rate of call to action instead.

<img width="668" alt="Screen Shot 2021-08-30 at 14 34 18" src="https://user-images.githubusercontent.com/73683982/131408762-d541ec0a-77bc-4d84-850b-5f3ab6bc4049.png">

After updating our formulation to calculate CTA, this is a better measure to test the effectiveness of LinkedIn’s campaigns. The CTR of InMail drops from 65% to 3% yet, LinkedIn still remains the highest among all campaign types across the platform.

### Facebook & Instagram

<img width="362" alt="Screen Shot 2021-08-30 at 14 37 41" src="https://user-images.githubusercontent.com/73683982/131409088-418e44b6-c608-4a3b-910a-da8fb0061d51.png">

The sponsored post on Facebook for FEMBA (orange dot) did not generate a high CTR despite its high cost to run the marketing campaign. After noticing Facebook’s ineffective advertisements, Merage can consider changing either the message, visuals, or placement of the advertisement in order to improve its conversions. 

Whereas for the Lead Gen for FTMBA campaign (pink dot), the campaign produced a high CTR at a low cost. Because of the high conversions of the FTMBA’s advertisements, Merage can consider allocating the budget more towards this campaign.

### Google Ads

<img width="516" alt="Screen Shot 2021-08-30 at 14 39 49" src="https://user-images.githubusercontent.com/73683982/131409284-d031bcd5-cce1-4739-8620-6bfbbbb91252.png">

The tree map above shows the various sizes of the total cost and CTR for each campaign displayed on the Google platform. The colors represent the CTR and the size of the box represent the total cost. From the visualization, the search ads for FEMBA have the highest spending and a significantly high CTR. Additionally, the search ads for FTMBA also generated a high CTR with relatively low costs. From this observation, we suggest that Merage may want to shift their focus from display ads to Google search ads instead.

### LinkedIn

<img width="520" alt="Screen Shot 2021-08-30 at 14 41 04" src="https://user-images.githubusercontent.com/73683982/131409401-94913791-4954-44bf-8d7e-182bd2355ab4.png">

This tree map depicts the total spending of each campaign and its respective CTR. There is a disconnect between the size and the color, meaning that the marketing team is not distributing most of the budget to the best performing campaigns. For example, FEMBA Inmail LA & OC October and November campaigns have high CTR but not much spending compared to the campaigns in January and June.

We noticed that October and November are the most popular times to apply for the MBA program. January is the standard MBA deadline for the second round of application submissions along with the last deadline being in June, which explains the low CTR for those two months. Comparatively, October and November are the most efficient time to attract students. Therefore, the team may consider putting more of the budget on the October and November campaigns.

## Google Keyword Analysis

The dataset also includes the Google search terms and keywords that Merage specifically chose for their Google search ad campaign. The following analysis evaluates keywords and search terms that either benefit or harm the school's attraction.

In order to examine the correlation between interaction rate and keywords, we ran a regression model to understand this relationship. Our dependent variable, interaction rate, measures the rate of prospects that clicked on the Google search link. After converting the 31 keywords into dummy variables, we decided to use a regularization method because of the 1,400 observations in order to avoid overfitting.
  + **Ridge Regression**
  + **Lasso Regression**
  + **Elastic Net Regularization**

<img width="261" alt="Screen Shot 2021-08-30 at 14 49 36" src="https://user-images.githubusercontent.com/73683982/131410329-2f28ca71-be95-4c2a-b970-89f17c51b324.png">

Comparing the results from three models, we concluded that the Elastic Net model has the best performance.

## Recommendation

1. According to the lead source analysis and platform analysis, most prospects start inquiring about Merage’s MBA programs in September and January while October and November have a relatively high CTR, suggesting more prospects are engaging with the ads. Our suggestion is that September to January is the best timing for MBA advertising.

2. Another aspect of Merage’s campaign that the team can consider is allocating their budget from LinkedIn InMail to Google Ads. By understanding the definition of each metric on each platform, Merage can then efficiently strategize their marketing campaign. At times, the social platform analytics tend to boost its statistics of advertisements to appear successful but in reality, it does not reflect how well the ad is performing.

3. Along with that, Merage can regularly monitor search terms and remove some poor performing keywords. By selecting more direct competing schools as the keywords, like UCLA, UCI ads may attract more relevant students who are interested in MBA programs.

4. Lastly, Merage can also exclude negative search terms that UCI does not necessarily want to associate with. By removing harmful keywords like mentioned previously, marketing campaigns can allocate their money more effectively.


The complete analysis can be found on: https://hehuiyin.github.io/UCI-Merage-Online-Ads/
