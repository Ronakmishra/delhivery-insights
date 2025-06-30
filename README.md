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
