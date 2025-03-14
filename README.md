# TMP2-Recommendation-system-project

## Project Overview

This project aims to develop a recommendation system that provides personalized suggestions based on user behavior and preferences. The system analyzes past interactions and item properties to predict future user engagement and improve decision-making.

### Analytical Questions

#### The following key analytical questions were explored:

**1.User Interaction Patterns**: How do users interact with different product categories?
** 2.Predictive Features**: What features contribute most to predicting user engagement (e.g., add-to-cart events)?
** 3. Recommendation Optimization**: How can we improve recommendation accuracy using different models?
**4. Performance Trade-offs**: What are the trade-offs between model complexity and computational efficiency?
**5. Real-Time Applicability**: Can the system be deployed for real-time recommendations?

## Dataset Description
The project leverages three datasets:
1. Events Data (events.csv): Contains ~2.75 million user interactions, capturing actions such as 'view', 'addtocart', and 'transaction'.

2. Item Properties (item_properties.csv): Contains weekly snapshots of ~417,000 products with associated attributes.

3. Category Tree (category_tree.csv): Defines hierarchical relationships across 1,669 item categories.

## Methodology
* Data Preprocessing & Feature Engineering
* Merging Data: Combined event logs with item properties using merge_asof on timestamps.
* Feature Engineering: Created user interaction profiles and extracted key predictive features.
* Handling Missing Data: Addressed null values using forward/backward filling techniques.
* Model Development & Evaluation
* Model Selection: Implemented a Random Forest classifier to predict user engagement.

## Optimization Strategies:
* Reduced memory load by optimizing tree depth and reducing dataset dimensionality.
* Fine-tuned hyperparameters to enhance model accuracy.

### Evaluation Metrics:
* Achieved an accuracy of ~58-60%, demonstrating moderate predictive power.
* Precision and recall trade-offs were analyzed for performance insights.

## Key Insights

* User Engagement is Predictable: Historical behavior significantly influences recommendation accuracy.

* Feature Selection Matters: Limiting features to the most relevant ones improves efficiency without major accuracy loss.

* Hybrid Models Enhance Performance: Combining collaborative filtering with content-based methods improves recommendations.

## Deployment Considerations
* Investigated integration options for API-based recommendation deployment.
* Considered real-time processing capabilities for enhanced user experience.

## Getting Started
* Prerequisites

1. Python 3.x

2. Pandas, NumPy, Scikit-learn, Matplotlib

3. Jupyter Notebook (recommended for exploration)

## Installation
**Clone the repository:**
git clone https://github.com/akuakorkor/TMP2-Recommendation-system-project.git

**Install dependencies:** 
1. pip install -r requirements.txt
2. Run the preprocessing script:
3. python preprocess.py

**Train the model:**
hybrid_model.pkl

## Conclusion

This project highlights the importance of data preprocessing, feature engineering, and model optimization in building effective recommendation systems. Future iterations will focus on improving accuracy and integrating real-time recommendation capabilities.