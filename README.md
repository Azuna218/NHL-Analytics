Project Overview
This project analyzes NHL player data and trends in births in Canada from 1991 to 2022. It combines data on player birthplaces, team rosters, and team success, while also applying predictive models and clustering techniques for exploratory analysis. Additionally, a Shiny app provides an interactive platform to visualize and predict player classes based on their physical attributes (height and weight) and birth country.

Project Structure
Data Files:

nhl_teams.csv: Contains information about NHL teams.
nhl_rosters.csv: Contains the rosters of players for each NHL team.
nhl_player_births.csv: Contains data on the birthplaces of NHL players.
canada_births_1991_2022.csv: Contains the number of births in Canada for each year between 1991 and 2022.

R Script:

The script loads the data, performs analysis using ggplot2 and dplyr, and deploys a Shiny app to visualize NHL player analysis.
Key Features

Trends in Canadian Births (1991-2022):
Aggregates and plots the yearly total births in Canada.
Visualization: A line chart showing the trend of births from 1991 to 2022.

NHL Player Birthplace Analysis:
Analyzes the number of NHL players based on their birth province in Canada.
Visualization: A bar chart showing the top provinces producing NHL players.

NHL Teams and Birthplaces:

Merges player and team data to analyze player birth countries across NHL teams.
Visualization: A bar chart showing the distribution of players' birth countries for different NHL teams.
Shiny Application:

Interactive platform for analyzing player height, weight, and birth country.
Predicts player class (e.g., Forward, Defense/Goalie) based on user input.
User Input:
Select birth country
Choose height and weight ranges
Predict player class
K-Means Clustering:

Applies K-means clustering to group players based on height and weight.
Visualization: Scatter plot of clusters, with players grouped into two clusters (e.g., height vs. weight).

Silhouette Plot:
Evaluates the quality of clustering using silhouette width.
Visualization: Silhouette plot showing cluster separation.

How to Run
Install Required Packages: Ensure the following R packages are installed:

ggplot2
dplyr
shiny
cluster
You can install these packages using:


install.packages(c('ggplot2', 'dplyr', 'shiny', 'cluster')
Deploy Shiny Application: Set up your RSConnect account to deploy the Shiny app:

Run the Shiny App Locally: To run the Shiny app locally, use the following:
shinyApp(ui = ui, server = server)

Execute the Analysis: Run the script to visualize the trends, player birthplace distribution, and team analysis:
source("NHL_Player_Analysis.R")

Outputs
Plots:
Trend of Canadian births (1991-2022).
NHL player birthplaces by Canadian province.
Distribution of players' birth countries across NHL teams.
Clustering of players based on height and weight.
Silhouette plot for clustering.

Shiny Interactive Features:
Interactive plot of NHL player height vs. weight.
Player class prediction based on user inputs.
Future Improvements
Modeling: Refine the predictive model for player class prediction using additional features like age, position, or experience.
Clustering: Experiment with other clustering methods like DBSCAN to better capture player characteristics.
Visualizations: Enhance the Shiny app with additional visualizations for team performance and player statistics.

License
This project is released under the MIT License.

Author
Francesco Sebastian
