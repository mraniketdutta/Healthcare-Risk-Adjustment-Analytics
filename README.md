# Healthcare Claims Revenue Cycle Dashboard — Power BI

An interactive Power BI dashboard analyzing health insurance claims data to surface 
key Revenue Cycle Management (RCM) KPIs — claim volume, approval/denial rates, and 
reimbursement amounts — enabling data-driven decisions on billing performance and 
claims processing efficiency.

## Overview

This dashboard ingests raw health insurance claims data and transforms it into a 
single-page executive view covering claim status distribution, financial exposure, 
and provider-specialty performance. Built to simulate a real-world RCM analytics 
use case: tracking claims from submission through approval, denial, or pending 
resolution.

## Key Features

- **KPI Cards** — Total Claims, Approved Claims, Rejected Claims, Pending Claims
- **Financial Tracking** — Total Amount Submitted, Paid, Denied, and Pending
- **Rate KPIs with Targets** — Approval Rate % and Denial Rate % benchmarked 
  against industry targets (90% approval / <5% denial), with year-over-year trend lines
- **Provider Specialty Breakdown** — Clustered column chart comparing approval 
  and denial rates across provider specialties to identify outlier departments
- **Dynamic Filtering** — Slicer panel for Year, Claim Status, Submission Method, 
  and Claim Type

## DAX Measures

Custom measures built for this model include:
- `Total Claims`, `Approved Claims`, `Rejected Claims`, `Pending Claims`
- `Total Amount Submitted`, `Total Amount Paid`, `Total Amount Denied`, `Total Amount Pending`
- `Approval Rate %`, `Denial Rate %` (using `DIVIDE()` for safe handling of zero-claim filter contexts)
- Target benchmarks for approval and denial rate goal-tracking

## Tools & Techniques

- **Power BI Desktop** — report design, DAX measure authoring, data modeling
- **Power Query** — data shaping and transformation
- **SQL** — querying and structuring source claims tables prior to modeling
- **Data Modeling** — relationship design between claims, provider, and date dimensions

## Dataset

Built on a synthetic health insurance claims dataset (~4,500 records) covering 
claim status, provider specialty, submission method, claim type, and claim amount 
fields — structured to mirror real-world payer/provider claims data.

## Skills Demonstrated

Revenue Cycle Management (RCM) analytics · Healthcare claims data modeling · 
DAX measure design · KPI benchmarking · Denial/approval rate analysis · 
Dashboard UX for healthcare stakeholders
