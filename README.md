
# Toman Bike Share

### Dashboard Link : https://app.powerbi.com/links/ubkFangZwP?ctid=45f26ee5-f134-439e-bc93-e6c7e33d61c2&pbi_source=linkShare

## Problem Statement

The Toman Bike Share program seeks the development of a comprehensive dashboard to enhance decision-making by visualizing key performance metrics. The dashboard must include an hourly revenue analysis, profit and revenue trends, seasonal revenue insights, and rider demographics. It should follow the company's color scheme and be user-friendly. Access to the company's databases will be provided; if no database exists, one must be created. A preliminary version of the dashboard is needed as soon as possible. Additionally, recommendations on whether to raise prices next year should be included based on the data analysis. The objective is to create an effective dashboard that aids Toman Bike Share in strategic planning and operational improvements.

![Screenshot 2024-05-14 185444](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/8c18f4e4-dc0f-4b4c-83d7-be56104ec4fa)


### Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a SQL file.
- Step 2 : A matrix visual was added to the canvas representing hourly sales data across a week 
- Step 3 : A Line and Cluster chart was added to the canvas representing  the trend of key performance indicators (KPIs) over time, such as the number of riders, average profit, and average revenue. The insights provided visualize changes in the number of riders and financial performance over months, highlight seasonal patterns and trends, and help in understanding periods of high and low performance.  
- Step 4 : A Clustered Bar Chart was added to the canvas. This bar chart breaks down the revenue by different seasons, identifying which seasons generate the most revenue, showing the distribution of revenue across different times of the year, and revealing seasonal fluctuations, with season 3 being the most profitable at $1.7M.   
- Step 5 : A Donut Chart was added to the canvas. This chart shows the percentage distribution of different rider types, revealing that the majority of riders are registered (80.11%) while a smaller portion are casual riders (19.89%), providing insights into the composition of the user base. 
- Step 6 : I had to transform data because of an issue with cost of goods(COGS). COGS is COGS for each one of the bikes so we must multiply COGS by riders also | SQL code fix down below 
# Snapshot of Incorrect (RED) & Correct (GREEN) Code

![Screenshot 2024-05-14 174116](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/371fb811-20fb-41ad-a0fe-cc1194a1e5b3)

![Screenshot 2024-05-14 174058](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/184d49da-11e5-40c8-bd9c-725fb167fdcb)


- Step 7 : A Card is added to the canvas representing the revenue and profit for 2021 & 2022
- Step 8 : A Card is added to the canvas representing the overall rider engagement and the financial health of the Toman Bike Share program. To reach this conclusion, a new measure was used to calculate the profit margin 

![Screenshot 2024-05-14 182636](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/fc62e777-769b-4aaf-ba59-c5a81867df8c)

- Step 9 : A Slicer was added with the 'year' filter being used. This allows the viewer to see the different data from 2021 and 2022 seamlessly. 'Transform Data' was used to change (0,1) to (2021,2022), making it easier for the viewer to understand the data.

![Screenshot 2024-05-14 183629](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/8c86bf51-5b56-4db1-9d68-b638fa09938c)

- Step 10 : Evaluated whether we could raise the prices for the upcoming year using a table with (riders, revenue, profit)

- Step 9 : The report was then published to Power BI Service


# Snapshot of Dashboard (Power BI Service)

![Screenshot 2024-05-14 184905](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/840094ff-704f-4bc2-af9f-3e2ba7db6984)

 
 # Report Snapshot (Power BI DESKTOP)

 
![Screenshot 2024-05-14 185029](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/8b577f8f-688d-49a3-840f-056b29ceaef3)

# conclusion

We can consider a conservative price increase based on market factors driving demand. Given that our rider count has surged by 64%, it’s reasonable to explore a price adjustment. Previously, we increased the price by 25% (from $3.99 to $4.99). A conservative increase of 10-15% would set the new price at $5.49 to $5.74. I recommend starting with a 10% increase to $5.49. This approach allows us to test the market and gauge customer response before deciding on further adjustments.

![Screenshot 2024-05-14 184809](https://github.com/CyrusTruitt/CyrusTruitt/assets/169110603/2a850db1-5640-4292-a368-8657bcef1ccc)
