LECTURE ONE: Adding and Exploring Data Sources in Tableau
---------------------------------------------------------
Objectives
----------
- Load data into Tableau
- Customize dimensions and measures (columns/features) in the Workspace
- Make elementary visualizations

**First, make sure you have a copy of Tableau Public!**
- Detailed instructions to download Tableau Public can be found [here](https://github.com/learn-co-curriculum/dsc-v3-tableau-public-getting-started/blob/main/README.md) .
- Ensure all students have created a Tableau Public account and downloaded Tableau Public.
* Students should be able to follow along using their own Tableau accounts.
* This first lecture is about making sure students can connect to Tableau and perform some basic data manipulations.
* The general structure of this lecture is first to demonstrate some technique and then to have students perform a similar manipulation.

1. **Importing Data/ Populate the Data Souce page**
	1. Download **pop_soda_data.csv and 2019_Census_US_Population_Data_By_State_Lat_Long.csv** in the data folder to ~Documents/My Tableau Repository/Datasources
	2. From the Start page, select **Connect > To a File > Text File**. Select pop_soda_data.csv. This will launch the Data Source page.
	3. Populate the data source page by dragging the table to the Canvas.
		1. You will notice that other files in the same directory can also be accessed from the data pane.
		2. Drag the 2019_Census_US_Population_Data_By_State_Lat_Long.csv from the Data pane to the Canvas. Because both tables have a State column, Tableau intuits a relationship between them (eliminating the need to do a join)
	4. Before adding a new worksheet, take a look at the **data** and **metadata** tables to get a sense of the dataset. These two elements appear on the screen after you populate the Data Source page in Step 3.
		* Screen will look like this before populating the Data Source page 
			![[tab-2-2-data-source.png]]
		* Screen will look like this after populating the Data Source page.
			![[workbook2.png]]

	1. This lesson contains detailed instructions (with screenshots and/or videos) on importing data/populating the data source page: [Tableau Public - Data Source Page and Tableau Workspace] (https://github.com/learn-co-curriculum/dsc-v3-tableau-public-data-source-page)
	2. This lesson contains detailed instructions (with screenshots and/or videos) on customizing data sources (look in the second half of the lesson under the heading "Your Turn: Create a Custom Data Source"): [Tableau Public - Customizing Data Sources] (https://github.com/learn-co-curriculum/dsc-v3-tableau-public-customizing-data-sources) 

2. **Build a Simple Visualization**
	1. Switch to a Worksheet tab and build a simple visualization. You can use this example, or come up with an example of your own.
		1. **Example:** 
		2. 2019 US Population by State (Regional Map - Count)
		3. 2019 US Population by State (Regional Map - Percentage)
		4. Terms for Soft Drinks in Top-5 Most Populous States (Bar Chart)
	2. **Make sure to demonstrate the technique of dragging dimensions and measures (columns) from the Data pane to the Marks card and adding different attributes**. 
		1. This lesson has detailed instructions on how to use the Marks card to change attributes (colors, labels, marks, sizes) [Tableau Visualizations - Tableau Visualization Basics Lab](https://github.com/learn-co-curriculum/dsc-v3-tableau-visualizations-lab). 
	3. **Discuss accessibility** 
		1. During the discussion about adding color, you should mention that it is important to consider accessibility when choosing a color palette. 
		2. You can use the Coblis Color Blind Simulator (https://www.color-blindness.com/coblis-color-blindness-simulator/) with this example image (color-example-1.png) to discuss how certain color combinations can make the information in the viz more difficult to interpret. 

3. **Visualization Workshop**
	1. Give students around five minutes to try loading the datasets on their own and linking them on the Data Source page. You may want to take a volunteer or two to share their work.
	4. When everyone has loaded the data, demonstrate a visualization.
	5. You can use one of these examples, create your own example, or allow students to suggest an example.
		2. 2019 US Population by State (Regional Map - Count)
		3. 2019 US Population by State (Regional Map - Percentage)
		4. Terms for Soft Drinks in Top-5 Most Populous States (Bar Chart)
	6. Allow students time to re-create the example, or come up with one of their own.
