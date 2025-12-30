# SpaceX-Falcon-9-Landing-Prediction-Cost-Analysis
A comprehensive Data Science pipeline predicting SpaceX Falcon 9 landing success using API/Web Scraping, SQL, Folium, and Plotly Dash. Features 4 optimized Machine Learning models with 83.3% predictive accuracy. 🚀🐍📊

## 📌 Executive Summary
The goal of this project is to predict the success of SpaceX Falcon 9 first-stage landings. SpaceX offers launches for **$62 million**, significantly cheaper than competitors ($165M+), primarily because they reuse the first stage. This project uses machine learning to predict landing outcomes, providing a strategic edge for competitors to estimate launch costs.

## 🛠️ Tech Stack & Methodologies
- **Data Collection:** `Requests` (API), `BeautifulSoup` (Web Scraping).
- **Data Wrangling:** `Pandas`, `NumPy` (One-Hot Encoding, missing value handling).
- **Exploratory Data Analysis (EDA):** `SQL` (queries for payload and site analysis), `Seaborn`, `Matplotlib`.
- **Interactive Visuals:** `Folium` (Geospatial Mapping), `Plotly Dash` (Interactive Dashboards).
- **Machine Learning:** `Scikit-Learn` (Logistic Regression, SVM, Decision Trees, KNN).

## 📊 Key Insights from Analysis
- **Success Trends:** Landing success rates have increased over time, particularly with the introduction of the "Block 5" booster.
- **Payload Impact:** Missions with payload masses between **2,000kg and 4,000kg** have the highest success rates.
- **Geospatial Strategy:** All launch sites are located near coastlines to facilitate safe landings on Drone Ships or return-to-launch-site maneuvers.



## 🤖 Machine Learning Results
All models were tuned using `GridSearchCV` and evaluated on a test set.

| Model | Test Accuracy | Best Hyperparameters |
| :--- | :--- | :--- |
| **Logistic Regression** | 83.33% | C=0.01, Penalty=l2 |
| **SVM** | 83.33% | Kernel=Sigmoid, C=1.0 |
| **Decision Tree** | 83.33% | max_depth=6, criterion='gini' |
| **KNN** | 83.33% | n_neighbors=10, p=2 |

**Conclusion:** All models reached an accuracy ceiling of 83.33% due to the small test set size. However, the models are highly robust for predicting future landing outcomes based on mission parameters.



## 🚀 How to Run the Project
1. Clone the repository: `git clone https://github.com/your-username/spacex-landing-prediction.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Run the Dash App: `python scripts/app.py`

## 🤝 Contact
Author: Devprakash Rai
LinkedIn: www.linkedin.com/in/devprakash-rai-8608b5208
