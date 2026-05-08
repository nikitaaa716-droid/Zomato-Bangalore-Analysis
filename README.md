# 🍽️ Zomato Bangalore Restaurant Analysis

An Exploratory Data Analysis (EDA) and Machine Learning project on Zomato's Bangalore restaurant dataset using Python.

---

## 📌 Objective

To analyze restaurant data from Zomato Bangalore and uncover insights about location trends, online ordering impact, cost-rating relationships, and build a machine learning model to predict whether a restaurant will be highly rated.

---

## 📂 Dataset

- **Source:** Kaggle — Zomato Bangalore Restaurants Dataset
- **Records:** 41,665 restaurants (after cleaning)
- **Features:** 17 columns including location, cuisines, cost, ratings, votes, online ordering, and restaurant type

---

## 🔧 Data Cleaning

- Removed `/5` from rating column and converted to float
- Removed commas from cost column and converted to integer
- Encoded `online_order` (Yes → 1, No → 0) for ML compatibility
- Dropped rows with missing rating values

---

## 🔍 Key Insights

1. **BTM is Bangalore's most restaurant-dense area** — with ~4000 listings, nearly double the next location (Koramangala 5th Block), making it the city's biggest food hub.

2. **Online ordering correlates with slightly better ratings** — restaurants with online ordering average 3.73 vs 3.66 for those without, suggesting more customer-engaged businesses tend to perform better.

3. **Cost and rating have a weak positive correlation (r = 0.385)** — spending more slightly improves your chances of a good meal, but it's no guarantee. A ₹200 restaurant can still rate 4.5.

4. **Most Bangalore restaurants cluster under ₹1500 for two** — the city's dining market is largely budget to mid-range, with relatively few premium options.

5. **ML model achieved 78.16% accuracy** in predicting whether a restaurant is highly rated, using only cost and online ordering as features.

6. **Cost is by far the strongest predictor (97.4%)** — the Random Forest model found cost almost entirely drives rating prediction, while online ordering availability contributed only 2.6%.

---

## 📊 Visualizations

| Chart | Description |
|-------|-------------|
| `restaurants_per_loc.png` | Top 10 locations by number of restaurants |
| `online_order_rating.png` | Average rating: online order vs no online order |
| `cost_vs_rating.png` | Scatter plot of cost vs rating with trend line |
| `feature_importance.png` | ML model feature importance |

---

## 🤖 Machine Learning

- **Model:** Random Forest Classifier
- **Features:** Approx cost for two, Online order availability
- **Target:** High rating (1 if rate ≥ 4.0, else 0)
- **Accuracy:** 78.16%
- **Library:** scikit-learn

---

## 🛠️ Tools & Libraries

- Python 3.12
- pandas
- matplotlib
- seaborn
- scikit-learn
- Google Colab

---

## 🚀 How to Run

1. Clone this repository
2. Upload `zomato.csv` to your working directory
3. Open the `.ipynb` file in Jupyter or Google Colab
4. Run all cells in order

---

## 👤 Author

**Nikita**  
NIT Trichy
