# Google Ads display campaign budget checker
Google Ads script to check budgets and pause campaigns (it works for display campaigns)

Goal of this Google Ads script is to pause display campaign or send notification if campaigns spend more than can daily to the end of campaign. It is useful when you have campaigns in specific date.

In spreadsheet you just fill column with right informations and algorith will work to check campaigns spend vs. target spend.

It calculate how much you can spend daily to the end of campaign. Then it check yesterday spend and today spend. If yesterday/today spend is higher than can be it will do action (pause/notification). It calculate with column Pause Ratio and Notification ratio. It will multiply yesterday/today spend with Ratios and if its higher than target daily spend it will do action.

It is easy to implement. 

1) Put the script on your MCC account and enable hourly run.
2) Create copy of spreadsheet and insert url to script: https://docs.google.com/spreadsheets/d/1eFJHA8i9OC0oemhyy4NakTHlD8MK-p2McaZb0n8rOJw/edit?usp=sharing 
3) you can just fill the columns in spreadsheet (you can copy right formatted column in range G2:M2 to your row and set your own conditions)
4) set label written in spreadsheet on that campaigns.
5) set column ENABLED on TRUE or you can disable action of script by setting column ENABLED in that row to FALSE

Columnt Client + campaign will be email title, so for every campaign you will have separated messages in your mailbox
