# blind-trader

## Architecture

#### Sociopath - Social Media Bot

[]()
#Step 1: Fethcing the data
- Start connecting into some of the social media data via API. To start, the following SM's should be captured as a base line:
  $ Twitter
  $ Stocktwits
  $ ?


#Step 2: Storing the data
- Spin up a MySQL database for us to house the data. 

#Step 3: Spinning up a server
- We can either stand one up locally (I have a desktop I can use for this) or we use Heroku or Dokku which are a couple that are recommended.

#Step 4: Parsing the data
- There are couple options I found online such as (Redis -https://redis.io/) and (Pudo - https://github.com/pudo/dataset)
- Ultimatley we have to create tables that can reflect the following:
  $ TICKER SYMBOL
  $ # of TIMES someone talked about it
  $ the amount of time that has occured
      (There is a cool video that I want to find that talks about how reddit always keeps updating their front based based on a defined set rules. We could replicate something similar to that to see what the most popular ticker is at any given time.
      
$Step 4: Building the bot
- ?

#### Hoarder - Historical Data Bot

[IEX Trading](https://iextrading.com/developer/)

#### Nerd - Statistical Computation Bot

[]()

#### Executioner - Stock Trader Bot

[Alpaca API](https://alpaca.markets/)

#Step 1: Fethcing the data
- Start connecting into some of the market data via API. To start the following tickers should be captured as a base line:
  $AAPL
  $GOOGL
  $SQ
  $NVDA
  $AMD
  $NDX
  $DJX
  $SPX
  $VIX
  $SPY

- A minimum of 10 years should be captured, but 20 years would be ideal so that we can capture bear market conditions such as that in 2008

#Step 2: Storing the data
- Spin up a MySQL database for us to house the data. 

#Step 3: Spinning up a server
- We can either stand one up locally (I have a desktop I can use for this) or we use Heroku or Dokku which are a couple that are recommended.

#Step 4: Parsing the data
- There are couple options I found online such as (Redis -https://redis.io/) and (Pudo - https://github.com/pudo/dataset)
- Ultimatley we have to create tables that can reflect the following:
  $ TICKER SYMBOL
  $ PRICE
  $ TIME STAMP

$Step 5: Building the bot
- This is where we can have fun. There are a couple basic scenarios we can start with for a technical bot:

++ Bare Minimum requirements for stock selection:
  - Market Cap: <$10,000,000
  - Average Trading Volume: <100,000
  - ?
++ TEST CASES
  - Test 1: BUY IF 20 SMA CROSSES OVER 50 SMA and SELL IF 20 SMA CROSSES UNDER 50 SMA
  - Test 2: BUY IF RSI FALL UNDER 25 and SELL IF RSI CROSSES OVER 75
  - Test 3: BUY IF STOCK IS WITHIN +/- 5% of 200 SMA and SELL IF... (need to look at this one)
  
