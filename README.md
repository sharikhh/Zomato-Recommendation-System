# 🍽️ Zomato Recommendation System

A comprehensive machine learning project that provides personalized restaurant recommendations using a combination of clustering, NLP, and multiple recommendation strategies including popularity-based, memory-based, association rules, and content-based filtering.

> **By Sharikhh Hunagund**

---

## 📚 Table of Contents

- [Problem Statement](#problem-statement)
- [Plan of Action](#plan-of-action)
- [Text Preprocessing](#text-preprocessing)
- [Clustering with K-Means](#clustering-with-k-means)
- [Observations & Inferences](#observations--inferences)
- [Recommendation Systems](#recommendation-systems)
  - [1. Popularity-Based](#1-popularity-based)
  - [2. Memory-Based](#2-memory-based)
  - [3. Association Rule-Based](#3-association-rule-based)
  - [4. Content-Based](#4-content-based)
- [Key Insights](#key-insights)
- [Conclusion](#conclusion)
- [Technologies Used](#technologies-used)

---

## ❓ Problem Statement

- To optimize the delivery system of Zomato by analyzing user preferences and behavior.
- To recommend restaurants to customers based on past behavior, similar cuisines, ratings, and more.
- To extract actionable insights for restaurant partners and the Zomato platform.

---

## 🚀 Plan of Action

1. **EDA (Exploratory Data Analysis)**
2. **Text Preprocessing**
3. **K-Means Clustering**
4. **Recommendation System Development**
5. **Insight Extraction & Evaluation**

---

## 🧹 Text Preprocessing

The following steps were performed on review and restaurant text data:
- Lowercasing  
- Removal of punctuation  
- Removal of stopwords  
- Removal of URLs  
- Spelling correction  

---

## 📊 Clustering with K-Means

K-Means Clustering was used to segment restaurants and user behavior into distinct groups. These clusters helped:
- Understand user preferences
- Optimize delivery boy allocation
- Formulate better targeted recommendations

---

## 🧠 Observations & Inferences

- **Cluster 0**: High average ratings and frequent online orders.
- **Cluster 1**: Fewer online orders with mixed reviews.
- **Cluster 2**: New/low-rated restaurants with sparse data.

📌 Delivery trends:
- Cluster 0 → 55% of delivery load
- Clusters 1 & 2 → Remaining 45%

These insights help optimize staffing and delivery efficiency.

---

## 🔁 Recommendation Systems

### 1. ⭐ Popularity-Based
Recommends restaurants based on:
- High ratings
- Number of votes
- Trending cuisines in cluster 0

Great for new users with no prior history.

---

### 2. 🧠 Memory-Based

Uses collaborative filtering based on:
- User-item interaction matrix
- Cosine similarity between users/restaurants
- Recommends restaurants preferred by similar users

---

### 3. 🔗 Association Rule-Based

Uses market basket analysis logic:
- Identifies frequently ordered dish combinations
- Suggests items that are often bought together

---

### 4. 🧾 Content-Based

Based on restaurant attributes like:
- Cuisines
- Location
- Review content
- Cost

Finds and recommends similar restaurants using cosine similarity of text vectors.

---

## 💡 Key Insights

- **From Ratings**: Restaurants with similar average ratings tend to be recommended together.
- **From Reviews**: Textual similarity in customer reviews improves recommendations.
- **From Combos**: Certain food items are frequently sold together and can be bundled.
- **From Popularity**: Cluster 0 contains the most popular and recommended restaurants.

---

## ✅ Conclusion

✔️ Addressed both problem statements:
- Optimized delivery allocation using K-Means
- Built four types of recommendation systems

✔️ Extracted valuable insights that:
- Help restaurants understand their standing
- Help Zomato refine its recommendation strategy

📦 All four systems can be pipelined to form a robust hybrid recommendation engine.

---

## 🧰 Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- NLP (TF-IDF, cosine similarity)
- K-Means Clustering
- Association Rule Mining

---

> ⚠️ **Note:** This project is a prototype. Future versions can include collaborative filtering with more dynamic user data and deep learning models.

