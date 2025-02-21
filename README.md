# BlackScholes

# 📘 Black-Scholes Option Pricing Calculator**
### A Python-based **Black-Scholes Model** for pricing European **call and put options** with an interactive **Jupyter Notebook UI** using `ipywidgets`.

## **🚀 Features**
✅ **Calculates theoretical option prices** using the Black-Scholes formula  
✅ **Fetches real-time stock prices** using **Alpha Vantage API**  
✅ **Computes historical volatility** using 1-year price data  
✅ **Interactive UI with Jupyter Widgets** for easy input selection  
✅ **Supports call and put options**  
✅ **Error handling for invalid inputs**  

## **📌 How It Works**

The formula used is:

\[
C = S N(d_1) - K e^{-rT} N(d_2)
\]

\[
P = K e^{-rT} N(-d_2) - S N(-d_1)
\]

where:

- \( S \) = Current stock price  
- \( K \) = Strike price  
- \( T \) = Time to expiration (in years)  
- \( r \) = Risk-free interest rate  
- \( \sigma \) = Volatility of the stock  
- \( N(d) \) = Cumulative normal distribution  

---

Open the **Black-Scholes-Calculator.ipynb** file.

### **Select Inputs in the UI**
- Pick a **stock ticker** (AAPL, MSFT, TSLA, etc.).
- Select an **option maturity date**.
- Enter a **strike price**.
- Choose **Call or Put**.
- Click **"Calculate"** to see the option price.

---

## **📊 Example Output**
```
Black-Scholes call option price for AAPL: $12.35
```

---

## **⚡ Technologies Used**
- **Python** (Core computation)
- **NumPy & SciPy** (Mathematical operations)
- **Alpha Vantage API** (Fetching real-time stock prices)
- **ipywidgets** (Interactive UI for Jupyter Notebook)
- **Jupyter Notebook** (Running & visualizing calculations)

---

## **📝 Notes**
- This model **assumes European-style options**, meaning options can only be exercised at expiration.
- The **risk-free rate** is based on the **10-year Treasury yield**.
- The script fetches **historical volatility** using **1-year stock price data**.
