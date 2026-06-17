# SaaS B2B Sales Analytics — Power BI

End-to-end Power BI project simulating sales performance for a B2B SaaS company, built on a star schema (1 fact table + 5 dimension tables) with time-intelligent DAX measures for ARR, churn, and rep performance.

## Business Problem
A simulated SaaS company needs visibility into recurring revenue health (Active ARR, churn, expansion/contraction), not just total bookings — plus a way to drill into individual sales rep performance.

## Data Model
Star schema: `Fact_Sales` + `Dim_Date`, `Dim_Customer`, `Dim_Product`, `Dim_Geography`, `Dim_SalesRep`.

## Key DAX Measures
- **Active ARR**: recurring revenue currently in effect at any selected date (not just bookings) — calculated with `FILTER` + `SUMX` over contract start/end dates.
- **Churn Rate %, Expansion ARR, Contraction ARR**: SaaS-specific recurring revenue health metrics.
- **Time intelligence**: YTD, YoY growth, same period last year comparisons.

## Report Pages
1. **Executive Overview** — KPIs, monthly trend, deal type mix, sales by region.
2. **Product & Revenue Analysis** — ARR by product tier, segment matrix, COGS vs profit.
3. **Customer & Geography Analysis** — top customers, churn by segment, map view.
4. **Sales Rep Performance** (drill-through) — individual rep KPIs and deal history.


## Tools
Power BI Desktop · Power Query (M) · DAX · Star Schema Data Modeling
