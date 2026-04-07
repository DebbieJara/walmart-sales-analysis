Walmart Sales Executive Summary — Google Sheets Analysis
The Business Problem
Walmart operates hundreds of departments across stores of different sizes. But which departments are actually driving revenue? And which ones are occupying valuable floor space without delivering proportional results?
This analysis was built to answer exactly that.
What I Did
I took Walmart's 2012 weekly sales data and built a full analytical pipeline in Google Sheets — from raw data to executive dashboard. I cleaned the data, joined department and store catalogues, validated data quality, defined KPIs, and built an interactive dashboard that makes the findings immediately actionable.
What the Data Revealed
Two metrics told the real story:

Participation % showed which departments contributed most to total revenue — helping prioritize commercial strategy
Sales per m² exposed which departments were truly efficient versus those that looked strong on paper but underperformed relative to their store footprint

Data quality checks surfaced 6,435 records without assigned departments, 27 negative sales values, and 954 stores with missing size data — all handled before any analysis was run.
Technical Details
File Structure
SheetDescriptionTyperaw_ventasOriginal weekly sales data by store and departmentRaw Dataraw_departamentoDepartment catalogue with namesLookupraw_tiendasStore catalogue with type (A/B) and size in m²Lookupclean_ventasCleaned data with catalogue joins, standardised week, and department nameClean DataPivotDynamic tables with aggregated metrics by departmentPivot TablesDashboardInteractive widget to filter by department, showing KPIs, charts and visualisationsDashboardResumenSynthesis of findings, insights and business implicationsAnalytical Summary
KPIs & Formulas
KPIDescriptionFormulaInterpretationSales per m²Sales adjusted by store sizeTotal Sales / Store SizeHigher values indicate greater efficiency per square metreParticipation %Each department's proportion of total 2012 salesDept Sales / Total SalesHigh values = greater contribution to total revenue
Data Quality Checks
CheckFormulaResultStores without assigned department=CONTAR.SI(clean_ventas!I:I,"no tiene departamento")6,435Negative or null sales=COUNTIF(clean_ventas!D:D,"<0")27Store sizes with value 0=COUNTIF(raw_tiendas!C:C,0)+COUNTBLANK(raw_tiendas!C:C)954
Tools & Skills Demonstrated
SQL (PostgreSQL) · Google Sheets · VLOOKUP · Pivot Tables · COUNTIF · Dashboard Design · Data Quality Validation
Project Structure
walmart-sales-analysis/
│
├── Proyecto_2_Resumen_Ejecutivo_Ventas_Walmart.xlsx   # Full analysis file
└── README.md                                           # Project documentation

By Deborah Jara | Data Analyst | México
LinkedIn · GitHub
