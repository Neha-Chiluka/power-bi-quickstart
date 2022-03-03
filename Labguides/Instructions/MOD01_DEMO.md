# Module 1: Introduction to Self-Service BI Solutions

- [Module 1: Introduction to Self-Service BI Solutions](#module-1-introduction-to-self-service-bi-solutions)
  - [Lesson 2: Introduction to Data Analysis](#lesson-2-introduction-to-data-analysis)
    - [Demo 1: Importing Data with Power BI Desktop](#demo-1-importing-data-with-power-bi-desktop)
  - [Lesson 3: Introduction to Data Visualization](#lesson-3-introduction-to-data-visualization)
    - [Demo 1: Visualizing Data with Power BI Desktop](#demo-1-visualizing-data-with-power-bi-desktop)

## Lesson 2: Introduction to Data Analysis

### Demo 1: Importing Data with Power BI Desktop

1. Ensure that you have copied all folders from `Desktop/power-bi-quickstart` folder into **D:\\** drive before starting the lab.

2. In the **D:\\Demofiles\\Mod01** folder, run **Setup.cmd** as **Administrator**.

3. In the **User Account Control** dialog box, click **Yes**.

4. If prompted to continue this operation, type **Y**, and then press Enter.

5. When the script completes, press any key to close the window.

7. On the desktop, double-click **Power BI Desktop**.

8. To close the getting started window, at the top-right of the window, click **X**.

11. On the **Power BI Desktop** screen, click **Get data**.

12. In the **Get Data** dialog box, click **SQL Server**, and then click **Connect**.

13. In the **SQL Server** dialog box, in the **Server** box, type **localhost**.

14. In the **Database (optional)** box, type **AdventureWorksDW**, and then click **OK**.

15. In the **SQL Server** dialog box, leave the default settings unchanged, and then click **Connect**.

16. In the **Encryption Support** dialog box, click **OK**.

17. In the **Navigator** dialog box, select the **FactInternetSales** check box.

18. Click **Select Related Tables**, and then click **Transform Data**.

19. If the **Connection Settings** dialog box appears, leave **Import** selected, and then click **OK**.

20. In the **Power Query Editor** window, in the **Queries** pane, click **FactInternetSales**.

21. Right-click the **CarrierTrackingNumber** column, and click **Remove**.

22. Right-click the **CustomerPONumber** column, and click **Remove**.

23. In the **Queries** pane, click **DimCustomer**.

24. Right-click the **Title** column, and click **Remove**.

25. Right-click the **NameStyle** column, and click **Remove**.

26. Right-click the **Suffix** column, and click **Remove**.

27. Right-click the **MaritalStatus** column, and click **Replace Values**.

28. In the **Replace Values** dialog box, in the **Value To Find** box, type **M**.

29. In the **Replace With** box, type **Married**, and then click **OK**.

30. Right-click the **MaritalStatus** column, and click **Replace Values**.

31. In the **Replace Values** dialog box, in the **Value To Find** box, type **S**.

32. In the **Replace With** box, type **Single**, and then click **OK**.

33. Right-click the **Gender** column, and click **Replace Values**.

34. In the **Replace Values** dialog box, in the **Value To Find** box, type **F**.

35. In the **Replace With** box, type **Female**, and then click **OK**.

36. Right-click the **Gender** column, and click **Replace Values**.

37. In the **Replace Values** dialog box, in the **Value To Find** box, type **M**.

38. In the **Replace With** box, type **Male**, and then click **OK**.

39. On the **Home** menu, click **Close & Apply**.

40. Wait until the data has successfully loaded.

41. In the **FIELDS** pane, expand **FactInternetSales**, and then click **SalesAmount**.

42. On the **Modeling** tab, in the **Formatting** group, click **Format: Currency general**, point to **Currency**, and then click **$ English (United States)**.

![](./images/20.png)

43. In the **FIELDS** pane, right-click **DimCustomer**, and then click **New column**.

44. In the formula bar, type **FullName = DimCustomer[MiddleName] & " " & DimCustomer[LastName]**, and then press Enter.

45. On the **File** menu, click **Save**. Name the file **Adventure Works Sales**, and save the file to **D:\\Demofiles\\Mod01**.

46. Leave Power BI Desktop open for the next demonstration.

---

## Lesson 3: Introduction to Data Visualization

### Demo 1: Visualizing Data with Power BI Desktop

1. In Power BI Desktop, in the **FIELDS** pane, under **DimCustomer**, select **Gender**, and **MaritalStatus**.

2. Under **FactInternetSales**, select **SalesAmount**.

3. In the **VISUALIZATIONS** pane, click **Clustered column chart**. 

4. Click **Format**, expand **Title**, and then change the **Title text** to **Sales by Gender and Marital Status**.

![](./images/21.png)

5. Change **Alignment** to **Center**.

6. In the **FIELDS** pane, expand **DimProduct**, and drag the **Color** field onto the report canvas to create a new table.

7. Under **FactInternetSales**, drag the **OrderQuantity** field onto the new table.

8. In the **VISUALIZATIONS** pane, click **Donut chart**.

9. Click **Format**, and then expand **Title**.

10. Change the **Title text** to **Orders by Color**.

11. Change **Alignment** to **Center**.

12. In the **FIELDS** pane, under **FactInternetSales**, drag the **SalesAmount** field onto the report canvas to create a new column chart.

13. In the **VISUALIZATIONS** pane, click **Fields**.

14. In the **FIELDS** pane, expand **DimDate**, and drag the **EnglishMonthName** to the **Axis** property.

15. Grab the resizer on the column chart to widen the chart so that the month names display clearly.

16. In the **VISUALIZATIONS** pane, click **Format**, and then expand **Title**.

17. Change the **Title text** to **Sales by Month**.

18. Change **Alignment** to **Center**.

19. On the **File** menu, click **Save**.
