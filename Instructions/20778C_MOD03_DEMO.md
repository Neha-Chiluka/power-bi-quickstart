# Module 3: Power BI Data

- [Module 3: Power BI Data](#module-3-power-bi-data)
  - [Lesson 1: Using Excel as a Data Source for Power BI](#lesson-1-using-excel-as-a-data-source-for-power-bi)
    - [Demo 1: Importing Files from a Local Folder](#demo-1-importing-files-from-a-local-folder)
      - [Import Data from an Excel File](#import-data-from-an-excel-file)
      - [Import Data from a CSV File](#import-data-from-a-csv-file)
  - [Lesson 2: The Power BI Data Model](#lesson-2-the-power-bi-data-model)
    - [Demo 1: Creating a Hierarchy](#demo-1-creating-a-hierarchy)
      - [Creating a Hierarchy](#creating-a-hierarchy)
      - [Using a Hierarchy](#using-a-hierarchy)
  - [Lesson 3: Using Databases as a Data Source for Power BI](#lesson-3-using-databases-as-a-data-source-for-power-bi)
    - [Demo 1: Importing Data from SQL Server](#demo-1-importing-data-from-sql-server)
      - [Import Data from SQL Server](#import-data-from-sql-server)
      - [Import Data Using a Query](#import-data-using-a-query)


## Lesson 1: Using Excel as a Data Source for Power BI

### Demo 1: Importing Files from a Local Folder

#### Import Data from an Excel File

1. Ensure that you have copied all folders from `Desktop/power-bi-quickstart` folder into **D:\\** drive before starting the lab.

2. In the **D:\\Demofiles\\Mod03** folder, run **Setup.cmd** as Administrator.

3. In the **User Account Control** dialog box, click **Yes**.

4. If prompted to continue this operation, type **Y**, and then press Enter.

5. When the script completes, press any key to close the window.

6. On the taskbar, click **Power BI Desktop**.

7. To close the getting started window, at the top-right of the window, click **X**.

10. In the **Power BI Desktop** window, click **Get data**.

11. In the **Get Data** dialog box, click **Excel**, and then click **Connect**.

12. In the **Open** dialog box, navigate to **D:\\Demofiles\\Mod03\\Demo\\Files for Import**, click **Sales.xlsx**, and then click **Open**.

13. In the **Navigator** window, click **Sales** to show a preview of the data. Use the horizontal scrollbar to display the columns, select the **Sales** check box, and then click **Load**.

14. When the load completes, in the **FIELDS** pane, point out the **Sales** table. Mention that Power BI has detected columns that can be used in aggregations, as indicated by the **Sum** symbol next to the column names.

#### Import Data from a CSV File

1. On the **Home** tab, click **Get Data**.

2. In the **Get Data** dialog box, click **Text/CSV**, and then click **Connect**.

3. In the **Open** dialog box, navigate to **D:\\Demofiles\\Mod03\\Demo\\Files for Import**, click **SalesPerson.csv**, and then click **Open**.

4. In the preview window, drag the lower-right corner to enlarge the window and display more of the data, and then click **Load**.

5. In the **FIELDS** pane, expand the **SalesPerson** table to show the columns. Mention that the two tables from different sources are now available to use together in a report. If the report is published, the tables will be part of the same dataset.

6. On the **File** menu, click **Save As**, name the report **Adventure Works Sales 3**, and then save to the **D:\\Demofiles\\Mod03\\Demo** folder.

7. Leave Power BI open for the next demonstration.

---

## Lesson 2: The Power BI Data Model

### Demo 1: Creating a Hierarchy

#### Creating a Hierarchy

1. In the **FIELDS** pane, under **Sales**, right-click **Country**, and then click **New hierarchy**. The new hierarchy column is added.

2. Right-click **Territory**, point to **Add to hierarchy**, and then click **Country Hierarchy**.

3. Right-click **State Province**, point to **Add to hierarchy**, and then click **Country Hierarchy**.

4. Right-click **City**, point to **Add to hierarchy**, and then click **Country Hierarchy**.

5. Right-click **Country Hierarchy**, click **Rename**, type **Region Hierarchy**, and then press Enter.

6. In the **FIELDS** pane, under **Sales**, drag the **Total Due** column to the report canvas to create a new chart.

7. Drag the **Region Hierarchy** to the **Axis** in the **VISUALIZATIONS** pane.

8. Resize and move the chart on the canvas so it fills the report canvas.

9. In the **FIELDS** pane, under **Sales**, click the **Total Due** column to give it focus.

10. On the **Modeling** tab, click **Format: General**, point to **Currency**, and then click **$ English (United States)**.
#### Using a Hierarchy

1. In the top right-hand corner of the chart, click **Click to turn on Drill Down**. Notice that the arrow icon is now black.

2. Click the **United States** column in the chart to show the data by Territory. Notice that the chart title has changed.

3. Click the **Northwest** column, and again, notice that the chart title changes.

4. Click the **Oregon** column. Notice that the title of the chart has changed, and the down arrow in the top left-hand corner is disabled.

5. Click the **Drill Up** icon to return to the State Province level.

6. Click the **Drill Up** icon to return to the Territory level.

7. Click the **Expand all down one level in the hierarchy** icon to see the Total Due by Country, Territory, and State Province.

8. Leave Power BI open for the next demonstration.

---

## Lesson 3: Using Databases as a Data Source for Power BI

### Demo 1: Importing Data from SQL Server

#### Import Data from SQL Server

1. On the **Home** tab, click the **Get Data** arrow, and then click **SQL Server**.

2. In the **SQL Server database** dialog box, in the **Server** box, type **localhost**, in the **Database (optional)** box, type **AdventureWorks**, and then click **OK**.

3. If the **SQL Server database** dialog box appears, ensure the **Windows** tab is selected, click **Use my current credentials**, and then click **Connect**.

4. If the **Encryption Support** dialog box appears, click **OK**.

5. In the **Navigator** window, select the **Sales.vSalesPerson** and **Sales.vStoreWithDemographics** check boxes, and then click **Load**.

6. If the **Connection settings** window appears, ensure **Import** is selected, and then click **OK**.

#### Import Data Using a Query

1. On the **Home** tab, click the **Get Data** arrow, and then click **SQL Server**.

2. In the **SQL Server database** dialog box, in the **Server** box, type **localhost**, in the **Database (optional)** box, type **AdventureWorks**.

3. Expand **Advanced options**, and in the **SQL statement (optional, required database)** box, type **SELECT * FROM [Production].[Product]**, and then click **OK**.

4. In the **localhost: AdventureWorks** window, a preview of the data is displayed, and then click **Transform Data**.

5. In Power Query Editor, in the **ProductSubcategoryID** column, click the filter icon, and then click **Remove Empty**.

6. In the **Queries** pane, right-click **Query1**, click **Rename**, type **Products**, and then click **Close & Apply**.
