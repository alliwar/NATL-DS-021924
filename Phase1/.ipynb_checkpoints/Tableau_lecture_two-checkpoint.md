## Objectives
* Experiment with different vizzes
* Combine the vizzes into a dashboard

## Overview
The primary purpose of this lecture is to illustrate how to build a dashboard in Tableau. It utilizes a dataset that contains historical information about soccer games played in the German Bundesliga from 1963-2020.

### Procedure
1. First, we'll walk through the construction of several vizzes. 
2. Then, we will use them to build out a dashboard.
3. Finallly, we will leave time for students to experiment on their own.

### 1. Build Vizzes
Use these examples to quickly review the procedure for building data vizzes in Tableau. 

1. **Line Chart**: "SC Freiburg's Home Goals Year over Year":
	* Add the `Home Team` dimension to the workspace and filter for SC Freiberg.
	* The screen should look like this:
<img width="750" alt="freiburg_home_goals_line_chart" src="https://user-images.githubusercontent.com/116017015/231609077-de1270ff-a406-47da-a038-29adee0c5e5b.png">
                                  
2. **Packed Bubble Chart**: "Teams Having 1000+ Home Goals (with less than 1000 goals given up at home)"
* Demonstrate how to:
	* Drag the `Home Team` dimension into your to the Columns shelf.
	* Drag the `Home Goals` and the `Away Goals` measures to the **Filters Card**. (These goals will be automatically summed)
	* Drag the `SUM(Away Goals)` to the **Marks Card** and assign the **Size attribute**.
	* Drag the `Home Team` dimension and `SUM(Home Goals)` and `SUM(Away Goals)` to the **Marks Card** and assign them the **Label attribute**.
	* Drag the `SUM(Home Goals)` measure to the **Marks Card** and assign the **Color attribute**.
  * The screen should look like this:
<img width="750" alt="teams_1000+_home_goals_1000-_away_goals" src="https://user-images.githubusercontent.com/116017015/231608996-df6f8a40-6e09-438a-9798-0d6bf8769feb.png">

3. **Scatter Plot:**  Example - "Teams with 40+ Goals in 1964"
* Demonstrate how to:
	* use Filter to include only the 1964 for the `Year` dimension.
	* add `Home Goals` to the Rows shelf and `Away Goals` to the Columns shelf.
	* change the marker shape from "Default" to "Filled"
* The screen should look like this:
	<img width="750" alt="teams_40+_home_goals_1963-4" src="https://user-images.githubusercontent.com/116017015/231609363-db415a0e-a71b-431d-ab99-f75d165227fb.png">

4. **Horizontal Bar Chart:** "Teams with 350+ Goals during Away Games"
* Demonstrate how to:
	* Bring in the` Away Team` dimension and the `Away Goals` measure into your workspace and then filter on `Away Goals`. 
	* Use the **Sort Descending** on the tool bar to sort by `Away Goals`
* The screen should look like this:
	<img width="750" alt="teams_350+_away_goals_sorted" src="https://user-images.githubusercontent.com/116017015/231609421-86c71d92-420e-47c0-abee-4382294103b5.png">


### 2. Build Dashboard
Now: Add some or all of these worksheets to a new dashboard. 

For a detailed instructions and visual aids regarding how to demo/discuss the items below, see these resources:
[Short Video: Tableau Dashboards](https://learning.flatironschool.com/courses/6948/pages/short-video-tableau-dashboards-dashboard-layouts)
[Tableau Dashboard Basics](https://github.com/learn-co-curriculum/dsc-v3-tableau-dashboard-basics)
[Tableau Dashboard Basics Lab](https://github.com/learn-co-curriculum/dsc-v3-tableau-dashboard-lab)

#### Demonstration Items
Example image:
<img width="750" alt="dashboard" src="https://user-images.githubusercontent.com/116017015/231612048-d507b200-961c-41a1-a3ba-23b5ad3d0f62.png">

1. Use the **Sheets Tab** to create a new dashboard.
2. Use the **Device Type Card** to create a new layout (for Desktop).
3. Use the **Objects Card** to set the dashboard to a **Tiled Layout**.
4. Use the **Objects Card** to add **Horizontal** and **Vertical Containers** to the dashboard.
5. Use the **Dashboard Pane** to drag sheets/vizzes onto the dashboard. 
6. Use the **More Options** menu to apply a filter of your choice.

#### Discussion Items
#### A. Layouts 
##### Device Type Options
* Discuss the need to consider the end user and what kind of device they will use to access the dashboard.
###### Object Placement: Floating vs Tiled
* If you set the layout to "Floating" you can put each chart exactly where you want. The drawback is that your layout may appear skewed in different resolutions.
* If you set the layout to "Tiled", the ability to position charts is less flexible, but the layout will be more resilient to different resolutions.

#### B. Filters/Dynamic Updates
* Change one of the underlying worksheets to demonstrate that the dashboard automatically updates to reflect the changes.
* Demonstrate how using filters on the worksheets versus the dashboards changes the appearance of the dashboard.

### 3. Students Build a Dashboard
Give students some time to work on their own dashboard.

##### Viz Examples for Students
Here are some examples of vizzes they could build:
1. Build a line chart of the away goals year over year for Bayern München or Borussia Mönchengladbach.
2. Use a bar chart to illustrate the average home goals scored for every home team.
3. Build a packed bubble chart of the teams that have at least 1000 away goals and at most 1000 goals given up on the road.

***Make sure to use the Away Team dimension!***
