🧠 ML Algorithm
K-Means Clustering
This algorithm helps group restaurants based on similar features such as:

Average rating

Cost for two

Cuisine types

📈 Exploratory Data Analysis (EDA)
✔️ Initial Insights:
Counted missing and duplicate values

Cleaned columns like Cost and Rating

Used visualizations like heatmaps, barplots, and pie charts

📊 Sample Visualizations:
1. Top 10 Cuisines:

2. Rating Distribution:

3. Correlation Heatmap:

4. Cost vs Rating:

📌 Clustering Process
Cleaned and preprocessed the dataset

Used LabelEncoder for categorical columns like Cuisines

Selected features: Cost, Rating, Cuisine Type

Applied KMeans with n_clusters=5

Visualized clusters using matplotlib

python
Copy
Edit
from sklearn.cluster import KMeans
model = KMeans(n_clusters=5)
df['Cluster'] = model.fit_predict(scaled_features)
💡 Insights
North Indian and Chinese were the most common cuisines

Restaurants with higher cost often had better ratings

Cluster 2 had low cost but high ratings — a sweet spot!

Restaurants with high online engagement had better performance overall

📈 Business Impact
✔️ Helps businesses:

Benchmark competitors

Target ideal customer segments

Identify underperforming cuisines or locations

✔️ Helps customers:

Discover similar restaurants

Choose based on cost-rating clusters
