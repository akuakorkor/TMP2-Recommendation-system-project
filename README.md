# TMP2-Recommendation-system-project

## Overview
This project aims to develop a robust recommendation system for an e-commerce platform by leveraging historical user behavior data and dynamic item properties. The system will provide personalized product recommendations, content suggestions, and service optimizations to enhance user engagement, conversion rates, and customer satisfaction.

## Hypotheses
- **Personalization Impact:** Utilizing historical user interactions and dynamic item properties to drive personalized recommendations will lead to improved engagement, higher conversion rates, and enhanced customer satisfaction.
- **Data Quality Impact:** Removing or filtering abnormal user behavior (noise) from the dataset will significantly improve the recommendation system’s accuracy and effectiveness.

## Analytical Business Questions
1. **User Interaction Predictiveness:** Which types of user interactions (e.g., product views, add-to-cart events, transactions) are most predictive of a purchase decision, and how can these be weighted in the recommendation system?
2. **Category Performance:** How do different product categories perform in terms of user engagement and conversion rates, and does personalization within categories lead to improved sales?
3. **Abnormal User Impact:** What is the effect of abnormal or noisy user behavior on the performance of the recommendation system, and how does filtering these users change key performance metrics?
4. **Temporal Dynamics:** How do recency and frequency of user interactions correlate with conversion rates?
5. **Influence of Item Properties:** Which dynamic item properties (e.g., price changes, vendor information) most significantly impact the accuracy of recommendations, and how can these be effectively integrated into the model?
6. **Customer Retention:** How does the introduction of personalized recommendations affect customer retention and repeat purchase behavior over time?
7. **Revenue Generation:** What is the overall impact of the recommendation system on sales revenue, and which aspects contribute most to incremental revenue gains?

## Data Description
The project utilizes three primary datasets:
- **Events Data:** Contains user interaction logs (views, add-to-cart, transactions) along with timestamps.
- **Item Properties:** Provides time-dependent snapshots of various item attributes (e.g., price, category), stored as a change log where consecutive, unchanged snapshots are merged.
- **Category Tree:** Represents the hierarchical relationships between product categories, which can be used to contextualize recommendations based on category information.

## Project Structure