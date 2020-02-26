# budget-checker
Google Ads script to check budgets and pause campaigns

Goal of this Google Ads script is to pause display campaign or send notification if campaigns spend more than can daily to the end of campaign.

In spreadsheet you just fill column with right informations and algorith will work to check campaigns spend vs. target spend.

It calculate how much you can spend daily to the end of campaign. Then it check yesterday spend and today spend. If yesterday spend is higher than can be it will do action (pause/notification). It calculate with column Pause Ratio and Notification ratio. It will multiply yesterday/today spend with Ratios and if its higher than target daily spend it will do action.

It is easy to implement. You just put the script on your MCC account and enable hourly run.

After that you can just fill the columns in spreadsheet and set label on that campaign.

Columnt Client + campaign will be email title, so for every campaign you will have separated messages in your mailbox

You can disable action of script by setting column ENABLED in that row to FALSE
