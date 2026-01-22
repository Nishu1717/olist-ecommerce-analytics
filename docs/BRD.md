# Business Requirements Document (BRD)
**Project:** Brazilian E-Commerce Analysis
**Date:** 7th January 2026
**Author:** Nisarg Patel

## 1. Executive Overview
The objective of this project is to analyze the historical data of a Brazilian marketplace to optimize logistics performance and improve customer retention strategies. The insights derived will guide operational improvements and targeted marketing initiatives.

## 2. Business Objectives
-   **Improve Customer Satisfaction:** Identify key drivers of negative reviews to increase average CSAT scores.
-   **Optimize Logistics:** Determine the acceptable threshold for delivery delays before customer sentiment turns negative.
-   **Increase Retention:** Segment customers based on purchasing behavior to tailor re-engagement campaigns for "at-risk" and "hibernating" users.

## 3. Data Scope
The analysis encompasses 100k+ orders from 2016 to 2018, specifically utilizing the following datasets:
-   **Orders:** Timestamps, status, and delivery info.
-   **Customers:** Unique identifiers and location data.
-   **Reviews:** Customer sentiment scores (1-5).
-   **Payments:** Transaction values.
-   **Logistics:** Weight, dimensions, and seller info.

## 4. Functional Requirements
### 4.1 Data Processing
-   **Transformation:** All timestamps must be converted to datetime objects.
-   **Aggregation:** Master tables must be created by joining disparate datasets on key identifiers (`order_id`, `customer_id`, etc.).
-   **Cleaning:** Missing values in category translations must be handled ("unknown").

### 4.2 Analysis Modules
-   **Module A: RFM Segmentation**
    -   Calculate Recency, Frequency, and Monetary scores.
    -   Classify customers into standard segments (e.g., Champions, Hibernating).
-   **Module B: Logistics Impact**
    -   Calculate `delivery_delay` (Actual Delivery Date - Estimated Delivery Date).
    -   Correlate delay with review scores to find the "Disappointment Cliff".

## 5. Key Deliverables
1.  **Cleaned Data Pipeline:** Notebook code for reproducible data processing.
2.  **Executive Dashboard:** Visualizations of Customer Segments and Delivery Impact.
3.  **Strategic Recommendations:** Actionable insights based on the analysis.

## 6. Success Metrics
-   Identification of at least 3 distinct customer segments.
-   Determination of the exact day-count delay that drops average review scores below 3.0.
