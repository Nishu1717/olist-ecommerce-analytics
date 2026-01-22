# Brazilian E-Commerce Analytics Project

## Executive Summary
This project delivers a comprehensive analysis of the Brazilian E-Commerce landscape, focusing on customer behavior and logistics performance. By leveraging a robust dataset of 100k+ orders, we have identified key drivers of customer satisfaction and actionable segments for marketing optimization.

## Dataset
The dataset used in this project is the Brazilian E-Commerce Public Dataset by Olist.
You can download it here: [Olist Dataset - Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

### Key Insights
1.  **The "Disappointment Cliff"**: Our analysis reveals a critical threshold in delivery delays. Customer satisfaction plummets (average review score < 3.0) once a package is more than **3 days late**. This insight provides a tangible SLA target for logistics partners.
2.  **Customer Segmentation**: Using RFM (Recency, Frequency, Monetary) analysis, we categorized the customer base. A significant portion falls into the "Hibernating" segment, indicating a need for aggressive re-engagement campaigns. Conversely, "Champions" are highly valuable but scarce, suggesting a focus on retention is paramount.

## Project Structure
```
/E-Commerce
├── /data/                  # Raw datasets 
├── /notebooks/             # Jupyter Notebooks for detailed analysis
│   └── E_Commerce_Analysis.ipynb
├── /visualizations/        # Exported charts and figures
├── /docs/                  # Business Requirements and documentation
│   └── BRD.md
└── requirements.txt        # Python dependencies
```

## Getting Started
1.  Install dependencies
    ```bash
    pip install -r requirements.txt
    ```
2.  Run the analysis
    - Launch Jupyter Notebook: `jupyter notebook notebooks/E_Commerce_Analysis.ipynb`

## Technologies Used
-   **Python**: Primary language
-   **Pandas & NumPy**: Data manipulation
-   **Matplotlib & Seaborn**: Data visualization
-   **Jupyter**: Interactive analysis environment

---
*Author: Nisarg Patel*
*Date: 10th January 2026*
