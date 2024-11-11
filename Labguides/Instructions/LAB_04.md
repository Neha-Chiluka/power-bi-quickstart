# Module 4: Filters , Visualizations And Data Pane

In our default view( i.e Report View) we have filters, visualizations and data panes which are indeed adds up to the part of data analysis part.

**Note:- This is a theory explanation of all the features in the panes**

![1](https://github.com/Neha-Chiluka/power-bi-quickstart/blob/master/Images/8.png?raw=true "1")


**1. Filters in Power BI (Filter Pane)**

Filters allow you to control which data is displayed in your report, and they provide an interactive way for users to drill down and segment data on the report.

**Types of Filters**

There are three main types of filters in Power BI:

- **Visual Level Filters:** These filters apply only to a specific visualization. If you apply a filter to a visualization, it only affects that chart or graph, not the entire report.

*Example: If you apply a filter on a bar chart to only show data for "2023", the other visualizations on the report will not be affected.*

- **Page Level Filters:** These filters apply to all visualizations on a specific page or tab of your report. They are useful when you want to apply a uniform filter across the page but leave other pages unaffected.

*Example: If you apply a filter for "Region = North America" on a page, all visualizations on that page will reflect this region-specific data.*

- **Report Level Filters:** These filters apply to every visualization in the entire report, regardless of the page. They are global filters that ensure consistency across all pages in the report.

*Example: If you apply a filter for "Year = 2023" at the report level, all pages in the report will show only data from 2023.*


**Using Filters in Power BI**

You can drag fields from your Fields pane to the Filters pane (located on the right side of the Report View).

When you drag a field to the filter area, you can define specific conditions to filter the data, such as:

![2](https://github.com/Neha-Chiluka/power-bi-quickstart/blob/master/Images/10.png?raw=true "2")

- **Basic filtering:** Select specific values (e.g., regions, products).

- **Advanced filtering:** Set conditions like "greater than", "less than", or "equals".

- **Top N filters:** Show only the top or bottom N items based on a specific measure (e.g., top 10 sales).

You can apply filters either to individual visualizations or across the entire report depending on the level at which you want the filter to apply.

**Filter Pane Options**

- **Basic Filtering:** Select or deselect individual categories.

- **Advanced Filtering:** Create conditional filters (e.g., showing data where sales > $1,000).

- **Relative Date Filtering:** Filter by time periods, such as "Last 7 days," "This quarter," etc.

- **Searchable Filters:** For fields with many distinct values, you can search to quickly find and apply filters.


------------


**2. Visualizations in Power BI (Visualizations Pane)**

The Visualizations pane in the Report View allows you to choose the type of visualization that best represents your data, such as charts, graphs, maps, tables, and more. These visualizations are interactive and can be customized to fit the specific needs of your report.

![5](https://github.com/Neha-Chiluka/power-bi-quickstart/blob/master/Images/9.png?raw=true "5")

**Common Types of Visualizations**

- **Bar and Column Charts:** Display data with rectangular bars (horizontal or vertical). Bar charts are great for comparing categories, while column charts are better for time-based data or comparisons across categories.

- **Line Chart:** Useful for showing trends over time, making it great for time-series analysis.

- **Pie and Donut Charts:** Good for showing proportions or percentages of a whole.

- **Tables:** Display data in a tabular format. Useful for detailed data presentation.

- **Matrix:** Similar to a table, but with the ability to group data by rows and columns, making it ideal for hierarchical data or multi-dimensional analysis.

- **Card and KPI Visuals:** Display single values like total sales or key performance indicators (KPIs), such as target vs. actual metrics.

- **Tree Map:** Displays hierarchical data using nested rectangles. The size and color of the rectangles can represent values and categories.

- **Map Visualizations:** Plot data on a map using geographical information (e.g., country, state, zip code) to visualize location-based data.

- **Slicers:** Interactive filters that allow users to select data to display in the report. Slicers work similarly to filters but are visible on the report page, enabling users to modify the report view dynamically.

- **Funnel Chart:** Shows data progression through stages, often used for sales or marketing pipelines.

- **Waterfall Chart:** Helps to visualize cumulative changes in a measure over time, showing how values build or deplete in a sequential manner.

**Custom Visuals**
In addition to the standard visuals, Power BI allows you to import custom visuals from the AppSource marketplace or create your own custom visualizations using tools like the Power BI developer tools. These can add specialized chart types or other visualizations to suit specific needs.

**Interactivity with Visualizations**
- **Cross-filtering and Cross-highlighting:** When you select an item in one visualization (e.g., a bar in a bar chart), other visualizations on the report are automatically filtered or highlighted to reflect that selection.
- **Drillthrough:** Allows users to right-click on a data point in a visualization and drill through to a detailed page that shows more granular data based on that specific point.
- **Tooltip:** Hovering over a visualization shows additional information or metrics related to the data point being hovered over. Tooltips can be customized to show relevant details.


------------


**3. Data Columns in Power BI (Fields Pane)**

The data pane in the Report View displays the data columns and tables from the data model you’ve imported or created. These fields in the tables are used to create your visualizations and filters.

**Note: You will be able to see these fields when you import tables into PowerBI(Which you will be learning in advanced level of PowerBI labs)**

**Below is a sample image**

![4](https://github.com/Neha-Chiluka/power-bi-quickstart/blob/master/Images/11.png?raw=true "4")

**Organizing Data Columns**

- **Tables:** In the Fields pane, data is organized into tables (which represent your data sources or queries). You can expand or collapse tables to see the columns within them.

- **Columns:** Each table contains columns, which represent individual data fields (e.g., "Sales Amount," "Product Name," "Region"). These columns can be used in your visualizations and filters.

- **Measures:** In addition to regular columns, you may have calculated measures (e.g., Total Sales, Average Revenue), which are calculations made based on other columns. Measures are typically defined using DAX (Data Analysis Expressions).

**Using Data Columns in Visualizations**

**Drag and Drop**: You can drag and drop columns and measures from the Fields pane into visualizations. 

**For example:**
*Drag a "Product Category" field into the Axis of a column chart.
Drag a "Sales Amount" measure into the Values of a chart.
Use columns in the Legend or Details areas of certain visualizations (like pie charts or scatter plots).*

- **Field Formatting**
You can format data columns by clicking on a column or measure and adjusting its properties. 

**For example:**
*Set the data type (e.g., Text, Number, Date).
Adjust number formatting (e.g., currency, percentage, decimal places).
Customize the way data is displayed in visualizations (e.g., changing font sizes, colors).*


- **Filters:**
Apply filters to specific visualizations, pages, or the entire report.
Use basic, advanced, or relative date filters to control data visibility.

- **Visualizations:**
Choose from a wide variety of charts, tables, maps, and custom visuals to represent your data.

Interact with visuals using cross-filtering, drillthrough, and tooltips.
Customize the appearance and behavior of visualizations to communicate insights effectively.


------------


