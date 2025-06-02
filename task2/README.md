# Stock Price Prediction using LSTM Neural Networks

A machine learning project that predicts stock prices using Long Short-Term Memory (LSTM) neural networks implemented in TensorFlow/Keras.

## 🎯 Project Overview

This project demonstrates time series forecasting for stock price prediction using deep learning techniques. It includes data preprocessing, feature engineering, model building, and comprehensive evaluation of LSTM-based neural networks.

## 📊 Dataset

The project uses the [Stock Market Dataset](https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset) from Kaggle, which contains:
- Historical stock price data for multiple companies
- OHLCV data (Open, High, Low, Close, Volume)
- Stock metadata and company information

## 🛠️ Technologies Used

- **Python 3.7+**
- **TensorFlow/Keras** - Deep learning framework
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Scikit-learn** - Machine learning utilities

## 📋 Requirements

Install the required packages using:

```bash
pip install -r requirements.txt
```

You'll also need to set up the Kaggle API:
1. Go to Kaggle → Account → Create API Token
2. Download `kaggle.json` and place it in `~/.kaggle/`
3. Set permissions: `chmod 600 ~/.kaggle/kaggle.json`

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd stock-price-prediction-lstm
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the notebook**
   ```bash
   jupyter notebook main.ipynb
   ```

## 📁 Project Structure

```
├── main.ipynb              # Main Jupyter notebook
├── requirements.txt        # Python dependencies
├── README.md              # Project documentation
├── .gitignore             # Git ignore file
└── stock_data/            # Downloaded dataset (created when running)
    ├── stocks/            # Individual stock CSV files
    └── symbols_valid_meta.csv
```

## 🔬 Methodology

1. **Data Acquisition**: Download stock market data from Kaggle
2. **Data Preprocessing**: 
   - Handle missing values
   - Normalize price data using MinMaxScaler
   - Create sequences for time series prediction
3. **Model Architecture**:
   - Basic LSTM model with dropout layers
   - Advanced model with Bidirectional LSTM + GRU
4. **Training & Evaluation**:
   - 80/20 train-test split
   - RMSE evaluation metric
   - Comprehensive visualization

## 📈 Results

The notebook includes two model implementations:
- **Basic LSTM**: Simple architecture for baseline performance
- **Advanced Model**: Bidirectional LSTM + GRU with learning rate scheduling

Performance is evaluated using:
- Root Mean Square Error (RMSE)
- Visual comparison plots
- Training/validation loss curves

## ⚠️ Disclaimer

This project is for **educational purposes only**. The models and predictions should not be used for actual trading or investment decisions without proper risk management, additional validation, and professional financial advice.

## 🤝 Contributing

Feel free to contribute by:
- Reporting bugs
- Suggesting new features
- Improving documentation
- Adding new model architectures


## 🙏 Acknowledgments

- Kaggle for providing the stock market dataset
- TensorFlow team for the excellent deep learning framework
- The open-source community for various tools and libraries used
