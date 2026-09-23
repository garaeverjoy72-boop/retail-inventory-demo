# Retail Inventory Management: systems analysis and working demo

**Everjoy Gara | Portfolio case study**

This repository presents a new, small browser prototype inspired by my completed IBM Systems Analyst final project, *Optimize the Inventory Management System for a Small Retail Store*. The original course case concerned an eco-friendly retailer using spreadsheets. This prototype was created afterward to demonstrate how some of the proposed requirements could work. It is not the original graded submission or a production system. All sample products and figures are fictional.

## Problem and goal

Manual spreadsheets made stock updates time-consuming and increased the risk of stockouts and overstocking. The goal was to define a simple, affordable future-state inventory process that staff with limited IT experience could use.

## My analysis work

- Identified stakeholders, scope, assumptions and constraints.
- Compared the spreadsheet process with a future state using gap analysis.
- Defined functional and non-functional requirements.
- Modelled current and proposed data flows with context diagrams and Level 1 DFDs in draw.io for the course project.
- Recommended a cloud-based solution for the case study, with stock visibility, sales updates and reorder alerts.

## New portfolio prototype

Open [`index.html`](index.html) in a browser, or publish this repository with GitHub Pages. The demo lets a user add products, record sales, restock one unit, see reorder alerts and export inventory to CSV. It calculates gross profit on sales as `(selling price - unit cost) × units sold`.

The demo uses `localStorage`: information stays in the current browser. It has no authentication, shared database, cloud sync or supplier integration. These would be later requirements for a real store.

## Requirements traced to the demo

| Need | Demonstrated behavior |
| --- | --- |
| Know current stock | Inventory table and stock summary |
| Avoid selling unavailable units | Sale is rejected when requested units exceed stock |
| Spot reorder needs | Alert when stock is at or below each product's threshold |
| Record product and sales data | Add product and record sale forms |
| Share inventory snapshot | CSV export |
| Work on a phone | Responsive layout |

## Data flow

See [SYSTEM-DIAGRAM.md](SYSTEM-DIAGRAM.md) for a simplified context and Level 1 flow. The diagram describes the new demo, not a copy of the original course submission.

## How to test

1. Open `index.html` and note the three fictional products.
2. Sell one Bamboo Toothbrush. Its stock changes from 4 to 3, and gross profit increases by R17.
3. Try to sell more units than remain. The sale is rejected.
4. Add a product with a unique SKU, then export the CSV.
5. Use **Reset sample data** when you want to start over.

## Skills shown

Systems analysis, requirements traceability, process modelling, inventory logic, HTML, CSS, JavaScript, browser storage, form validation and CSV export.
