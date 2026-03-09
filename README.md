# Customer Segmentation on a Sports Facility (Data Mining)

Project focused on customer segmentation in a gym/health club, based on data provided by the company’s ERP system (2014-06-01 to 2019-10-31). We applied several clustering approaches to obtain complementary perspectives: value/demographics (K-Means, Hierarchical K-Means, SOM+K-Means) and activity preferences (K-Modes), with DBSCAN for noise removal.

## Objective
Segment customers to support decisions in marketing, retention, and service allocation (programs, pricing, promotions, positioning).

## Methodology 
- EDA & Preprocessing: consistency checks, missing value and outlier handling, feature engineering (tenure, `UsageRate`, monthly RFM), scaling, and one-hot encoding.
- DBSCAN: mainly used for noise/outlier detection prior to other models.  
- K-Means / Hierarchical K-Means / SOM+K-Means (demographic/value perspective).  
- K-Modes (preference perspective).  
- Merging perspectives: post-clustering with agglomerative to combine K-Means and K-Modes labels.  

## Key Insights 
- Segments with high value but high risk (good usage/monetary but poor recency) → retention priority.  
- New/recently joined segments with low frequency → need onboarding and usage nudges.  
- Activity preferences differ across clusters (e.g., water vs. team sports; gender differences).  
