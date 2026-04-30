
# Retail Sales Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project performs a deep-dive **Exploratory Data Analysis** on a retail dataset to uncover the underlying patterns governing product sales across various outlets. By leveraging statistical visualizations, this analysis identifies key distributions, outliers, and categorical imbalances that directly impact business decision-making and future predictive modeling.

---

## 🔍 Statistical Analysis & Key Findings

### 1. 🔥🗺️ Correlation Heatmap

* **Description:**

> A heatmap showing the strength and direction of linear relationships between numerical variables using color intensity and annotated correlation values.

* **Observations:**

> *Only Item_MRP has a noticeable positive relationship with Item_Outlet_Sales, while all other variables show weak or negligible correlations.

<img width="1060" height="682" alt="correlation_heatmap_with_coolwarm_cmap" src="https://github.com/user-attachments/assets/98772be2-33a9-4f00-864d-79d3395d6591" />


### 2. 📦 Box Plot of Item_Outlet_Sales

* **Description:**

> A box plot summarizing the distribution of Item_Outlet_Sales through median, quartiles, spread, and outliers.

* **Observations:**

> The data is right-skewed with many high-value outliers, meaning most sales are relatively low with a few exceptionally high values.

<img width="1574" height="525" alt="Item_outlet_plot" src="https://github.com/user-attachments/assets/76580462-fa13-4c69-9565-476377492ed2" />


### 3. 📊 Histogram of Item_Weight

* **Description:**

> A histogram illustrating how Item_Weight values are distributed across different ranges.

* **Observations:**

> The weights are fairly evenly distributed without strong skewness or extreme outliers, indicating a balanced spread of values.

<img width="859" height="448" alt="Item_Weight_histo" src="https://github.com/user-attachments/assets/8d6b8927-ff0c-4b99-8ce2-e06f515113c1" />


### 4. 📊 Item MRP Distribution

* **description:**

> Histogram showing the distribution of item prices (MRP) across the dataset, expressed as percentages.

* **observation:**

 > The distribution is fairly spread out across the price range, indicating a wide variety of product pricing with no strong skewness or dominant peak.

<img width="841" height="448" alt="Item_MRP" src="https://github.com/user-attachments/assets/e0819a1d-7bd6-4f50-a5ca-073de5369014" />


### 5. 📊 Item Visibility Distribution

* **description:**

> Histogram showing the distribution of item visibility across the dataset, expressed as percentages.

* **observation:**

> The distribution is right-skewed, indicating that most items have low visibility, while only a small number of items have high visibility.

<img width="841" height="448" alt="Item_Visibility_Distribution" src="https://github.com/user-attachments/assets/19a95132-0a96-408c-b04f-f31f77bff957" />


### 6. 📊 Outlet Size Distribution

* **description:**

> Bar plot showing the distribution of items across different outlet sizes in the dataset.

* **observation:**

> Medium-sized outlets have the highest count, while High-sized outlets have the lowest representation, indicating an imbalance in outlet size distribution.

<img width="580" height="490" alt="Out_Size_Distirbution" src="https://github.com/user-attachments/assets/6378d683-0b09-49d6-8c60-5b50fd5f0f25" />


### 7. 📊 Outlet Type Distribution

* **description:**

> Bar plot showing the distribution of items across different outlet types in the dataset.

* **observation:**

> Supermarket Type1 has the highest count by a large margin, indicating it is the most dominant outlet type in the dataset.

<img width="580" height="490" alt="Out_Size_Distirbution" src="https://github.com/user-attachments/assets/6a1fe05c-3a18-4ab2-936e-e7cacd31b989" />


---

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **Data Manipulation:** `Pandas`, `NumPy`
* **Visualization:** `Seaborn`, `Matplotlib`

---

## 🚀 Future Work & Recommendations
* **Feature Engineering:** Apply **Log Transformations** to the skewed sales and visibility data to normalize the distribution for linear modeling.
* **Data Imputation Strategy:** Investigate the artificial frequency spike in `Item_Weight` to determine if it resulted from mean/median imputation.
* **Bivariate Analysis:** Explore the correlation between `Item_MRP` and `Item_Outlet_Sales` to see if higher price tiers yield higher total volume.
