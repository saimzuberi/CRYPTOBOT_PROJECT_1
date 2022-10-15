# Project_Module_1
## CryptoBOT Analytics Buy &amp; Sell Triggers
---
# PROJECT OVERVIEW 

The objective of the current project was to establish the basis of building a alogrithim based trading bot working on various possible strategies including trading pattern and 200D simple moving average (SMA) technical data to make a decision for buying and selling of a crypto currency. 

For the purpose of implementation of the solution we have used POLYGON.io which provides us with the data for the complete crypto currencies over the last 2 year and based on the categorization of the crypto currencies, we have established 3 types of coorelated portfolios including MEME Cryptos, BLOCKCHAIN crypto and COIN Crypto and identified the complete co-relation among them. 

The implementaion of the analysis allowed for implemenation of buy and hold strategy which resulted in the following results. 

---

## BUY & HOLD STRATEGY 
    
    INITIAL INVESTMENT 100,000

    MEME STOCK RESULTS - USD 58447.00

![PORTFOLIO RESULTS - MEME](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.14.04 AM.png)
    
    COIN STOCK RESULTS - USD 235,581.00

![PORTFOLIO RESULTS - COIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.10.26 AM.png)

    BLOCKCHAIN STOCK RESULTS - USD 151779.00

![PORTFOLIO RESULTS - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.12.59 AM.png)

---

## PORTFOLIO RISK IDENTIFICATION

Using MONTY CARLOS simulation, the following are the results of the possible risk analysis portfolios 

### MEME CRYPTOS  
![MONTYCARLOS - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.07.42 AM.png)
![CORELATION - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.08.50 AM.png)

### COIN CRYPTOS 
![MONTYCARLOS - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.05.15 AM.png)
![CORELATION - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.06.38 AM.png)

### BLOCKCHAIN CRYPTOS 
![MONTYCARLOS - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 12.58.26 AM.png)
![CORELATION - BLOCKCHAIN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.02.21 AM.png)

---

# PATTERN RECOGNITION USING TALIB

We using the TALIB to do the analysis of 297 crypto currencies and identified the candle stick patterns dertining the bear or bullish patterns in the symbols. 

![CRYTO CANDLESTICK PATTERN](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.15.35 AM.png)

Our analysis communicated the currency wise bear or bullish patterns over the last 2 years. 

![CRYTO CANDLESTICK MAPPING](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.19.06 AM.png)

---

# TRADING STRATGY RESULTS

Using the determinant from the CANDLE STICK patterns and MONTY CAROLS, we selected BTC to implement the TALIB to implement 200 DAY SMA to implement buy and sell strategy. The result of the strategy is as below. 

![BUY & SELL ORDERS](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.25.14 AM.png)

![PRICE SMA & RSI ](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.26.59 AM.png)

![Bollinger bans ](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.28.17 AM.png)

![CANDLESTICK DISPLAY OF BTC](blockchainbot/Documentation/Screenshot 2022-10-15 at 1.38.54 AM.png)

---

# INSTALLATION GUIDE
## INITIAL SETUP
> Run: `pip install -r requirements.txt` from the `blockchainbot/` folder

### At the start of every Notebook
* Add the following code in the first cell of any notebook you start
```
import sys

sys.path.append('../SourceCode/')
```

### local_settings.py (file structure)
    data_storage_path='/Users/charlotte/Data'
    source_code_path='/Users/charlotte/UofT/blockchainbot/SourceCode'
    
    
    * create the file (if not exist in the repo) `SourceCode/` (Where README.md file exists)
    * set the following variables:
        * data_storage_paht='/absolute/path/to/the/shared/google/drive/folder/for/data'
        * source_code_path= 'absolute/path/to/the/`SourceCode`/folder'
        * polygon_api_key='your_polygon_api_key'

### .env (file structure)
    api_key='your_polygon_api_key'
    polygon_api_key='your_polygon_api_key'

**NOTE: To get absoute path of a file or a folder, use the terminal. Drag the file or the folder onto the terminal. The absolute path will be revealed**

### Pattern Recognition:
* installation >> `conda install -c conda-forge ta-lib`
___
## References:

* Polygon API Documentation for Stocks Crypto and Forex API
    > polygon.io/docs/crypto/getting-started
* Dependencies
---
# CODE ARCHITECHTURE

## DATA ARCHITECHTURE 

![DATA ARCHITECTURE](blockchainbot/Documentation/DataStructure.drawio.png)

## CODE FOLDERS 

    blockchainbot (database local copy) 
    Documentation (documents and images) 
    Notebook (main code) 
    Scripts (code downloading script) 
    Scource Code ( supporting code including candlestickpattern.py, dataManagement.py, local_settings.py, marketData.py, MCForecastTools.py and  other temp code)  
    Presentation
    Readme.md
    requirements.txt 
    
