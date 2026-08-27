## Retail Sales & Cost Analysis Dashboard

A two-page Power BI dashboard built to analyze retail sales performance, cost drivers, and target achievement across a chain of stores. This project was completed as part of the CFI Power BI Fundamentals training, focused on dashboard user experience and interactivity.

## Overview

The dashboard tracks sales, gross margin, and year-to-date performance for a retail business, then lets a user drill into cost and staffing detail for individual stores. It is built around two connected pages rather than a single flat view, so the experience moves from a high-level summary down to store-level detail.

## Dashboard Pages

### Sales

* KPI cards for Total Sales, Total Sales YTD, and Total Gross Margin
* A map visual plotting sales by store location, colored by store type
* A clustered column chart breaking down sales by department and store type
* A ribbon chart showing how department rank shifts by store location over time
* Slicers for date, department, and store type, with cross-filtering enabled between the map and the other visuals

### Cost & Target

* A drillthrough page reached from the Sales page, filtered to the selected store type
* A table comparing total sales, total wages, and the difference from target by store location
* A scatter chart comparing store size in square feet against total rent, split by store type, to visualize cost efficiency across the store fleet
* A KPI visual tracking total sales against target over time
* Navigation buttons to move between report views

## Data Model

The report is built on a star-style model with the following tables:

* Retail Sales, containing the Total Sales and Total Sales YTD measures
* Retail Cost, containing Total Gross Margin, Total Wages, Total Rent, Store Size, Total Target, and Difference From Target measures
* Store Details, with store location, store type, and store ID
* Categories, with department information
* Date, used for time intelligence and filtering across both pages

## Skills Demonstrated
* DAX measure design, including a year-to-date calculation and a variance measure comparing actuals to target
* Dashboard information architecture, using a summary page paired with a drillthrough detail page instead of a single crowded canvas
* Cross-filtering and slicer configuration to make the report interactive rather than static
* Selection of chart types matched to the question being asked, including a ribbon chart for rank over time and a scatter chart for cost efficiency
* Data modelling across multiple related tables

## Tools

Power BI Desktop, DAX, Power Query

## Notes

This repository contains the .pbix file for the dashboard.
