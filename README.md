# Databases-Analytics-Assignment

# NorthStar Urban Mobility and Logistics - Analytics & Database Solution

## Overview
This repository contains the complete analytical workflow and NoSQL database design for the **NorthStar Urban Mobility and Logistics** case study. The project investigates operational inefficiencies, financial leakages, and service reliability issues using a combination of relational data extraction, statistical visualization, and document-based NoSQL architecture.

## Technologies Used
* **SQL (via R `sqldf`):** Used for relational data extraction and metric calculation across operational silos.
* **R (`ggplot2`):** Used for statistical visualizations of hub performance and financial profitability.
* **Python (`pandas`, `matplotlib`, `seaborn`):** Used for data processing, merging asset data with incident logs, and visualizing vehicle health trends.
* **MongoDB Atlas (`pymongo`):** Used to design and deploy an optimized, nested NoSQL database for a unified "Customer Journey" view.

## Key Analytical Findings
1. **Service Reliability:** Identified specific route overrides and delivery window breaches contributing to customer dissatisfaction.
2. **Financial Leakage:** Calculated gross profit margins to isolate unprofitable service types.
3. **Hub Inefficiency:** Highlighted specific city hubs responsible for the highest volume of manual route overrides.
4. **Asset Maintenance:** Proved via Python data processing that current predictive maintenance metrics fail to correlate with critical vehicle incidents.

## Database Architecture
The project successfully bridges the gap between structured legacy systems and semi-structured platform data. A new MongoDB collection (`CustomerJourneys`) was built and optimized with indexing to nest `orders`, `app_events`, and `complaints` into highly scalable, single-document views.

## Execution
All code is contained within a master Google Colab notebook, designed to run sequentially from data ingestion to cloud database deployment.
