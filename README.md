# Number of Orders Prediction

A machine learning project that predicts the number of orders for retail stores using LightGBM regression. This project analyzes various factors like store type, location, holidays, and discounts to forecast order volumes.


## 🔍 Overview

This project implements a machine learning solution to predict the number of orders for retail stores based on various business factors. The model uses LightGBM (Light Gradient Boosting Machine) for regression analysis to forecast order volumes, helping businesses optimize their inventory management and resource planning.

## ✨ Features

- **Data Analysis**: Comprehensive exploratory data analysis with interactive visualizations
- **Feature Engineering**: Automatic encoding of categorical variables
- **Machine Learning**: LightGBM regression model for accurate predictions
- **Interactive Visualizations**: Plotly-based charts for data insights
- **Easy Deployment**: Jupyter notebook format for easy execution and sharing

## 📊 Dataset

The dataset contains **188,340 records** with the following features:

| Column | Description | Type |
|--------|-------------|------|
| ID | Unique identifier | Object |
| Store_id | Store identifier | Integer |
| Store_Type | Type of store (S1, S2, S3, S4) | Categorical |
| Location_Type | Location category (L1-L5) | Categorical |
| Region_Code | Regional identifier | Object |
| Date | Transaction date | Object |
| Holiday | Holiday indicator (0/1) | Binary |
| Discount | Discount availability (Yes/No) | Binary |
| #Order | Number of orders (target variable) | Integer |
| Sales | Sales amount | Float |

### Dataset Statistics
- **Total Records**: 188,340
- **Features**: 9 input features + 1 target
- **Memory Usage**: ~14.4 MB
- **No Missing Values**: Clean dataset ready for analysis

## 🚀 Installation

### Prerequisites
- Python 3.7+
- Jupyter Notebook or Google Colab

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Number-of-orders-Prediction-.git
   cd Number-of-orders-Prediction-
   ```

2. **Install required packages**
   ```bash
   pip install pandas numpy scikit-learn lightgbm plotly
   ```

3. **For Google Colab users**
   - Simply open the notebook in [Google Colab](https://colab.research.google.com/github/PrajwalNandaragi/Number-of-orders-Prediction-/blob/main/number_of_orders_prediction.ipynb)

## 📖 Usage

### Running the Notebook

1. **Open the notebook**
   ```bash
   jupyter notebook number_of_orders_prediction.ipynb
   ```

2. **Execute cells sequentially**
   - The notebook is designed to run from top to bottom
   - Each cell builds upon the previous one

3. **View results**
   - Interactive visualizations will display in the notebook
   - Model predictions will be shown in the final output

### Key Steps

1. **Data Loading**: Import and examine the dataset
2. **Exploratory Data Analysis**: Generate insights through visualizations
3. **Data Preprocessing**: Encode categorical variables
4. **Model Training**: Train LightGBM regressor
5. **Prediction**: Generate order predictions

## 📈 Model Performance

The model uses **LightGBM Regressor** with the following configuration:

- **Algorithm**: LightGBM (Light Gradient Boosting Machine)
- **Training Data**: 150,672 samples (80% of total data)
- **Test Data**: 37,668 samples (20% of total data)
- **Features Used**: 4 (Store_Type, Location_Type, Holiday, Discount)
- **Training Method**: Row-wise multi-threading (auto-selected)

### Sample Predictions

| Sample | Predicted Orders |
|--------|------------------|
| 1      | 47.35            |
| 2      | 97.07            |
| 3      | 66.58            |
| 4      | 85.14            |
| 5      | 54.45            |

## 📊 Visualizations

The project includes interactive visualizations for:

- **Store Type Distribution**: Pie chart showing order distribution across store types
- **Location Type Analysis**: Geographic distribution of orders
- **Discount Impact**: Effect of discounts on order volumes
- **Holiday Patterns**: Order behavior during holidays vs. regular days

## 📦 Requirements

```txt
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
lightgbm>=3.2.0
plotly>=5.0.0
jupyter>=1.0.0
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

