# 📊 KPI Catalog

This document defines standard KPIs used in Business Intelligence reporting and Qlik Sense dashboards.

---

## 💰 Revenue KPIs

### Total Revenue
Sum of all sales transactions.

```qlik
Sum(SalesAmount)

Net Revenue
Revenue after returns and discounts.
Sum(SalesAmount) - Sum(ReturnAmount)

👤 Customer KPIs
Active Customers
Number of unique customers with at least one transaction.
Count(DISTINCT CustomerID)

Customer Retention Rate
Percentage of returning customers.

📦 Sales KPIs
Total Orders
Total number of orders placed.
Count(OrderID)

Average Order Value (AOV)
Sum(SalesAmount) / Count(OrderID)

---

## 4. Commit message:

```text
Add KPI catalog definitions
