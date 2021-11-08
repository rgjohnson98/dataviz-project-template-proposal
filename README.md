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

## Project Progress Report and Revised To-Do List 


  * Make sure the track names are consistent across vizzes
  * Update README for each file
