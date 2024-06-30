# Trading-Bot_with_ALPACA

<!DOCTYPE html> 
![logo](https://github.com/prabhakarvenkat/Trading-Bot_with_ALPACA/blob/33b3c9ed8e7a638b161997a947b5e6368ecf6524/2023-12-15_2024-6-20/Screenshot%202024-06-30%20223105.png)
<html> <head> </head> <body> <h1>Alpaca Trading Bot</h1> <h2>Overview</h2> <p>This is a Python script that creates a trading bot using the Alpaca API. The bot scans for trading opportunities based on the top losing stocks and popular crypto assets from YahooFinance. It then uses the Alpaca API to execute buy and sell orders and sends notifications via Slack about the trades it makes.</p> <h2>Key Features</h2> <ul> <li>Retrieves historical market data for stocks and crypto via the Alpaca API</li> <li>Calculates the rate of change (ROC) of the ask price for a list of stocks over a 1 minute timeframe</li> <li>Compares the ask price and last traded price for the stock with the highest ROC</li> <li>Places a buy order for the stock if ask price > last traded price, allocating 100% of capital</li> <li>Sells the stock after a 2% gain</li> <li>Sends trade notifications via Slack</li> </ul> <h2>Setup</h2> <p>To use the bot, you'll need:</p> <ul> <li>An Alpaca account (paper trading account recommended)</li> <li>API keys from Alpaca</li> <li>Python installed with required libraries like alpaca-trade-api and pandas</li> </ul> 

<h2> Procedure: </h2>
1. Create a virtual environment `conda create -n trader python=3.10` <br>
2. Activate it `conda activate trader` <br>
3. Install initial deps `pip install lumibot timedelta alpaca-trade-api==3.1.1` <br>
4. Install transformers and friends `pip install torch torchvision torchaudio transformers` <br>
5. Update the `API_KEY` and `API_SECRET` with values from your Alpaca account <br>
6. Run the bot `python tradingbot.py`  <br>
  
<h2>Usage</h2> <p>The bot can be run from the command line by executing the main Python script. It will automatically scan for trading opportunities, place orders, and send Slack notifications.</p> 

## Other References 🔗

<p>-<a href="github.com/Lumiwealth/lumibot)">Lumibot</a>:trading bot library, makes lifecycle stuff easier .</p>


<h2>Disclaimer</h2> <p>This bot is for educational and informational purposes only. It does not constitute financial advice. Past performance is not indicative of future results. Use at your own risk.</p> </body> </html>
