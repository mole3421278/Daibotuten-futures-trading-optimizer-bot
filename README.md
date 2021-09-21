# Optimizer-Futures-Trader-Bot
A bot to automatize the futures trading on Binance
# Warning: The bot DOESN'T guarantee ALWAYS a profit and in case of market crash you can lose ALL your funds
# How does it work?
The bot finds the best cryptocurrencies to buy at each moment to resell them later.
# Settings
The bot leaves a high margin of customization to the user, to fit different strategies: you can change the settings whenever you think the market has changed, so do your own research to maximize the returns from it.

LEVERAGE

You can choose the leverage to use: higher the leverage higher the risk to incur in a loss of funds, but also higher the potential profit. (Possible values: from 3 to 15, however it is recommended to stay maximum around 10, at least you are really sure that we are in a bull run)

AMOUNT PER POSITION

You can choose how much to put at maximum in each position: in order to let the bot work well you need to have at least 50 times the value you put here, so, if you choose 2 usdt you must have at least 100 usdt in the futures funds. (Possible values: it depends on the leverage you use. The minimum value is 15/LEVERAGE, so, if you choose as leverage 10 you can choose 1.5 usdt or over. There isn't a maximum value)

CLOSE

You can choose to close the position just by clicking a button: the bot is set to close them in the moment that it is the best for it, but if you want to close them before that moment, you can do it.

EXCLUDE

You can choose to exclude certain cryptocurrencies to be bought by the bot depending on your own research just by typing their ticker symbol (so BTC for bitcoin) on clicking on the button EXCLUDE.

INCLUDE

If you excluded a cryptocurrency, you can readd it to the list of the bot just by typing its ticker symbol and clicking on the button INCLUDE.

STOP

If you believe the market is entering in a crash you can stop the bot from buying other cryptocurrencies to reactivate it later, whenever you believe it's fine.

# Activation
To start the bot you need to link it to an API key.
To create the API key go to https://www.binance.com/en/my/settings/api-management and be sure that the API key has a tick on: 
- Enable Spot & Margin Trading
- Enable Futures
- Enable Withdrawals

Be also sure that you have some Matic and Fantom in the spot, because they are used as devs fee.

# Devs Fee
There is a fee of 5 Matic or 5 Fantom to activate the bot.
There is a fee of AMOUNT PER POSITION*LEVERAGE*0.05 Matic or Fantom each day or each time the bot is started (if you stop the bot clicking on the button and then restart it you don't incur on the fee, but if you stop the bot closing the app and then reopening it yes), so for example with 1.5 as AMOUNT PER POSITION and 10 as LEVERAGE you have a fee of 0.75 Matic or Fantom.
You can choose if to use Matic or Fantom, but if the blockchain of one of them is under maintenance you have to choose the other one or wait before to use again the bot.
