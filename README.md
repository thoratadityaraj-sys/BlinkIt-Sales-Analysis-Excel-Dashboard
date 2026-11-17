# 🛒 Blinkit Sales Analysis | Excel Dashboard

![Dashboard Preview](images/dashboard-full.png)

> An interactive Excel dashboard that turns 8,500+ rows of grocery order data
> into actionable insights on sales, outlets, and product performance.

**Tools used:** Microsoft Excel (Pivot Tables, Pivot Charts, Slicers, Power-user formatting)

---

## 📌 Business Problem

Blinkit is India's quick-commerce grocery delivery app, delivering from
outlets located close to customers. Management needs to understand:

- How is overall sales performance trending?
- Which product categories and fat-content types drive revenue?
- How do outlet size, location tier, and outlet type affect sales?
- Do older outlets perform better than newer ones?

**Goal:** Build a dynamic dashboard so stakeholders can slice the business
by outlet size, location tier, and item type and make data-driven decisions.

---

## 📊 About the Data

| Detail | Info |
|---|---|
| Rows | ~8,500 orders |
| Columns | 12 |
| Source | Sample/replica dataset (not real company data) |

**Key fields:** Item Fat Content, Item Type, Item Identifier, Outlet
Establishment Year, Outlet Size, Outlet Location Type, Outlet Type,
Item Visibility, Item Weight, Sales, Rating.

### 🧹 Data Cleaning
- Standardized inconsistent labels in *Item Fat Content*
  (`LF`, `low fat` → **Low Fat**; `reg`, `R` → **Regular**)
- Checked for blanks/errors in mandatory fields (Sales, Outlet fields);
  null values in non-mandatory fields (Item Weight, Rating) were left as-is
- Converted the range into an Excel Table for easy Pivot Table creation
- Added a serial number column to count items

![Cleaning](images/data-cleaning-before-after.png)

---

## 🎯 KPIs

| KPI | Value |
|---|---|
| Total Sales | $1.2M |
| Average Sales | $141 |
| Number of Items | 8,523 |
| Average Rating | 4.0 |

---

## 📈 Analysis & Visualizations

| Requirement | Chart Used |
|---|---|
| Total sales by fat content | Donut chart |
| Total sales by item type | Bar chart |
| Fat content by outlet | Clustered bar chart |
| Sales by outlet establishment year | Area/line chart |
| Sales by outlet size | Donut chart |
| Sales by outlet location | Funnel chart |
| All metrics by outlet type | Bar charts (total sales, avg sales, items) |

*(Embed 2-3 of your best chart screenshots here)*

### Interactivity
- 3 slicers: **Outlet Size, Outlet Location, Item Type**
- All slicers connected to every pivot table via Report Connections
- Navigation buttons (Home → Pivot sheets, Data → raw data)

---

## 🔍 Key Insights

*(This is the most important section. Write YOUR findings.)*

- Low Fat items contribute **[X]%** of total sales vs **[Y]%** Regular
- **[Item type]** is the top-selling category, followed by **[ ]**
- **[Medium/High/Small]** outlets generate the most sales
- **Tier [ ]** locations lead in revenue
- Outlets established in **[year]** show the highest sales
- Average rating stays around 4.0 across segments

---

## 💡 Recommendations

1. Stock more of the top-selling categories ([ ]) in high-performing outlets
2. Investigate underperforming outlet sizes/tiers for growth opportunities
3. Promote [Low Fat/Regular] items where demand is higher

---

## ⚠️ Limitations & Next Steps

**Limitations**
- Dataset is a sample, not real-time or real company data
- No date/time column, so true trend and seasonality analysis wasn't possible
- Missing values in Item Weight and Rating limit some analysis
- No cost/profit data, so only sales (not profitability) was analyzed

**Next Steps**
- Rebuild the same dashboard in **Power BI** and **SQL**
- Add time-series analysis if order dates become available
- Add profit and customer-segment analysis

---

## 📂 Repository Contents
- `Blinkit_Dashboard.xlsx` – final dashboard
- `data/` – raw dataset
- `images/` – screenshots

## 👤 Author
**Adityaraj Thorat**
[LinkedIn](your-link) | [Email](your-email)
