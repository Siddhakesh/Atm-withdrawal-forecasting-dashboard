# Atm-withdrawal-forecasting-dashboard

ATM Withdrawal Forecasting Streamlit Dashboard

## Files
- `app.py`: Streamlit dashboard
- `sample_atm_transactions.csv`: Sample upload file in the transaction format
- `requirements.txt`: Python dependencies

## Run Locally
1. Install Python 3.10+.
2. Open a terminal in this folder.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the dashboard:
   ```bash
   streamlit run app.py
   ```
5. Upload `sample_atm_transactions.csv` when prompted.

The dashboard aggregates transaction data hourly, creates lag features, trains either Linear Regression or Random Forest, evaluates MAE/RMSE, plots actual versus predicted values, and allows downloading results.

*Note: The sample data is synthetic. The dashboard predicts hourly withdrawal demand, not the cash balance remaining in the ATM.*
