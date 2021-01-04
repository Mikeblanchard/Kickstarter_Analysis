# **Kickstarter Challenge Analysis**

## This project was an extension of our analysis of Kickstarter campaigns for Louise, who is interested in Kickstaring a play.

#### Analysis and Challenges
The most difficult part of this analysis was choosing which data mattered. We had tons of data to refine, but decided to go in depth on comparing the success of Theater Play campaings to Launch Date and initial Goals. 

##### Launch Date Analysis
![](https://github.com/Mikeblanchard/Kickstarter_Analysis/blob/main/Theater_Outcomes_Vs_Launch.png)

From this chart, we can determine that the most successful month for successful campaigns is May, followed closely by the rest of the summer. By far the worst month for campaigns  is December, as is to be expected during the holiday season; people have other financial priorities during this time of year.

A point of notice is that the arc of successes and failures do both follow a same path throughout the year. Additional data would be needed to further determine successful campaigns. We would recommend a look at the type of plays being put on, perhaps categorized by genre, and a closer examination of the state or province in which these campaigns succeeded and failed. 

##### Initial Goal Analysis
![](https://github.com/Mikeblanchard/Kickstarter_Analysis/blob/main/Outcomes_Vs_Goals.png)

Our second area of interest was the success rate of campaigns at different starting Goals. We can see that low inital Goals of less that 5000$ do the best, with the most frequency. Its interesting to see how the two lines mirror each other, with serious dips in success occuring around the 25,000$ range, jumping up again breifly at 35,000$ then right back down again at 45,000$. It is important to note that there was only a combined total of 26 campaigns above 35,000$, of which only 8 were successful. We believe these to be outliers, and much more data at this starting Goal range is needed. 

On a technical note, we had some dicciculty with the COUNTIFS statements

      * * =COUNTIFS(Kickstarter!D:D, ">=1000", Kickstarter!F:F,  "successful", Kickstarter!$D:$D, "<5000", Kickstarter!R:R, "plays")* *
