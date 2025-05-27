📊 Task 2: Exploratory Data Analysis on EV Sales Dataset
📁 Dataset
Name: EVSalesDataset.csv

Description: Contains sales figures of electric vehicles (EVs) over multiple years and across different models/brands.

Goal: Perform Exploratory Data Analysis (EDA) to identify patterns, anomalies, and relationships among the variables.

✅ Tasks Completed
1. Summary Statistics
Used df.describe() to extract:

Mean, median, standard deviation, min/max, and quartiles.

Checked for missing values and confirmed all numerical columns (Year, Value) were clean.

2. Histograms
Created histograms to understand the distribution of:

Year: Most EV records are concentrated in recent years, showing a trend of growing interest in EVs.

Value: Right-skewed distribution indicating that a few EV models had very high sales, while most had moderate or low figures.

3. Boxplots
Used to detect outliers in the numerical features:

Value: Outliers were present, revealing that certain EV models had significantly higher sales than the rest.

Year: No significant outliers were found, data distribution was tight.

4. Correlation Matrix
Generated with:

python
Copy
Edit
sns.heatmap(df[num_cols].corr(), annot=True, cmap='coolwarm', fmt=".2f")
Insights:

Weak positive correlation (~0.25) between Year and Value, suggesting that sales have increased slightly over the years.

No strong linear dependencies.

5. Pairplot
Used sns.pairplot(df[num_cols]) to visually observe:

Mild upward trend between Year and Value, reinforcing the correlation matrix.

Data clustering around recent years with varying sales values.

📌 Inferences
EV sales have increased over recent years, as newer records dominate the dataset.

A few EV models are clear outliers in terms of sales (Value), indicating their popularity or market dominance.

No strong multicollinearity was found, but a moderate upward trend was observed between Year and Value.

📦 Files Included
EVSalesDataset.csv: Raw dataset used.

Task2Ans.ipynb: Jupyter notebook with code and analysis.

README.md: This summary document.
