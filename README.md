# Data Visualization Project

## Data

The data I propose to visualize for my project is a datset containing information on every NASCAR race run from 1975 to 2003. I have been a fan of the sport for over 10 years and so I would really like to work with this data as I can provide some insight via domain knowledge that I have. This dataset contains 10 variables including the driver's name, starting and finishing positions, their payout, car make, etc. There is an accompanying dataset that contains information on each track (such as length and track type) that joins this dataset via a composite key, and would allow for further visualizations and interactivity. 
Here is a link to the driver dataset: https://gist.github.com/rgjohnson98/1adb1e0d401abab38e1d294ac70f547e

## Prototypes

Thus far, I have two prototype visualizations. The first is this scatterplot showing the finishing positions of each car make throughout the 28 years shown in this dataset. As we can see, neither Plymouth nor Chrysler won any races during that time, but all others have won at least once.

[![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/2f0df7ce5a50ea1d0fc450a7a7a95675cf0cc549/NASCAR%20Make%20Scatterplot.PNG)](https://vizhub.com/rgjohnson98/7bfbdfe47ee34b5d811ede4ea41232a4)

The second prototype I have is this one. This is a bar chart showing the number of starts it took each winner in the dataset to win their first race. Fans might be interested in this as we can see just how few different winners there were during this stretch (only 61 out of 683 total drivers), and about how long it takes a driver, who does win, to win their first race. This did require some data preprocessing in R before the data was ready to use in Vizhub.

[![image](https://github.com/rgjohnson98/dataviz-project-template-proposal/blob/2f0df7ce5a50ea1d0fc450a7a7a95675cf0cc549/NASCAR%20Starts%20Bar.PNG)](https://vizhub.com/rgjohnson98/8f4ebea5b2a74516a648fb5764fd233e)


## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:
  * How has driver's payout changed over time? (Further, how has the winner's payout changed over time?)
  * Use a node-link tree diagram for the different tracks and determine which driver has the most wins there (make it interactive by seeing a full breakdown of the winners there or allow the user to filter by track type)
  * Update my driver's first win bar graph and make it interactive so we can see which track their first win came at
  * Who had the most starts during this time frame?
  * Where, geographically, are most tracks located? (Interactive to zoom in on regions)
  * Update my scatterplot for car maker finishes so that the size of the dots increases based on the number of finishes at that position
  * Is there a correlation between starting and finishing positions?
  * At what starting position do winners tend to start from?
  * Can we track cumulative wins to see who won the most during this time frame?

## Sketches

(insert one or more hand-drawn sketches of interactive visualizations that you imagine)
(describe each sketch - how is the data visualized, what are the interactions, and how do these relate to the questions/tasks)

## Open Questions

(describe any fear, uncertainty, or doubt you’re having about the feasibility of implementing the sketched system. For example, “I’m not sure where to get the geographic shapes to build a map from this data” or “I don’t know how to resolve the codes to meaningful names” … Feel free to delete this section if you’re confident.)
