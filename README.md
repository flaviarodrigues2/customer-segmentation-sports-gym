# Customer Segmentation on a Sports Facility (Data Mining)

Academic project (Master’s in Data Science and Advanced Analytics) focused on **customer segmentation** in a gym/health club, based on data provided by the company’s ERP system (2014-06-01 to 2019-10-31). We applied several **clustering approaches** to obtain complementary perspectives: value/demographics (K-Means, Hierarchical K-Means, SOM+K-Means) and activity preferences (K-Modes), with **DBSCAN** for noise removal.

> This repository contains **reproducible code** and the structure to place the data locally. The original dataset is **not** public and therefore not included.

## 🔍 Objective
Segment customers to support decisions in **marketing**, **retention**, and **service allocation** (programs, pricing, promotions, positioning).

## 🧱 Methodology (summary)
- **EDA & Preprocessing**: consistency checks, missing value and outlier handling, *feature engineering* (tenure, `UsageRate`, monthly RFM), *scaling*, and *one-hot encoding*.  
- **DBSCAN**: mainly used for **noise/outlier detection** prior to other models.  
- **K-Means / Hierarchical K-Means / SOM+K-Means** (demographic/value perspective).  
- **K-Modes** (preference perspective).  
- **Merging perspectives**: *post-clustering* with agglomerative to combine K-Means and K-Modes labels; useful but with some **overlap** (documented limitation).  

## 📈 Key Insights (high-level)
- Segments with **high value but high risk** (good usage/monetary but poor recency) → **retention priority**.  
- **New/recently joined** segments with low frequency → need **onboarding** and usage nudges.  
- **Activity preferences** differ across clusters (e.g., water vs. team sports; gender differences).  

---

> Original academic work by Catarina Rodrigues, Flávia Rodrigues, and Sophia Ramos (Group 52).  
