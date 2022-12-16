### Peer review team

- Peer review by: Group C
- Names of team members that participated in this review: Lena Binder, Julian Kulinsky, Sven Ritzmann

### Goal of the project

The goal of the project is to reduce the violence in Chicago by opening a new crime prevention center. An analysis of the data should help to find out which crimes occur particularly frequently and where they happen. This information will then be used to determine where the new Crime Prevention Center will be built.

### Data

The data contains information about crime incidents that happened in Chicago. For each incident data was collected about the date (year, month, day and hour), the place (latitude, longitude, block, beat, district, ward and community area), the IUCR code, if an arrest was made and if the incident was domestic-related. Numeric, ordinal and nominal data types are represented in the data set and these are in the formats category, date and float.

Further findings are the following: 

- In the data dictionary the same descriptions for latitude and longitude were used. This should be adjusted.
- Please differentiate the relevance of the columns `domestic` and `domestic_False`and `domestic_True`- they are all the same. The same applies to the columns `arrest`, `arrest_False` and `arrest_True`. Here, we suggest that one column with 0/1 values is enough to get the intention. Otherwise it is redundant.
- You used `.info()` to show data overview and first impressions (good).
- We also suggest using `.describe()` to show general statistics and detect first peculiarities such as outliers and other anomalies.
- Descriptive statistics for category variables are missing. This could also be relevant to gain more insights.
- Are there any columns that need to be dropped to make the analysis clearer? (In our opinion: yes, such as id and the domestic_False/True, arrest_False/True)

### Visualization approach

Create better graphs by adjusting the range of each data to avoid empty spaces which are not necessary (e.g. draft_arrest20221209-180000.html).
Furthermore, there is no description of the individual graphs that describes the exact 'findings'. So you see a graph but not the goal why the graph is crucial for the hypothesis. (See all graphs)
Align the title left to allow better reading flow (See all graphs)
The label descriptions should be worded better, instead of 'count' (e.g. draft_arrest20221209-180000.html) you can write 'count of committed crimes'.
In the map a weighted representation would be better since it lets recognize faster, where the criminal emphasis lies (draft_disctrict_map20221209-180000.html) . Also color combinations support the faster finding one's way in the visualization. Here a tooltip for altair would be interesting to show the exact values of the criminal activities.
The clarity is lost with single numbers above the bar charts if you look at "Count of committed crimes per type and domestic" (draft_domestic_crime20221209-180000.html). Here numbers disappear in the bar charts and therefore do not always appear which reduces the value of the chart.
With the bar chart "Count of committed crime per month" (draft_per_month20221209-180000.html) a line chart would be more meaningful around the Cluttering to avoid, thereby one could particularly emphasize the important values with colors. The same challenge arose with the "Count of committed crime per hour" (draft_per_hour20221209-180000.html) here one would also find oneself more easily with a line diagram. The individual bars irritate at first sight.
In general, it was difficult to deduce the meaning of the diagrams, since the representations such as the "Count of committed crime in the districts" (draft_per_district20221209-180000.html), for example, would have been better understood with a map representation.

### Lack of clarity

Further findings are the following: 

We recommend providing more insights into your analysis approach: What can you derive from your exploratory analysis? Which features are relevant? Which can be ignored? What does the first look on the statistics indicate? Are there anomalies?
We suggest summarizing the findings after each section (at least).
Hypotheses: Although it is not easy and straight-forward, try to formulate more possible hypotheses. The current hypothesis is limited and very general. Try to dive deep and imagine possible outcomes which could lead to a certain call-to-action.
Also the points commented regarding your visualization approach should be considered.

### Possible improvements

- Remove commented out code blocks that aren’t needed anymore. When looking at the code, it is irritating.
- There were problems to recreate the Visualizations with the Code (the html pictures helped to review the Visualizations). Try to create a better usability: use the comment ‘pip freeze > requirements.txt’  to save the environment packages with the needed versions. This can be installed by the reviewer with the comment ‘pip install -r "requirements.txt"’. It will help the reviewers to install the correct versions of the packages needed for the code review. 
- Also the points in the 'Visualization approach' are to be considered
- Also, your charts do not provide any sort of interactivity. Interactive elements bind the reader to your work and allow them to dive deep if they wish to do so. It definitely increases your flexibility and lets the people focus on your charts. 
- Try to expand your descriptive data analysis and your exploratory data analysis to gain more insights in advance. Hence, you will be able to focus on the most relevant aspects in your analysis.
- Even if no final conclusion or recommended actions can be made with the current status of the analysis, superficial conclusions regarding the individual wards or the time of the crimes could have been made. It could have been addressed in which wards the most crimes happened or at which time of day the most of them happened.

### Presentation

The data can provide valuable insights in various ways, however, we would suggest the following to include in your final presentation:
- Where do most crimes happen?
- Is there a correlation between seasons, such as winter/sommer? Thinking about it, we would assume there are more crimes in winter due to bad weather, coldness etc.
- Are most crimes falling under the domestic violence act? Why? Why not? What is the domestic violence act?
- Daytime of most crimes across blocks. Are there abnormalities across blocks? Are some blocks more likely for crimes during night?

### Organization

Remove commented out code blocks that aren’t needed anymore. When looking at the code, it is irritating.
It would be beneficial to number all visualizations sequentially, as it will provide a better orientation to the visualizations.

### Further comments

- You concentrated yourself on the most relevant points in your analysis, which is good. Keep it short and sweet. However, we propose you to think outside the box, diving deep into your data and trying to find the not obvious within the data. Your audience will be astonished 

