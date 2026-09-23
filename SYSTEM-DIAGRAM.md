# Inventory demo: simplified data flow

This diagram documents the new portfolio prototype. It is a simplified illustration of the course project's analysis methods, not a reproduction of the original graded diagrams.

## Context

```mermaid
flowchart LR
  Staff[Store staff] -->|Product, sale, restock inputs| Demo[Inventory demo]
  Demo -->|Stock, alerts, profit, CSV| Staff
  Demo <--> Store[(Browser localStorage)]
```

## Level 1 flow

```mermaid
flowchart TD
  Staff[Store staff] --> Entry[1. Validate input]
  Entry --> Products[2. Update products and stock]
  Entry --> Sales[3. Record sale and profit]
  Products <--> Data[(Browser localStorage)]
  Sales <--> Data
  Data --> Report[4. Display status and export]
  Report --> Staff
```

**Boundary:** Only one browser is represented. A future cloud system would need shared storage, accounts, backups, access controls and synchronization across devices.
