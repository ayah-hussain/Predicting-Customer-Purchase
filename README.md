# Customer Purchase Prediction Project

## Project Overview
This project applies data mining and machine learning techniques to predict customer purchases within a 4-week period. As e-commerce grows, personalized experiences are crucial for customer retention. Our goal is to utilize historical transaction data to build a predictive model that can anticipate when customers need to replenish essential household items (such as personal care products, cleaning supplies, and pet food).

The system aims to predict:
1. Whether a customer will repurchase a product.
2. The specific week the replenishment is likely to occur.

This approach is designed to enhance customer satisfaction by enabling timely recommendations and optimizing inventory management.

## Team Members
* **Ayah A M Hussein** (150220917)
* **Ömer Erdağ** (150210332)

*Department of AI & Data Engineering, ITU*

## Dataset
The project utilizes a dataset containing historical transaction data of individual customer purchases and product-specific information.

> **Note:** The dataset used for this project was provided by the course instructor specifically for this coursework. As per course policy, the data is private and cannot be shared or included in this repository.

## Methodology
We propose evaluating several candidate models to handle the specific challenges of the dataset, such as high-cardinality categorical features and temporal dependencies.

### Proposed Models
* **XGBoost:** Selected for its ability to handle structured data and capture non-linear interactions between customer and product details. Its regularization capabilities help mitigate overfitting.
* **CatBoost:** Chosen specifically for its native handling of high-cardinality categorical variables (e.g., product groups, manufacturers) without extensive preprocessing or information loss.
* **LightGBM:** Utilized for its efficiency with large transactional datasets. Its leaf-wise tree growth strategy offers faster training and lower memory usage while capturing complex interactions.
* **LSTM (Long Short-Term Memory):** Employed to model the temporal aspects of the data. LSTM networks are well-suited for capturing long-term dependencies in customer purchasing frequency to predict the specific timing of repurchases.

## Evaluation Strategy
Models will be trained on features including User ID, Product ID, Category, and Repurchase Time. The best-performing model will be selected based on a comprehensive assessment of the following metrics:
* **F1 Score:** Prioritized to balance precision and recall.
* **Accuracy**
* **Precision & Recall**
* **AUC-ROC:** To measure the model's ability to differentiate between classes effectively.

## Repository Structure
* `/src`: Source code for data processing and model training.
* `/notebooks`: Jupyter notebooks for exploratory data analysis (EDA).
* `/docs`: Project documentation and reports.
