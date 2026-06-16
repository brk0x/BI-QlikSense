# 📊 KPI Catalog

This document defines standardized Business Intelligence KPIs used in Qlik Sense dashboards.

---

# 💰 Revenue KPIs

## Total Revenue
Total sum of all sales transactions.

```qlik
Sum(SalesAmount)
```

---

## Net Revenue
Revenue after returns and discounts.

```qlik
Sum(SalesAmount) - Sum(ReturnAmount)
```

---

# 👤 Customer KPIs

## Active Customers
Number of unique customers with at least one transaction.

```qlik
Count(DISTINCT CustomerID)
```

---

## Customer Retention Rate
Percentage of customers who return and make repeat purchases.

> Formula depends on business definition.

---

# 📦 Sales KPIs

## Total Orders
Total number of orders placed.

```qlik
Count(OrderID)
```

---

## Average Order Value (AOV)
Average revenue per order.

```qlik
Sum(SalesAmount) / Count(OrderID)
```

---

# 📌 Notes

- All KPIs must be aligned with business definitions
- Single source of truth should be maintained
- KPI logic should be reused in Qlik Master Measures
