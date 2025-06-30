# Delhivery Analytics Dashboard

A modern, interactive analytics dashboard for Delhivery’s supply chain operations—built to mirror client website aesthetics and empower stakeholders with actionable data insights.

## 🚚 Project Overview

This project delivers a comprehensive **Supply Chain Analytics Dashboard** tailored for Delhivery, India’s leading logistics provider. The solution focuses on real-time order tracking, operational visibility, and multi-dimensional analytics—adhering strictly to the client’s brand and usability requirements.

**Key Objectives:**

- Mirror the look and feel of the Delhivery website
- Provide real-time tracking of orders, revenue, product availability, defects, leakages, breakage, and shipping costs
- Enable deep-dive analytics by product, product type, carrier, location, and supplier
- Allow full data export/download in tabular format
- Deliver advanced filtering (“slice and dice”) and drilldown capabilities

## 📊 Dashboard Features

- **Order Tracking:** Monitor how many orders are dispatched from the warehouse.
- **Revenue Analytics:** Real-time revenue reporting across products, locations, and time.
- **Product Availability:** View current stock levels and availability percentages.
- **Defect & Leakage Monitoring:** Track product defect rates, leakage, and breakage incidents.
- **Shipping Cost Analysis:** Visualize shipping costs per order and unit.
- **Safety Metrics:** Multi-level safety tracking (by product, product type, carrier, etc.)
- **Unit Contribution:** Analyze sales contribution by individual units.
- **Comprehensive Filters:** Dynamic filters for Location, Gender, Role, Carrier, Product, and more.
- **Data Download:** One-click export of the complete dashboard dataset in a tabular format.

## 🗃️ Dataset Description

The dataset is sourced from Delhivery’s operations and contains **18 columns**:

| Column Name         | Description                            |
| ------------------- | -------------------------------------- |
| CARRIER             | Carrier or logistics provider          |
| CUSTOMER Gender     | Gender of the customer                 |
| LOCATION            | Transaction location                   |
| MODE                | Mode of delivery                       |
| PRODUCT             | Product name/ID                        |
| PRODUCT TYPE        | Category/type of product               |
| ROUTE               | Shipping/delivery route                |
| SUPPLIER            | Product supplier                       |
| AVAILABILITY (PCT)  | Product availability percentage        |
| DEFECT RATE (PCT)   | Percentage of products with defects    |
| ORDERS              | Number of orders                       |
| PRICE               | Price per unit                         |
| PRODUCTION          | Production figures                     |
| PRODUCTS SOLD       | Number of products sold                |
| REVENUE             | Total revenue generated                |
| STOCK LEVEL         | Current inventory/stock level          |
| Shipping costs      | Cost incurred for shipping             |
| Year of Transaction | Year in which the transaction occurred |

**Note:** The data was provided in CSV format, consolidated and verified for quality before loading into Snowflake.

## 🏗️ Architecture & Data Flow

- **Data Source:** Original CSV files from client
- **Warehouse:** All data loaded and managed in Snowflake (no more Excel/CSV dependence)
- **BI Tool:** Tableau, connected directly to Snowflake for a live connection

---

## 🖥️ Dashboard Filters

The following filters are available to slice and dice the data:

- Location
- Customer Gender
- Roles
- Carriers
- Products
- Product Type
- Year of Transaction
- Supplier
- Mode

---

## 🚦 Data Modeling

- All CSVs are consolidated in Snowflake as normalized tables.
- Relationships modeled for accurate joins across entities (Product, Supplier, Carrier, etc.).
- Star/Snowflake schema (as appropriate) for optimized querying.

---

## 🔗 How to Use

1. **Connect Tableau to Snowflake:**  
   Configure your Tableau instance to connect to the Snowflake warehouse containing the project data.
2. **Explore the Dashboard:**  
   Use filters to drill down into specific business dimensions.
3. **Export Data:**  
   Click the download button in the dashboard for a full data export in tabular format.

---

## 📊 Dashboard Demo

### Dashboard

![Dashboard Walkthrough](gif.gif)

---

## 🗺️ Data Model

![Data Model](DataModel.png)

---

## 📁 Repository Structure

```text
/
├── Delhivery Datasets/
├── Delhivery Dashboard.twbx
├── README.md
├── db1.png
├── db2.png
├── db3.png
├── gif.gif
├── datamodel.png
├── info project.docx
```
