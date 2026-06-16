# 🧠 Data Model Design (Qlik Sense)

This document describes the logical data model used in Qlik Sense analytics applications.

---

# 📌 Data Model Type

Star Schema is used for optimal performance and simplicity.

---

# ⭐ Star Schema Structure

```text
                DimDate
                   │
DimCustomer ── FactSales ── DimProduct
                   │
               DimRegion
```

---

# 📊 Fact Table

## FactSales

Contains transactional sales data.

### Fields:
- OrderID
- CustomerID
- ProductID
- SalesAmount
- Quantity
- OrderDate

---

# 📁 Dimension Tables

## DimCustomer
- CustomerID
- CustomerName
- Segment
- Country

## DimProduct
- ProductID
- ProductName
- Category

## DimDate
- Date
- Year
- Month
- Quarter

## DimRegion
- RegionID
- RegionName

---

# ⚙️ Design Principles

- Avoid synthetic keys
- Use proper key naming conventions
- Normalize dimensions
- Optimize for Qlik associative engine

---

# 🚀 Benefits

- Faster dashboard performance
- Easier maintenance
- Scalable architecture
- Better user experience
