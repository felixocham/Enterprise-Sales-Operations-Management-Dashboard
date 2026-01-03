# 📊 Enterprise Sales & Operations Management Dashboard

![Power BI](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![SQL Server](https://img.shields.io/badge/Microsoft%20SQL%20Server-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

> **A full-stack BI solution providing 360° visibility into Sales, Supply Chain Operations, and Strategic Growth.**

---

## 📖 Project Overview
This project demonstrates an end-to-end Power BI implementation designed to bridge the gap between high-level strategic planning and day-to-day operational logistics.

The solution was built following a rigorous design lifecycle:
1.  **Data Engineering:** Data extraction from **SQL Server**, transformation/cleaning via **Power Query**, and star-schema modeling with a custom Fiscal Date Table.
2.  **UI/UX Design:** Wireframe mockups were sketched and color palettes defined prior to development to ensure an intuitive user experience.
3.  **Implementation:** Advanced DAX measures, bookmark navigation, and drill-through capabilities.
4.  **Documentation:** Full Model Dictionary created for governance.

---

## 🔎 Dashboard Views & Features

### 1. 🎛️ Dynamic Navigation & Filtering
The report utilizes a custom sidebar for seamless navigation between views.
* **Filter View:** A dedicated, collapsible pane containing slicers for **Fiscal Year, Fiscal Quarter, Product Category, Continent, and Country**. Includes "Clear All" and "Close" actions for a clean UI.

### 2. 📈 Executive Dashboard (Home)
High-level KPIs designed for quick performance assessment.
* **KPI Cards:** Sales, Orders, Profits, and Quantities (featuring QoQ% and Avg Monthly values).
* **Dynamic Measure Switching:** Radio buttons allow the user to toggle charts below to display **Sales, Orders, Profits, Quantities, or COGS**.
* **Visuals:**
    * *Line Chart:* Selected measure trends by month.
    * *Decomposition Tree:* AI-driven root cause analysis (break down by FY, Quarter, Country, Product, etc.).
    * *Ranking:* Top Products, Customers, and Countries.

### 3. 🚚 Operations View
Focused on logistics, supply chain efficiency, and order fulfillment.
* **KPIs:** Avg Days to Ship, On-time Delivery %, Late/Pending Orders, Total Orders.
* **Geographic Analysis:** Orders by Continent (Pie), Country, and Sales Rep.
* **Drill-Through Capability:** Hovering over visuals reveals details on specific orders (Status, Lead Time, Salesperson, Granular Items).
* **Inventory Alerts:**
    * *Late/Pending Table:* Tracks delayed shipments.
    * *Procurement Table:* clear icons distinguishing between items to **Place Order** vs. **Wait for Receipt**.

### 4. ♟️ Strategic View
Long-term growth analysis and year-over-year comparisons.
* **KPIs:** % YoY Sales, % Profit, % Margin, Average Order Value (AOV).
* **Advanced Analytics:**
    * *Decomposition Tree:* Deep dive into Sales drivers.
    * *Scatter Plot:* Analyzing Sales Volume vs. % Margin by Country.
    * *YoY Comparison:* Line chart comparing current vs. previous year performance.

### 5. 📄 Data View
A granular detailed view containing raw row-level data.
* *Note:* This tab is **hidden** from the main navigation. It is exclusively accessed via **Drill-through** from the Operations view when investigating specific Order IDs.

---

## 🛠️ Technical Stack
* **Data Source:** Microsoft SQL Server
* **ETL:** Power Query (M Language)
* **Modeling:** Power BI Desktop (Star Schema, One-to-Many Relationships)
* **Calculations:** DAX (Time Intelligence, Dynamic Measures, SWITCH functions)
* **Visuals:** Native Visuals, Decomposition Tree, Filled Maps, Custom SVG Icons.

---

## 🚀 How to Use This Dashboard
*Maximize your insights by following these navigation tips:*

* **Custom Filtering:** Click the **"Filter"** button on the left sidebar to open the slicer panel. Select your desired Fiscal Year or Region. Remember to click the **"Close"** button to maximize screen real estate after selecting.
* **Dynamic Analysis (Dashboard View):** Use the **Radio Buttons** below the KPI cards to change the context of the charts. For example, selecting "Profits" will instantly update the Line Chart and Decomposition Tree to show Profit trends rather than Sales.
* **Deep Dives (Decomposition Tree):** In the Dashboard or Strategic view, click the `+` sign on the Decomposition tree to break down a metric by any dimension (e.g., "Why are sales down?" -> Break down by "Country" -> "Product").
* **Drill-Through Details:** In the **Operations View**, if you see a metric concerning a specific country or sales rep, **hover your cursor** over the visual. A "Drill-through" button will appear in the tooltip. Click this to see the raw invoice/order level data in the Data View.
* **Action Items:** Check the bottom tables in the Operations view daily. Look for the **"Place Order" icon** to identify stock that needs immediate procurement.

---

## 📸 Gallery

| Executive Dashboard | 
|:---:|
| <img width="1796" height="1010" alt="image" src="https://github.com/user-attachments/assets/3d9acec5-85d9-49a7-94d7-fd00ac226ba5" />|
| <img width="1800" height="1012" alt="image" src="https://github.com/user-attachments/assets/036e24f8-5f4a-470f-a7c5-8c94dc47e943" />|


| Operations View |
|:---:|
| <img width="1798" height="1015" alt="image" src="https://github.com/user-attachments/assets/4276d3c4-559d-4da8-8a80-f5e9b9da43a0" /> |
| <img width="1796" height="1010" alt="image" src="https://github.com/user-attachments/assets/a70b3c85-303c-4802-bdd4-e6b0e68f3271" /> |
| <img width="1797" height="1006" alt="image" src="https://github.com/user-attachments/assets/2846d6ad-40e9-4323-881d-7371cdf440e3" /> |
| <img width="1795" height="1007" alt="image" src="https://github.com/user-attachments/assets/78d7d995-cb2d-413e-b524-3a806b6c5b01" /> |

| Strategic View | 
|:---:|
| <img width="1798" height="1011" alt="image" src="https://github.com/user-attachments/assets/3409113b-2533-4300-b4db-08f57a03de68" />|
| <img width="1539" height="865" alt="image" src="https://github.com/user-attachments/assets/d9f1d96f-24e0-4551-a006-c67ae77ad74a" /> |
| <img width="1542" height="868" alt="image" src="https://github.com/user-attachments/assets/aafe6c3c-0112-4b86-a715-86dfe326c34a" /> |

| Filter Pane |
|:---:|
| <img width="1794" height="1011" alt="image" src="https://github.com/user-attachments/assets/0154b193-ab7e-4cbf-b2ff-e95de41db248" />|

| Info Page |
| :---: |
| <img width="1544" height="871" alt="image" src="https://github.com/user-attachments/assets/35609fb7-b496-41f7-8d66-f92ca9b9dbf6" /> |

| Model Dictionary|
| :---: |
| <img width="1542" height="867" alt="image" src="https://github.com/user-attachments/assets/49fafc86-108d-479f-9439-dbe1ee999321" /> |

| Model Relationships|
| :---:|
| <img width="1176" height="856" alt="image" src="https://github.com/user-attachments/assets/c259c2a5-bfe0-4bbc-a9a4-bd745cbfb573" /> |

| Wireframe Mock ups|
| :---:|
| <img width="1288" height="730" alt="image" src="https://github.com/user-attachments/assets/15cfc943-bb25-484f-80ae-4f0d9b8ae144" /> |
| <img width="1287" height="725" alt="image" src="https://github.com/user-attachments/assets/f91d0f0e-c5ed-4c12-86ef-3b2a403b2771" /> |
| <img width="1291" height="718" alt="image" src="https://github.com/user-attachments/assets/d1a94d39-0f76-4fa9-bd63-d9db7f695f49" /> |
| <img width="1282" height="721" alt="image" src="https://github.com/user-attachments/assets/4cafbff9-9546-478b-add9-1331af231fc1" /> |
| <img width="1291" height="715" alt="image" src="https://github.com/user-attachments/assets/c7f6bcd3-7e7d-4031-ba36-6ad2991d54a7" /> |

---

## 🙏 Acknowledgements & Inspiration
Special thanks to the following creators and resources for their tutorials on advanced Power BI techniques used in this project:

* **SQLBI** - [Creating custom visuals in Power BI with DAX](https://www.youtube.com/watch?v=JG5EbW1wr70&t=1875s)
* **Maven Analytics** - [Document Power BI Models in SECONDS with TMDL + AI](https://www.youtube.com/watch?v=stSAZlyTz74)
* **Lets Talk Data** - [Transform Power BI Tables using SVGs](https://www.youtube.com/watch?v=Uwvek8pG9Xg&t=1420s)
* **Next Level Power BI Reports** - [Design Next Level Power BI Filter Panes](https://www.youtube.com/watch?v=nbpdEcc-8Kc)
* **W3 Schools** - [SVG Introduction](https://www.w3schools.com/graphics/svg_intro.asp)

---

*Developed by [Your Name]*
