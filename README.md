
#Kickstart Campaign Data Report
Syed Ahmed
February 28, 2021
 
##Overview 
	The purpose of this analysis was to help Louise figure out how different Kickstarter campaigns fared in relation to their launch dates and their funding goals. In this report, I will be analyzing the Kickstarter dataset using Excel to visualize campaign outcomes as they relate to their launch dates and funding goals. 

##Analysis and Challenges
###Theater Outcomes Based on Launch Date
	My first challenge was to create a Pivot Table that summarized the count of outcomes (failures, cancellations, and successes) by month for theater campaigns. This involved using the Kickstarter data in order to create a Pivot Table (see fig. 1) and filtering the table based on “parent category” (theater) and “years”, which was used to extract the monthly row labels. Once the data was correctly sorted and filtered, a line chart was created in order to visualize the relationship between theater outcomes based on launch dates. The most challenging part of this process was to setup the row labels in order to show months of the year, as there was no direct method of showing months of the year in the row labels section. To achieve this, I had to use “date created conversion” in the row field and group the rows in the Pivot Table to show months. Once this was sorted, I simply selected the data to create a Pivot Chart.  
Parent Category	theater			
Years	(All)			
				
Count of outcomes	Column Labels			
Row Labels	successful	failed	canceled	Grand Total
Jan			56	33	7		96
Feb			71	39	3		113
Mar			56	33	3		92
Apr			71	40	2		113
May			111	52	3		166
Jun			100	49	4		153
Jul			87	50	1		138
Aug			72	47	4		123
Sep			59	34	4		97
Oct			65	50			115	
Nov			54	31	3		88
Dec			37	35	3		75
Grand Total		839	493	37		1369


###Outcomes Based on Goals
	This part of the analysis involved using the COUNTIFS ( ) function in Excel to collect the outcomes and goal data for the “plays” subcategory from the Kickstarter worksheet, in order to visualize the percentage of successful, failed, and canceled plays based on the funding goal amount.  Using the COUNTIFS ( ) function correctly was the main challenge for this part of the analysis, as a simple mistake in the syntax can lead to inaccuracies in the results. One of the main challenges I faced was filtering the subcategory by “plays” in the function in order to get the correct values for campaign outcomes. I tried filtering the Kickstarter data, but that would not be the best approach for getting all three columns of outcomes. In the end, I figured out how to filter by “plays” in the function (see Fig. 2). Once this was sorted, I simply selected the appropriate data to create a line chart which visualizes outcomes based on goal. 
 
![countifs_](https://user-images.githubusercontent.com/45697471/109448255-876d8100-7a13-11eb-8bdc-7a0d3b87c1ba.jpg)


##Results 
###Theater Outcomes
	Analysis of the relationship between theater outcomes and the launch date of the campaigns between 2009 and 2017 shows that there are more successful campaigns than there are failed or cancelled ones across the year. If we look at Fig. 3, the line representing successful campaigns never touches or falls below the lines for failed or canceled campaigns. 


![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/45697471/109448267-8b010800-7a13-11eb-8664-6936f2558e5f.png)



Another conclusion we can draw from the data is that the number of successful campaigns is most likely to be at its peak between the months of May and June. If we look at the graph above, we can see that in these months the number of successful campaigns spikes up to between 100 and 111 campaigns. This means that these months are the best time to launch a campaign.
Goal Based Outcomes 

###Goal Based Outcomes 
	Analysis of the relationship between the percentage of successful, failed, and canceled campaigns and the campaign goal from $1 – $50,000+, we can see that the most successful campaigns for plays typically have a goal between $1 to $5,000. If we look at the graph in Fig. 4, we can see that at this range, the percentage of successful campaigns is between 73% to 76%, which is higher than any other goal range. We see an increase in successes between the $35,000 to $44,999 range at 67% as well, but after this the graph has a negative slope. 


![Outcomes_vs_Goals](https://user-images.githubusercontent.com/45697471/109448274-8dfbf880-7a13-11eb-8da8-e72f105b62b4.png)



##Limitations and Recommendations 
	One limitation of this dataset is that it does not include the most recent statistics for the 2018 to 2020. Being that the most recent data we have is up until 2017, we may not be able to draw the most accurate conclusions about Kickstarter campaigns today, especially given the current climate we live in with the global pandemic. The pandemic has changed our global economy tremendously, so having access to 2020 data could be useful to identify trends and forecast for the coming years. 
	Other graphs and tables such as box plots, column charts, and pie charts could be created to further examine the relationship between campaign goals and success rates, the relationship between campaign goals and amount pledged, and the percentage of successful campaigns by campaign type.  
