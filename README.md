# 🔥 Classification of Fire Types in India Using MODIS Satellite Data

This project focuses on classifying various types of forest fires in India using NASA’s MODIS satellite data. The goal is to provide a machine learning-based solution to identify and predict fire categories, helping environmental agencies and disaster response units take timely actions.

## 📁 Project Structure

📦 Fire Classification Project
├── Classification_of_Fire_Types_in_India_Using_MODIS_Satellite_Data.ipynb
├── modis_2021_India.csv
├── modis_2022_India.csv
├── modis_2023_India.csv
└── README.md


## 🛰️ Dataset

The project uses fire data from the [MODIS (Moderate Resolution Imaging Spectroradiometer)](https://modis.gsfc.nasa.gov/) satellite, covering the years:

- 🔹 `2021` (`modis_2021_India.csv`)
- 🔹 `2022` (`modis_2022_India.csv`)
- 🔹 `2023` (`modis_2023_India.csv`)

### Dataset Features:

- `latitude`, `longitude`: Geospatial coordinates of the fire.
- `brightness`, `frp`: Indicators of fire intensity.
- `confidence`: Level of certainty that a fire occurred.
- `type`: Fire type indicator (e.g., vegetation fire, peat fire, etc.)
- `acq_date`, `acq_time`: Date and time of acquisition.

## 🧠 ML Pipeline

The core steps in the notebook are:

1. **Data Cleaning & Preprocessing**
   - Concatenation of datasets across years.
   - Handling missing values.
   - Encoding categorical features.

2. **Exploratory Data Analysis (EDA)**
   - Visualizations to understand spatial and temporal trends.
   - Distribution of fire types and intensities.

3. **Model Building**
   - Tested models: `Random Forest`, `Decision Tree`, `Logistic Regression`, `XGBoost`.
   - Evaluation metrics: `Accuracy`, `Precision`, `Recall`, `F1-Score`, `Confusion Matrix`.

4. **Model Evaluation**
   - Selected best performing model based on overall accuracy and class-wise recall.

## 📊 Results

| Model              | Accuracy |
|-------------------|----------|
| Random Forest      | 0.94     |
| XGBoost            | 0.95     |
| Decision Tree      | 0.91     |
| Logistic Regression| 0.88     |

🔍 **XGBoost** outperformed other models with the highest accuracy and stable generalization.

## 📷 Visualizations

> Include these screenshots in your GitHub repo and update the URLs below.

### Confusion Matrix  
![Confusion Matrix](https://github.com/your-username/your-repo/blob/main/assets/confusion_matrix.png)

### Feature Importance  
![Feature Importance](https://github.com/your-username/your-repo/blob/main/assets/feature_importance.png)

## 📌 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## ✅ Outcomes

- Successfully predicted fire types with high accuracy.
- Highlighted critical features like `brightness`, `frp`, and `confidence` in fire classification.
- Demonstrated temporal trends in forest fire occurrence.

## 🚀 Future Scope

- Integrate real-time satellite data using APIs.
- Deploy a live dashboard for fire monitoring.
- Extend model to include climatic variables (temperature, rainfall, etc.).

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

## 🙋‍♂️ Author

**Harshanth R**  
[LinkedIn](https://www.linkedin.com/in/harshanth0112) | [GitHub](https://github.com/harshanth0112)

---

