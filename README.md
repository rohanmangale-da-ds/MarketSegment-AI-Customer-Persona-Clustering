# MarketSegment-AI: Customer Persona Clustering

## 📌 Project Overview
**MarketSegment-AI** is an unsupervised machine learning project aimed at segmenting customers into distinct groups based on their demographic information, historical purchasing behavior, and interactions with marketing campaigns. By clustering customers, businesses can gain actionable insights to tailor personalized marketing strategies, maximize customer retention, and optimize marketing spend.

The project utilizes data processing techniques like **Principal Component Analysis (PCA)** for dimensionality reduction and **K-Means Clustering** to identify clear, actionable customer personas.

## 🎯 Objectives
- Perform Data Cleaning and Preprocessing on marketing campaign data.
- Handle missing values and process date-time variables effectively.
- Apply PCA to reduce dimensions and visualize high-dimensional data efficiently.
- Use the Elbow Method to determine the optimal number of clusters.
- Apply K-Means clustering algorithm to categorize customers into distinct segments.
- Provide descriptive insights based on the clustered groups.

## 🗂 Dataset
The dataset used is `marketing_campaign.csv`, which includes various features related to customer demographics, buying behaviors, and responses to campaigns, such as:
- **Demographics:** Year of Birth, Education, Marital Status, Income, Number of Kids/Teens at home.
- **Spending Behavior:** Amount spent on Wines, Fruits, Meat, Fish, Sweet, and Gold products.
- **Engagement:** Web visits, Purchases through deals, web, catalog, and physical stores.
- **Campaign Response:** Acceptance of marketing campaigns 1 through 5, and overall responsiveness.

## 🛠 Technology Stack
- **Python** (Core programming language)
- **Pandas & NumPy** (Data Manipulation and processing)
- **Matplotlib & Seaborn** (Data Visualization)
- **Scikit-Learn** (Machine Learning, PCA, K-Means, Preprocessing)
- **Yellowbrick** (Clustering Evaluation - KElbowVisualizer)
- **Jupyter Notebook** (Interactive Development environment)

## ⚙️ Methodology
1. **Data Preprocessing:**
   - Dropped missing values (e.g., in the `Income` column).
   - Parsed date columns into proper DateTime formats (e.g., `Dt_Customer`).
   - Standardized features and encoded categorical variables appropriately for machine learning models.
2. **Dimensionality Reduction:** 
   - Applied **PCA (Principal Component Analysis)** to reduce data complexity, eliminate noise, and prepare the dataset for efficient clustering.
3. **Clustering Analysis:**
   - Leveraged the **Elbow Method** (using Yellowbrick's `KElbowVisualizer`) to determine the optimal number of clusters (`k`).
   - Built the **K-Means** clustering model to map the customers into distinct persona segments.
4. **Evaluation:** 
   - Evaluated cluster distinctiveness visually and extracted cluster profiles for business interpretation.

## 🚀 How to Run
1. Ensure you have Python installed.
2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn yellowbrick
   ```
3. Check and update the dataset path in the notebook if needed.
4. Run the Jupyter Notebook.

## 📈 Potential Future Enhancements
- Experimenting with advanced clustering algorithms (e.g., DBSCAN, Agglomerative Hierarchical Clustering) to compare and contrast segmentations.
- Building an interactive dashboard (e.g., using Streamlit or Dash) for stakeholders to dynamically view and filter customer personas.
- Integrating a classification model to predict which segment a *new* customer will fall into based on their initial profile.

