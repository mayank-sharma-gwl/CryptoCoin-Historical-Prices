# CryptoCoin-Historical-Prices
This script scrapes data from the [historical data](https://coinmarketcap.com/currencies/ethereum/historical-data/) tab on coinmarketcap.com

## Install & Run

#### Download and install   
```
$ git clone [https://github.com/mayank-sharma-gwl/CryptoCoin-Historical-Prices.git]
$ cd CryptoCoin-Historical-Prices
$ pip3 install -r requirements.txt
$ python install_locally.py 
```

#### Running
To run the script and gather data for all listed cryptocurrencys on coinmarketcap you need to pass the start date and end date in YYYYMMDD format

```    
$ python3 crypto_history.py 20170101 20180201
``` 
you can also specify a cryptocurrency with a third argument

```    
$ python3 crypto_history.py 20170101 20180201 ethereum
``` 
The data will be saved to a CSV file

#### Importing

```bash
>>> from crypto_history import gather
>>> gather('20170101', '20170102', ['ethereum'])
(['Coin', 'Date', 'Open', 'High', 'Low', 'Close', 'Volume', 'Market Cap'], [[], ['ethereum', 'Jan 02, 2017', '8.17', '8.44', '8.05', '8.38', '14,579,600', '714,900,000'], ['ethereum', 'Jan 01, 2017', '7.98', '8.47', '7.98', '8.17', '14,731,700', '698,149,000']])
```


