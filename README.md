# Online-Shoppers-Purchase-Intention-Predictive-Analytics


## Project Overview
In the competitive e-commerce landscape, understanding visitor behavior is key to maximizing conversion rates. This project aims to predict whether a website visitor will complete a purchase based on their session behavior, such as page visits, duration, and bounce rates. By leveraging machine learning, businesses can target high-intent users more effectively and optimize marketing strategies.

## Live Demo
The model is deployed and can be accessed interactively here:
**[View App on Hugging Face Spaces](https://huggingface.co/spaces/nandutt/shopper-intent-prediction)** 

## Objectives
* **Identify Key Drivers:** Analyze which session attributes (e.g., Page Values, Exit Rates) most influence a visitor's decision to buy.
* **Predictive Modeling:** Build and optimize a classification model to forecast purchase intention with high precision and recall.
* **Inference Pipeline:** Develop a ready-to-use pipeline for real-time predictions on new visitor data.

## Tech Stack
* **Programming Language:** Python
* **Libraries:** Pandas, NumPy, Scikit-Learn, Joblib
* **Machine Learning:** Random Forest Classifier (Optimized via Grid Search/Random Search)
* **Deployment:** Hugging Face Spaces & Streamlit

## Dataset Description
The dataset consists of feature vectors belonging to 12,330 sessions.
* **Numerical features:** Administrative, Informational, and Product Related page visits, session durations, Bounce Rates, Exit Rates, and Page Values.
* **Categorical features:** Operating Systems, Browser, Region, Traffic Type, Visitor Type, Weekend, and Month.
* **Target Label:** `Revenue` (True if a purchase was made, False otherwise).

## Key Results & Insights
* **Feature Importance:** `PageValue` was identified as the most significant predictor, showing that users who visit high-value pages are exponentially more likely to convert.
* **Model Performance:** The final model was optimized to achieve a strong balance between Precision and Recall, ensuring that potential buyers are identified while minimizing false positives.
* **Ready for Inference:** The project includes a pre-trained model pipeline (`.pkl`) used for both the local inference and the live web app.
* **Robust Prediction:** Leveraged the power of Random Forest to handle non-linear relationships and provide stable predictions across diverse visitor sessions.

## Repository Structure
```text
├── Predictive_Analytics_for_E_commerce.ipynb  # Full EDA, Preprocessing, & Training
├── Inference.ipynb                             # Script for real-time model testing
├── optimized_ecommerce_model.pkl              # Saved trained model pipeline
└── README.md                                   # Project documentation
