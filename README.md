
Built by https://www.blackbox.ai

---

```markdown
# SPY Price Predictor

## Project Overview
The SPY Price Predictor is a web application designed to provide real-time price predictions for the SPDR S&P 500 ETF (SPY). The application fetches historical trading data, analyzes it using machine learning models, and presents predictions alongside current market data. It visually displays the predicted price, the actual current price, their respective changes, and prediction accuracy metrics, offering users valuable insights for trading strategies.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd spy-price-predictor
   ```

2. **Install the required Python packages:**
   Make sure you have Python installed on your machine. Use the following command to install the necessary packages:
   ```bash
   pip install -r requirements.txt
   ```

   Make sure to install the dependencies in `requirements.txt`, which should include packages like Flask, joblib, yfinance, scikit-learn, etc.

3. **Install Node.js dependencies:**
   If you plan to run the frontend, ensure you have Node.js installed, and then run:
   ```bash
   npm install
   ```

4. **Download the dataset:**
   Download the SPY intraday dataset from Kaggle or use the provided JSON metadata to fetch the data.

5. **Run the backend server:**
   Start the Flask server for the data API.
   ```bash
   python server.py
   ```

6. **Open the web application:**
   You can now open the `index.html` file in your browser to see the application in action.

## Usage

1. Open your web browser and navigate to `index.html`.
2. The application will display the current SPY price, the predicted price for the next 10 minutes, and additional key factors influencing the prediction.
3. The system updates every minute, showing real-time data and prediction changes.

## Features

- Real-time price prediction for SPY.
- Display current SPY price and its change.
- Prediction performance metrics including accuracy over the last hour and day.
- Visual representation of key factors impacting price predictions.
- Responsive design for mobile and desktop views.

## Dependencies

The main dependencies required for this project are listed in the `package.json` and `requirements.txt` files.

### Frontend Dependencies (package.json)
- Tailwind CSS: Used for styling the application.
- Font Awesome: For iconography.

### Backend Dependencies (requirements.txt)
- Flask: For creating the web server.
- yfinance: To fetch historical financial data.
- joblib: To save and load trained machine learning models.
- scikit-learn: For model training and predictions.
- pandas: To handle data manipulation.

## Project Structure

```
/spy-price-predictor
│
├── index.html         # Main HTML file for the web application
├── styles.css         # CSS file for styling the application
├── script.js          # JavaScript file for the frontend functionality
├── server.py          # Python script to run the backend server
├── model_trainer.py   # Script to train and save the prediction model
├── godel_client.py     # WebSocket client for real-time data connection
├── simulation.py      # Simulation script to evaluate predictions
├── historical_trainer.py # Loads and trains using historical data
├── simulation_with_kaggle_data.py # Runs simulations using Kaggle data
├── requirements.txt    # Python dependencies
└── package.json       # Frontend dependencies
```

## Conclusion

The SPY Price Predictor is a powerful tool for traders and investors looking to make informed decisions based on real-time data and predictive analytics. It combines financial data retrieval, machine learning, and user-friendly design to provide up-to-date insights into SPY price movements.
```