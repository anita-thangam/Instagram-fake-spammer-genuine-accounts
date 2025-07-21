**Instagram Fake, Spammer & Genuine Account Detection**

**Description:**
An end-to-end Machine Learning & Data Analysis project to detect fake/spammer Instagram accounts using profile features and behavioral metrics. 
Includes SQL-based EDA, visual analytics (power BI), and ML models (Random Forest, Decision Tree) with evaluation metrics.

**Project Overview**

Social media platforms like Instagram are plagued by fake and spammer accounts. This project aims to detect such accounts using Machine Learning, Data Analysis, SQL-based EDA, and Visualization tools.
We utilize a labeled dataset containing features like profile picture presence, follower/following counts, username patterns, and more to classify accounts as **Fake (1)** or **Genuine (0)**. The objective is to build a reliable classification model and explore impactful visual insights.

**Problem Statement**

> Detect and classify Instagram accounts as **fake/spammer** or **genuine** using account metadata and user behavior.

**Tools & Technologies**B

- **Python** (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn)
- **SQL** (PostgreSQL-style EDA)
- **Power BI** (Visualization)
- **Excel** (Preprocessing)
- **Colab google**

**Features:**
- `profile_pic`, `description length`, `#followers`, `#follows`, `#posts`, `username_length`, etc.
- `fake`: Target label (1 = fake, 0 = genuine)


**Workflow**

### 1. Data Preprocessing
- Handled missing values (none found)
- Scaled numerical features
- Created derived features like `followers/following` ratio

### 2. Exploratory Data Analysis (EDA)
- Distribution of fake vs genuine accounts
- Correlation heatmaps
- Feature impact: profile picture, followers, description length, etc.
- Visual patterns using Seaborn & Matplotlib

### 3. Model Building
- **Random Forest Classifier**
- **Decision Tree Classifier**

### 4. Model Evaluation
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix Visualization
- Feature importance bar charts

### 5. SQL-Based Analysis (EDA)
- Schema Design using `instagram_accounts` table
- Queries to analyze:
  - Profile picture distribution
  - Follower-following ratio
  - Username & fullname patterns
  - Private vs public account trends

### 6. Power BI Dashboard
- Visualizations for fake/genuine profiles
- Follower patterns & activity metrics
- Account privacy insights

**Results**

- **Decision Tree Accuracy:** 87%
- **Random Forest Accuracy:** 94%
- <img width="681" height="257" alt="image" src="https://github.com/user-attachments/assets/70298e32-f0f7-437d-acbd-2dbe7b425986" />

- Most Important Features:
  - `profile_pic`, `#followers`, `description length`, `#follows`, `private`

** Future Improvements**

- Add more diverse data (recent datasets)
- Use XGBoost / LightGBM for improved classification
- Tune models via GridSearchCV
- Address class imbalance with SMOTE
