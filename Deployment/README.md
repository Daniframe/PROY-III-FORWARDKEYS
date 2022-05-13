# Deployment
Little app built in R using shiny and flexdashboard, where the company can exploit our model based on association rules.

We tried to find the attributes of the passengers that most influence a full cancellation due to a major disaster on the destination, however, it is generalized for any type of bookingsign (partial_cancellation, partial_addition and new_booking).

It is also ready to be used by **FordwardKeys**, to easily explore more events like this attack on Paris.

 ### How to navigate the app
 <ol>
<li>Select the datasets (csv, ; separated) to examine, bottom-left for the data of the event, bottom-right for the data to compare with. Note: Datasets need to share the same timeframe (same month) </li>
<li>Data will start to load (watch the progress bar update).</li>
<li>On the DASHBOARD page, select the bookingsign to analyse and click compute rules (we can change it as many times as we want).
     The rules (attributes) will be plotted on the first chart by their score (influence on the event year).</li>
<li>Choose the combination of attributes to plot and press update, the second page of plots will show the relative frequency of the bookingsign selected for the datasets with and without the conditions, to easily compare them. As of right now it is not robust to errors, so if a combination of attributes does not exist in the data, the app will stop working.</li>
<li>A variety of metrics and information about the attack will be shown on the last tab. </li>
</ol>

### Libraries needed

arules, dplyr, ggplot2, tidyverse, reshape2, flexdashboard, shiny, shinyWidgets

## Data-ready deployment

As a way to easily show the dashboard. This app does not need to load any data from the client. It needs to have the datasets Nov2015 and Nov2014 installed though.
The easiest way to access the app is through shinyapps where it is uploaded.\
### shinyapps link
* Data-ready application: https://carlo0os.shinyapps.io/deployment_data-ready/
* Original Deployment: https://carlo0os.shinyapps.io/deployment_forwardkeys/
