# 🎥 Data-Driven Decision Making for SussexBudgetProductions

## Objective
Leveraged data-driven approaches to assist SussexBudgetProductions in making informed decisions regarding movie production investments by analyzing the IMDB Movie Dataset.

---

## 📊 Dataset Overview
- **Source**: [IMDB Movie Dataset]
- **Attributes**:
  - Movie genres, budgets, revenues, and IMDB ratings.
  - Director, actors, and production details.
- **Focus**: Identifying relationships between various factors and their impact on movie profitability.

---

## 🧹 Data Cleaning Process
1. **Inspect Null Values**:
   - Identified columns with a high percentage of missing data.
   - Rounded proportions to two decimal places for precision.

2. **Remove Unnecessary Columns**:
   - Excluded irrelevant fields, such as:
     - `color`, `director_facebook_likes`, `cast_total_facebook_likes`, etc.

3. **Handle Missing Values**:
   - Replaced missing values in categorical fields (e.g., language) with logical defaults (e.g., "English").
   - Dropped rows with significant missing data.

4. **Verify Rows Retained**:
   - Ensured sufficient data retention after cleaning.

---

## 🔍 Exploratory Data Analysis (EDA)
1. Conducted visualizations to explore relationships:
   - **Budget vs. Profit**: Observed no direct correlation.
   - **Profit vs. Gross Revenue**: Found a positive correlation.
   - Identified outliers and their potential impact on results.

2. Visual Highlights:
   - Scatterplot of Budget vs. Profit:
     
   - Bar chart of Genre vs. Average Profit:
    

---

## 📐 Hypothesis Testing
**Hypothesis**: Horror movies generate higher profits than other genres.

- **Null Hypothesis (H₀)**: Average profit for horror movies equals that of other genres.
- **Alternative Hypothesis (H₁)**: Average profit for horror movies is greater.

### Methodology:
- Used **Welch’s t-test** due to:
  - Varying sample sizes.
  - Unequal variances across groups.

### Results:
- At a **90% confidence interval**, horror movies are statistically more profitable than other genres.

---

## 💡 Key Findings and Recommendations
1. **Genre Selection**:
   - Recommended **Horror** movies for high profitability within budget constraints.
   - Highlighted **Action** and **Thriller** genres but deemed them less feasible due to limited budgets.

2. **Profitability Analysis**:
   - Certain genres, despite high profitability, had insufficient data samples.

3. **Strategic Planning**:
   - Allocate budget prioritizing genres with high ROI and sufficient data support.

---

## 🛠️ Key Technologies
- **Programming Language**: Python
- **Libraries**: Pandas, Matplotlib, Scikit-learn, Statsmodels
- **Techniques**:
  - Data Cleaning
  - EDA
  - Hypothesis Testing
  - Statistical Modeling

---

## 🌟 Future Scope
- Expand the scope to include ensemble machine learning models for predictive analysis.
- Test on broader datasets for comprehensive insights.
- Incorporate advanced statistical techniques to enhance decision-making.

---

## 🔗 References
- [IMDB Movie Dataset]

---

### 📖 How to Use
1. Clone the repository to your local machine.
2. Install the required Python libraries.
3. Run the notebook files to view the analysis and results.
