# 🏠 Airbnb NYC Listing Segmentation using K-Means Clustering

This project applies unsupervised learning (K-Means clustering) to segment Airbnb listings in New York City based on key features such as price, location, availability, reviews, and room type. The aim is to uncover hidden patterns and create business-meaningful customer segments.

---

## 📌 Objective

To analyze Airbnb NYC listings and group them into distinct clusters using **K-Means**, enabling better understanding of pricing behavior, location demand, and listing types.

---

## 📊 Dataset

- **Source**: [New York City Airbnb Open Data](https://www.kaggle.com/datasets/sudhanvahg/new-york-airbnb-bookings)
- **Size**: ~48,000 listings
- **Key Features**:
  - `price`, `minimum_nights`, `number_of_reviews`
  - `room_type`, `neighbourhood_group`, `availability_365`
  - Geographic coordinates (`latitude`, `longitude`)

---

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn (KMeans, StandardScaler)
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🧪 Methodology

1. **Data Cleaning**
   - Dropped irrelevant columns (`id`, `name`, `host_name`, etc.)
   - Handled missing values
2. **Feature Encoding & Scaling**
   - One-hot encoded `room_type` and `neighbourhood_group`
   - Standardized numerical features
3. **Elbow Method**
   - Determined optimal `k = 5` clusters
4. **K-Means Clustering**
   - Trained model on scaled data
   - Assigned clusters to each listing
5. **Cluster Profiling**
   - Analyzed each cluster’s average price, review count, location distribution, etc.

---

## 📈 Cluster Summary

| Cluster | Summary |
|---------|---------|
| **0** | Budget listings, mostly in Brooklyn, ~52% private rooms, avg. price ~$114 |
| **1** | High-end Manhattan apartments, longer stays, avg. price ~$184 |
| **2** | High-review, short-stay budget listings with high turnover |
| **3** | Affordable, long-availability listings in Queens |
| **4** | Small cluster in Staten Island — niche, outlier behavior |

---

## 🔍 Key Insights

- Clear segmentation of listing behavior based on price and borough
- Brooklyn and Manhattan dominate the listings with contrasting pricing patterns
- K-Means offers meaningful business insights for pricing strategy and market focus

---

