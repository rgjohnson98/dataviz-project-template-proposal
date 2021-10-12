# Data Visualization Project Proposal (Final Version)

## Data
The data I propose to visualize for my project is a datset containing information on every NASCAR race run from 1975 to 2003. I have been a fan of the sport for over 10 years and so I would really like to work with this data as I can provide some insight via domain knowledge that I have. This dataset contains 10 variables including the driver's name, starting and finishing positions, their payout, car make, etc. I will also be drawing from an accompanying dataset that contains information on each track (such as length and track type, etc.) that joins this dataset via a composite key. This would allow for further visualizations and interactivity. This is the same dataset I proposed in my [rough draft](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/Proposal_RoughDraft.md). [Here](https://gist.github.com/rgjohnson98/1adb1e0d401abab38e1d294ac70f547e) is a link a gist containing the driver dataset.

## Progress And Prototypes
Thus far, I five prototype visualizations in various states of completion. Just as a note, these did require some data preprocessing in R before the data was ready to use in Vizhub. They are as follows:

The first [prototype](https://vizhub.com/rgjohnson98/a646a003d3934b20b50c3576d380f507) I have is this one. This is a bar chart showing the number of starts it took each winner in the dataset to win their first race. Fans might be interested in this as we can see just how few different winners there were during this stretch (only 61 out of 683 total drivers), and about how long it takes a driver, who does win, to win their first race. For the question I am trying to answer, this is nearly complete. Note the highlighted bar and box showcasing my proposed interaction.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Starts%20Viz%20WIP.PNG)

My second [prototype](https://vizhub.com/rgjohnson98/ef337442a8c14016a30ec41408d8f8d7) is below. This interative bar chart allows for the user to choose from several different performance related metrics in the sport. The graph will update and display the top 10 drivers for the selected category. In terms of answering the question, this one will, upon completion, do that. This visualization is the most incomplete of the five I have been working on. 
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Stats%20Viz%20WIP.PNG)

My third [prototype](https://vizhub.com/rgjohnson98/077df419172944cea5e5e5c9559a2938) is here. For this, I created an interactive scatterplot. This plot shows the year on the x-axis, and the starting position of the race winner on the y-axis. Hovering over a dot (as shown in the following screenshot), will show the winner and the track that the race took place at.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Start%20Pos%20WIP.PNG)

My fourth [prototype](https://vizhub.com/rgjohnson98/a4e8883a6b62466aa6ebe21b90d89b42) is also an interactive scatterplot. This one showcases the different auto makers that were used, and how they compared to each other in terms of finishing position. The dots are sized by the number of finishes at that position. I still need to do some tweaking to make this plot more readable, but the general idea is here. Hovering over a dot will show the position and the frequency of that position, as demonstrated with the box in the bottom right corner. 
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Make%20Viz.PNG)

My fifth and final [prototype](https://vizhub.com/rgjohnson98/83f502237c234b50b205b7f9aea671a5) is an interactive map. This map shows the locations of the different tracks that NASCAR runs on by their geographical coordinates. The dots are colored by the type of track, and this plot is made interactive by hover capability. Hovering over a track will provide some details about it, such as it's type, length, status (some trackes closed between 1975 and 2003), and the last winner there.
![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/master/NASCAR%20Track%20Map%20Viz%20WIP.PNG)


## Questions & Tasks

The following tasks and questions represent my revised goals for this project.
  * How long does it typically take for drivers to win their first race? (My first visualization)
  * Who had the most starts (and other metrics such as wins) during this time frame? (My second visualization)
  * At what starting position do winners tend to start from? (My third visualization)
  * Create a scatterplot for car maker finishes so that the size of the dots increases based on the number of finishes at that position (My fourth visualization)
  * Where, geographically, are most tracks located? (My fifth visualization)
  * How has the winner's payout changed over time? (A potential sixth visualization, depending on how far I get)


Data processing is done.
TODO: Readme
Section for interatiocn, section for deliverables (what remains to be done)
