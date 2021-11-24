# Data Visualization Project Proposal (Final Version)

## Data
The data I propose to visualize for my project is a dataset containing information on every NASCAR race run from 1975 to 2003. I have been a fan of the sport for over 10 years and so I would really like to work with this data as I can provide some insight via domain knowledge that I have. This dataset contains 10 variables including the driver's name, starting and finishing positions, their payout, car make, etc. I will also be drawing from an accompanying dataset that contains information on each track (such as length and track type, etc.) that joins this dataset via a composite key. This would allow for further visualizations and interactivity. This is the same dataset I proposed in my [rough draft](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Proposal_RoughDraft.md). [Here](https://gist.github.com/rgjohnson98/1adb1e0d401abab38e1d294ac70f547e) is a link a gist containing the driver dataset.

## Progress And Prototypes
Thus far, I five prototype visualizations in various states of completion. Just as a note, these did require some data preprocessing in R before the data was ready to use in Vizhub. They are as follows:

The first [prototype](https://vizhub.com/rgjohnson98/a646a003d3934b20b50c3576d380f507) I have is this one. This is a bar chart showing the number of starts it took each winner in the dataset to win their first race. Fans might be interested in this as we can see just how few different winners there were during this stretch (only 61 out of 683 total drivers), and about how long it takes a driver, who does win, to win their first race. For the question I am trying to answer, this is nearly complete. Note the highlighted bar and box showcasing my proposed interaction.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Starts%20Viz%20WIP.PNG)

My second [prototype](https://vizhub.com/rgjohnson98/ef337442a8c14016a30ec41408d8f8d7) is below. This interactive bar chart allows for the user to choose from several different performance related metrics in the sport. The graph will update and display the top 10 drivers for the selected category. In terms of answering the question, this one will, upon completion, do that. This visualization is the most incomplete of the five I have been working on. 
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Stats%20Viz%20WIP.PNG)

My third [prototype](https://vizhub.com/rgjohnson98/077df419172944cea5e5e5c9559a2938) is here. For this, I created an interactive scatterplot. This plot shows the year on the x-axis, and the starting position of the race winner on the y-axis. Hovering over a dot (as shown in the following screenshot), will show the winner and the track that the race took place at.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Start%20Pos%20WIP.PNG)

My fourth [prototype](https://vizhub.com/rgjohnson98/a4e8883a6b62466aa6ebe21b90d89b42) is also an interactive scatterplot. This one showcases the different auto makers that were used, and how they compared to each other in terms of finishing position. The dots are sized by the number of finishes at that position. I still need to do some tweaking to make this plot more readable, but the general idea is here. Hovering over a dot will show the position and the frequency of that position, as demonstrated with the box in the bottom right corner. 
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Make%20Viz.PNG)

My fifth and final [prototype](https://vizhub.com/rgjohnson98/83f502237c234b50b205b7f9aea671a5) is an interactive map. This map shows the locations of the different tracks that NASCAR runs on by their geographical coordinates. The dots are colored by the type of track, and this plot is made interactive by hover capability. Hovering over a track will provide some details about it, such as it's type, length, status (some tracks closed between 1975 and 2003), and the last winner there.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Track%20Map%20Viz%20WIP.PNG)

## Questions & Tasks
The following tasks and questions represent my revised goals for this project.
  * How long does it typically take for drivers to win their first race? (My first visualization)
  * Who had the most starts (and other metrics such as wins) during this time frame? (My second visualization)
  * At what starting position do winners tend to start from? (My third visualization)
  * Create a scatterplot for car maker finishes so that the size of the dots increases based on the number of finishes at that position (My fourth visualization)
  * Where, geographically, are most tracks located? (My fifth visualization)
  * How has the winner's payout changed over time? (A potential sixth visualization, depending on how far I get)

## Summary of Interaction
Here is a summary of the interaction I have (or am planning on having) for each of my visualizations:
  * First Wins Bar Graph: Hovering over a bar will display the number of starts, the year, and the track. 
  * Top 10 Driver Bar Graph: The user will select a metric to view in the bar graph and it will update accordingly.
  * Starting Position Scatter Plot: The user can hover over dots and see which driver won and at what track.
  * Car Maker Scatter Plot: The user can hover over the dots to see the position and the frequency.
  * Track Map: User can hover over the dot and see details on the different tracks.

## Schedule of Deliverables 
Here is a schedule of deliverables:
  * Fix my preprocessed data
    * Split the driver's name into First Last, not FirstLast
    * Fix the data frame for my map so that it will display most wins at the track, not most recent winner
    * Projected completion date: 10/15
  * Starts before first win bar graph
    * Change the color
    * Fix with position and orientation of driver’s names
    * Add a title 
    * Projected completion date: 10/18
  * Driver metric bar graph
    * Fix the winning percentage metric. The x-axis is not displaying the data properly
    * Make sure the plot will display the requested metrics
    * Decide if other metrics should be included
    * Make sure the x-axis and scale are correct and update
    * Add a y-axis title and viz title
    * Play with the color
    * Projected completion date: 10/21
  * Starting position scatter plot
    * Make sure the names display properly
    * Change the color, the text size for the tooltip, and the opacity
    * Add the starting position to the tooltip, or change the axis scale
    * Projected completion date: 10/24
  * Car make scatter plot
    * Increase the size for the smallest dots so they are visible
    * Make the size of the bigger dots bigger (will make the contrast more obvious)
    * Play with color
    * Make sure the tooltip displays the proper data
    * Change variable name from "Freq" to "Frequency" so it will display properly
    * Projected completion date: 10/27
  * Track Map
    * Lighten the state outlines to be a lighter shade of grey or white
    * Recheck the track info to ensure there are no spelling errors and that it displays properly in the tooltip
    * Change the variable names in the gist and see if they can be left justified
    * Fix the title, and the title for the legend
    * Play with the colors
    * Change "recent winner" metric to "most wins" for the track
    * Projected completion date: 10/30
  * For all plots
    * Check the tooltip displays, especially the driver's names
    * Make sure the viz updates and displays properly
    * Update README
    * Projected completion date: 11/4

## Project Feedback Iteration
[Here](https://vizhub.com/rgjohnson98/19742d253430447fab8a8e43fb17c949) is my iteration of the "Winners by Starting Position" viz having incorporated the feedback given. This is exactly the direction I needed on this, and I think it looks so much better and more informative this way. I colored the points on the plot by the track name, and sized them by the track length. This provides the viewer with an opportunity to look for patterns, particularly among tracks and track types. For example, one may notice that the larger dots (such as the 2.66 mile Talladega Superspeedway) produce a lot more winners from further back in the field than short tracks like the .526 mile long Martinsville Speedway where passing is harder. 
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Starts%20Viz%20Iteration.PNG)

## Project Progress Report, November 8, 2021
Here is my project update as of November 8, 2021. I have five visualizations and they are essentially complete, minus updating the README files and potentially some cosmetic changes. Then, I will need to attach them to a dashboard and add a cross-filter so that they will all work together. The biggest tasks I have compelted since the last update are to update the data, work on the statistics plot with the dropdown menu (more on this below), and to ensure that there is a uniform color scheme between vizzes so that each track has it's own unique color. So, here are my updated plots:

[Here](https://vizhub.com/rgjohnson98/def19c52ecc94ae1aa78dad8a083d647) is my dashbord "skeleton" thus far. I have had some trouble constructing it and am continuing to work on it. Once it is ready, I will attach the plots to their designated spaces, and add a cross-filter so that the user can select a track, and all the plots will update accordingly to focus only on those stats. Please see the end of this section for an image of what I would like everything to look like when it is done, but note that it is just an image and not functional in any way.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg1.PNG)


My first [viz](https://vizhub.com/rgjohnson98/5e91de25a2744f658c6a2c947c361e1d) is below. I have included two images to demonstade the dropdown and hover capability. This viz is essentially complete. I added the stats dropdown, hover capability for the tracks, and a tooltip to display the driver's name and the track type. Very little remains to be done on this one. I need to add a title, move up the legend if that's possible, and update the README.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCARScattera.PNG)
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCARScatterb.PNG)


My second [viz](https://vizhub.com/rgjohnson98/83f502237c234b50b205b7f9aea671a5) is the track map. Once again, each track has it's own color and the tooltip displays data on the track such as the length, the type, and, now, who has the most wins there (plus the count). This viz is basically done, except for updating the README.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg3.PNG)


Next up is my [viz](https://vizhub.com/rgjohnson98/220e9635e3a246ce869f252569ff8b6e) of the race finishes by automaker. The first image below is the full viz, with no filter. The second image I have attached below shows my filter active, and set to Daytona International Speedway, home of the sport's most famous race. The filter I have now has to be set manually in the code, but this is something that will be changed once I have a cross-filter worked out. I will also try to make the dots the color of the track when the filter is activated, but I am not sure how to do that.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg4.PNG)
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg4%20(Filter%20Active).PNG)


Next is my [chart](https://vizhub.com/rgjohnson98/cbc26d9eb24f41548b2d048ead4915d2) displays the drivers with the top 10 most wins during this period, split by track. In order to display just the top 10, I added a variable to the dataset called "IsInTop10" to rows for those drivers. I also added a tooltip to display the track name, and the number of wins there. This viz is done for now. My intention is for the tracks other than the one selected to be greyed out during cross-filtering.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg5.PNG)


My final [viz](https://vizhub.com/rgjohnson98/85f04416bed44645963d1b47ec5bfde0) is the chart showing the number of starts it took for each winner to win their first race. The only modification I made recently is to change the track colors to match the other plots. This viz is done, except for what will need to be done for the cross-filter. Again, I'd like the bars other than the ones for the track selected to be greyed out.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjProg6.PNG)


I also created an image of what I would like the final product to look like, and have included it here. My goal is for the dashboard to look similar to this and for all of the visualizations to interact with each other, as described above. I made this in MS Word, and it is just a rough outline of what I would like to achieve as the final product. I would really like to thank our classmate Raul for pointing me in this direction. Before his suggestions, I did not have a clear idea for a final product. I had just planned on having five or six different visualizations that were not really connected. Now, I have ideas and a plan for getting them done. I really think an interactive dashboard will tie everything together.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_573_FinalProjGoal.PNG)


## Project Progress Report, November 17, 2021
With practically all of the work on the individual plots done, I took some time this week to work on my dashboard ideas, and constructed a seperate legend for it. The goal here is that, eventually, the user can select a track from the legend, and all five of the plots will update according to their selection. Creating the legend was relatively easy, but, to be honest, I struggled with the dashboard and made little headway all week. After meeting with Dr. Kelleher, though, we created a simple template to work from, and I feel slightly better about completing what I need to do now. I will likely need more help as we go on, but, for now, here is my progress:   

[Here](https://vizhub.com/rgjohnson98/9f61ebafa7f640058d74d70f7121c450) is my legend for the dashboard. This was relatively straightforward, and the only real challenge it presented was making sure the colors were in the correct order.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_Legend.PNG)


Secondly, [here](https://vizhub.com/rgjohnson98/bad8c60855a849d690c259453ea5bec0?edit=files) is what I have of the dashboard so far. The code from each plot has been added to its respective files in here, but it has not been properly integrated yet, and nothing is functional yet. This is going to be my big project for the coming week, and I anticipate I will need some more help to get everything how I would like it.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/CS_Dash.PNG)


What is left to do now:
  * Dashboard: Add all plots to the same sheet, add a header.
  * Cross-Filter: Add a cross-filter to the dashboard so that clicking a track in the legend will update all. How to implament it?
  * Cosmetic changes to vizzes: Add a fade effect to the vizzes for when the filter is active


## Project Progress Report, November 24, 2021
After getting the feedback last week, I spent this week working on the dashbord and going through different renditions of it. I had to change up what I was planning on doing slightly for several reasons. First, I have had to reduce the number of visualizations on the dahsboard from five to four, for space reasons. With three on a single row, it became too crowded and the details far too small. I also decided not to display the legend I was planning on doing for similar reasons. To fit it in would require me to make the text so small it was tough to read. This is one place I would like to get some feedback on. However, one thing here is that each track has a unique color that spans across all of the visualizations, so that helps to act as legend, escpecially when combined with the map plot. So, below are my four dashboard attempts, in the order they were created. I started off rather simply, and then tried some different things to see what worked and what did not.

## Dashboard 1
My first dashboard is pretty simple. It displays four plots and continues to utilize the same tooltips I used before. There are no filters here, just a very basic plot.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%201.png)

## Dashboard 2
My second dashboard is very similar to the first. The only difference here is that I switched out the "top 10 winners" plot in favor of the "starting positions of winners" plot.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%202.png)

## Dashboard 3
For my third dashboard, I added a filter (active in the second image below). It is pretty simple and, when activated, fades the dots not pertaining to the selected track. Sadly I am yet to figure out how to make it so there is only one dropdown for the entire dahsboard that adjustes every plot at once. What I have right now is a dropdown for each plot, so I suppose that is useful if you want to display different information at once. Each visualization resets with a click to the plot. I am very happy with how it has turned out.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%203a.png)
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%203b.png)

## Dashboard 4
For my final dashboard, I swapped out the "car maker" plot for my "top 10 wins" plot. Other than that, everything is the same. The dropdown works exactly the same for each plot, and they all update accordingly.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%204a.png)
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Dashboard%204b.png)

What is left to do now:
  * Potentially tie everything to a single dropdown
  * Reset the plots with the selection of "all tracks"
  * Work on some cosmetic changes based on feedback
  * Decide which four to display
