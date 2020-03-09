# Google Ads display campaign budget checker
Google Ads script to check budgets and pause campaigns (it works for display campaigns)

The goal of this Google Ads script is to pause the display campaign or send a notification if the daily campaign spend is significantly higher. It is useful when you run a campaign until a specific date.

In the spreadsheet, you just fill a column with the right information and the algorithm will work to check campaigns spend vs. target spend.

It calculates how much you can spend daily to the end of the campaign. Then it checks yesterday's spend and today's spend. If yesterday/today spend is higher than can be it will do the action (pause/notification). It calculates with column Pause Ratio and Notification ratio. It will multiply yesterday/today target spend with Ratios and if spend is higher than target spend it will do the action.

It is easy to implement. 

1) Put the script on your MCC account and enable an hourly run.
2) Create a copy of the spreadsheet and insert URL to script: https://docs.google.com/spreadsheets/d/1eFJHA8i9OC0oemhyy4NakTHlD8MK-p2McaZb0n8rOJw/edit?usp=sharing
3) you can just fill the columns in the spreadsheet (you can copy already formatted column in range G2:M2 to your row and set your own conditions)
4) set written labels in the spreadsheet on those campaigns
5) There are two columns with Status
      a) Today STATUS - if its enabled (TRUE) it'll send notifications or pause campaign because of today overspending.
      b) Yesterday STATUS - if its enabled (TRUE) it'll send notifications or pause campaign because of yesterday                                         overspending. So if script spamming you, you can set column to FALSE and notification from                                     yesterday overspending will stop.

Column Client + campaign will be the email title. For every campaign, you will get separated messages in your mailbox. 
