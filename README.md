# 🏦 Indian Bank Stock Price Prediction using Hybrid LSTM-QNN

A sophisticated stock market prediction system that combines Long Short-Term Memory (LSTM) neural networks with Quantum Neural Networks (QNN) to predict Indian bank stock prices with enhanced accuracy.

## 🌟 Features

- **Hybrid Architecture**: Combines classical LSTM with quantum computing concepts for improved prediction accuracy
- **Indian Bank Focus**: Pre-configured for 15 major Indian bank stocks
- **Real-time Data**: Fetches live stock data using Yahoo Finance API
- **Technical Indicators**: Incorporates RSI, Moving Averages, and Volume analysis
- **Interactive Visualization**: Comprehensive charts showing current vs predicted prices
- **Next-day Prediction**: Specialized focus on predicting the next trading day's closing price

## 🏗️ Architecture

The system uses a novel hybrid approach:

1. **LSTM Layer**: Processes sequential stock data to capture temporal patterns
2. **Quantum Neural Network**: Simulates quantum gates (RX, RY, RZ) and entanglement for enhanced pattern recognition
3. **Technical Analysis**: Integrates multiple technical indicators for comprehensive market analysis

## 📊 Supported Banks

The system supports 15 major Indian banks:

- HDFC Bank (HDFCBANK.NS)
- ICICI Bank (ICICIBANK.NS)
- State Bank of India (SBIN.NS)
- Kotak Mahindra Bank (KOTAKBANK.NS)
- Axis Bank (AXISBANK.NS)
- IndusInd Bank (INDUSINDBK.NS)
- Bandhan Bank (BANDHANBNK.NS)
- Federal Bank (FEDERALBNK.NS)
- IDFC First Bank (IDFCFIRSTB.NS)
- RBL Bank (RBLBANK.NS)
- Punjab National Bank (PNB.NS)
- Bank of Baroda (BANKBARODA.NS)
- Canara Bank (CANBK.NS)
- Union Bank of India (UNIONBANK.NS)
- Bank of India (BANKINDIA.NS)

## 🚀 Quick Start

### Prerequisites

```bash
pip install numpy pandas matplotlib yfinance scikit-learn
```

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/indian-bank-stock-prediction.git
cd indian-bank-stock-prediction
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the prediction system:
```bash
python main.py
```

### Usage

1. **Interactive Mode**: Run the script and select from 15 Indian banks
2. **Direct Symbol**: Specify a bank symbol directly
3. **Jupyter Notebook**: Use the provided notebook for detailed analysis

```python
from stock_prediction import StockPredictionSystem

# Initialize the system
predictor = StockPredictionSystem(symbol='HDFCBANK.NS', sequence_length=10)

# Fetch and prepare data
predictor.fetch_stock_data(period='6mo')

# Train the model
predictor.train_model(epochs=20)

# Predict tomorrow's price
predicted_price = predictor.predict_tomorrow()

# Generate visualization
predictor.create_visualization()
```

## 📈 Model Performance

The hybrid LSTM-QNN model typically achieves:
- **Training Loss**: ~0.075 (after 20 epochs)
- **Test Loss**: ~0.24
- **Prediction Accuracy**: Optimized for next-day price prediction

## 🔬 Technical Details

### LSTM Component
- Hidden units: 32 (configurable)
- Sequence length: 10 days
- Features: Open, High, Low, Close, Volume, MA_5, MA_10, RSI, Volume_MA

### Quantum Neural Network
- Qubits: 4 (configurable)
- Layers: 2
- Gates: RX, RY, RZ rotations with entanglement

### Data Processing
- MinMax scaling for normalization
- 80/20 train-test split
- Technical indicators calculation
- Sequence generation for time series

## 📊 Visualization Features

The system generates comprehensive visualizations including:

1. **Price Trend Analysis**: Historical vs predicted prices
2. **Current vs Next Day Comparison**: Bar chart comparison
3. **Price Change Analysis**: Expected change with percentage
4. **Volume Analysis**: Trading volume trends
5. **RSI Indicator**: Overbought/oversold signals
6. **Moving Averages**: 5-day and 10-day trends

## ⚠️ Disclaimer

This project is for educational and research purposes only. Stock market predictions are inherently uncertain, and this system should not be used as the sole basis for investment decisions. Always consult with qualified financial advisors before making investment choices.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Yahoo Finance for providing stock data API
- The quantum computing community for QNN concepts
- Indian banking sector for providing rich market data

## 📞 Contact

For questions or suggestions, please open an issue or contact [your-email@example.com].

---

**Made with ❤️ for the Indian financial market**
