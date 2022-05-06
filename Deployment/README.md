# Deployment
Little app built in R using shiny and flexdashboard, where the company can exploit our model based on association rules. (unfinished)

We tried to find the attributes of the passengers that most influence a full cancellation due to a major disaster on the destination, however, it is generalized for any type of bookingsign (partial_cancellation, partial_addition and new_booking).

 ### How to navigate the app
 <ol>
<li>Select the datasets (csv, ; separated) to examine, bottom-left for the data of the event, bottom-right for the data to compare with. Note: Datasets need to share the same timeframe</li>

<li>Data will start to load (watch the progress bar update)</li>
<li>On the DASHBOARD page, select the bookingsign to analyse and click compute rules (we can change it as many times as we want)
     The rules (attributes) will be plotted on the first chart by their score (influence on the event year)</li>
<li>Choose the combination of attributes to plot and press update, the second page of plots will show the relative frequency of the bookingsign selected for the datasets with and without the conditions, to easily compare them</li>
</ol>
