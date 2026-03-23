Walmart Sales Executive Summary — Google Sheets Analysis
  Project Overview
This project analyses Walmart's sales performance by department in 2012, identifying each department's contribution to total revenue and evaluating space efficiency. The analysis serves as a foundation for data-driven commercial decision making.

  Objective
Evaluate departmental sales performance to identify which departments contribute most to total revenue and which are most efficient in their use of store space — helping prioritise business strategies and infrastructure investments.

  File Structure
SheetDescriptionTyperaw_ventasOriginal weekly sales data by store and departmentRaw Dataraw_departamentoDepartment catalogue with namesLookupraw_tiendasStore catalogue with type (A/B) and size in m²Lookupclean_ventasCleaned data with catalogue joins, standardised week, and department nameClean DataPivotDynamic tables with aggregated metrics by departmentPivot TablesDashboardInteractive widget to filter by department, showing KPIs, charts and visualisationsDashboardResumenSynthesis of findings, insights and business implicationsAnalytical Summary

  KPIs & Formulas
KPIDescriptionFormulaInterpretationSales per m²Sales adjusted by store sizeTotal Sales / Store SizeHigher values indicate greater efficiency per square metreParticipation %Each department's proportion of total 2012 salesDept Sales / Total SalesHigh values = greater contribution to total revenue

  Data Quality Checks
CheckFormulaResultStores without assigned department=CONTAR.SI(clean_ventas!I:I,"no tiene departamento")6,435Negative or null sales=COUNTIF(clean_ventas!D:D,"<0")27Store sizes with value 0=COUNTIF(raw_tiendas!C:C,0)+COUNTBLANK(raw_tiendas!C:C)954

  Tools & Skills Demonstrated

Google Sheets — data cleaning, VLOOKUP, pivot tables, dashboard creation
Excel-compatible formulas — COUNTIF, dynamic references, conditional formatting
Data wrangling and catalogue joins
KPI definition and business metrics design
Data quality validation (QA)
Dashboard and data visualisation


  Project Structure
walmart-sales-analysis/
│
├── Proyecto_2_Resumen_Ejecutivo_Ventas_Walmart.xlsx   # Full analysis file
└── README.md                                           # Project documentation

🎓 Context
This project was completed as part of the TripleTen Data Analytics Bootcamp (2026).

By Deborah Jara | Data Analyst | Mexico
