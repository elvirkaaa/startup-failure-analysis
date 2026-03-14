# startup-failure-analysis
Startup Graveyard: Data-Driven Analysis of Startup Failures

# Strategic Analysis of Startup Failures: A Multi-Methodology Research
**Author:** Aubakirova Elvira
**Framework:** Meredith’s Project Life Cycle & Pareto Efficiency
**Stack:** Python (Pandas/Seaborn), SQL (MySQL), Interactive Dashboard (HTML/JS)

---

## 1. Executive Summary
This project presents a hybrid analysis of startup failures, specifically within the technology and FinTech sectors. The research bridges the gap between raw data and management theory by integrating two distinct analytical layers:
1. **Quantitative Macro-Analysis:** Statistical evaluation of 47 companies to identify broader market trends.
2. **Qualitative Micro-Analysis (Deep-Dive):** A detailed "Post-mortem" study of 7 high-profile cases (e.g., Quibi, Atrium) categorized by **Jack Meredith’s Project Life Cycle** phases.

## 2. Methodology: Synthesis of Dual Datasets
The project utilizes two independent data sources to verify hypotheses and provide a 360-degree view of business collapse:
* **Dataset 1(General Market Statistics):** Used for Pareto Analysis in Python. This dataset highlights a wide array of operational failures.
* **Dataset 2 (Custom SQL Database):** A hand-curated database of major cases focused on investment volumes and strategic lifecycle phases.

## 3. Key Findings

### 3.1 Pareto Analysis: The "Long Tail" of Failure
Using Python (Pandas & Seaborn), I conducted a Pareto Analysis on 47 startups. 
* **The Insight:** Factors such as "Niche Limits" show a lower percentage impact in the larger dataset compared to deep-dive cases. 
* **Scientific Reasoning:** In a large sample size, failure causes are highly fragmented (a "Long Tail" of operational errors). However, in the deep-dive analysis of major ventures, fundamental strategic flaws (Initiation and Planning) emerge as the primary "killers."



### 3.2 Interactive Analytical Dashboard
An interactive HTML/JS dashboard was developed to visualize the correlation between funding amounts, lifespan, and primary failure reasons. 
* **Key Observation:** High-capital ventures (Quibi, Atrium) tend to collapse during the **Initiation** and **Planning** phases, while bootstrapped or low-funded projects (Sip) struggle more during the **Execution** phase.

## 4. SQL Database Insights (Meredith's Framework)
Data from `Quantitative Summary.csv` was processed through SQL to categorize failures into Meredith's strategic phases:

| Phase (Meredith) | Strategic Context | Risk Level | Notable Case |
| :--- | :--- | :--- | :--- |
| **Initiation** | Selection error / Lack of MVP | Critical (High Burn) | Quibi ($1.8B) |
| **Planning** | Business model / Strategy flaw | High (Fast Death) | Atrium / Sip |
| **Execution** | Technical debt / Poor product | Medium | ScaleFactor |
| **Control** | Competitive adaptation failure | Medium | HotelsAroundYou |
| **Termination** | Exit strategy (Integration) | Low (Success) | Musical.ly |

## 5. Conclusion
This research confirms Meredith’s theory: **the quality of project initiation and planning dictates survival more than the volume of available capital.** The presence of numerous minor causes in the general dataset emphasizes the need for operational control, while massive failures are almost always rooted in the violation of early-stage strategic phases.

## 6. Project Structure
* `/resources`: Contains `Quantitative Summary.csv` and raw data.
* `Code of analysis of 3rddataset.ipynb`: Python scripts for Pareto Analysis and data cleaning.
* `startup_graveyaed_dashboard_en.html`,`Аналитика на русском(дашборд).html` for interactive visualization.
* `README.md`: Project documentation and findings.

## 7. References & Data Sources

### Academic Frameworks
* **Meredith, J. R., & Mantel Jr, S. J. (2011).** *Project Management: A Managerial Approach*. Wiley. (Used for the Lifecycle Phase Categorization).
* **Ries, E. (2011).** *The Lean Startup*. Crown Business. (Used for the analysis of MVP failure in the Quibi and Sip cases).

### Primary Data Sources
1. **Dataset 1:** [https://www.kaggle.com/datasets/dagloxkankwanda/startup-failures](https://www.kaggle.com/datasets/dagloxkankwanda/startup-failures) 
2. **Dataset 2:** [https://www.kaggle.com/datasets/sakharebharat/startup-failure-prediction-dataset/data] 
3. **Dataset 3:** [https://deepdatalake.com/details.php?dataset_id=104]
4. **Dataset 4:** [https://www.failory.com/cemetery]


### Tools & Documentation
* **Pandas Documentation:** [pandas.pydata.org](https://pandas.pydata.org/docs/) — Methodology for data cleaning and Pareto computations.
* **Seaborn Statistical Data Visualization:** [seaborn.pydata.org](https://seaborn.pydata.org/) — Standards for categorical data representation.
* **MySQL 8.0 Reference Manual:** [dev.mysql.com/doc/](https://dev.mysql.com/doc/refman/8.0/en/) — Architecture for the relational failure database.
