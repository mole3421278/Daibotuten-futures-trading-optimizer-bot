# Optimizer-Futures-Trader-Bot
A bot to automatize the futures trading on Binance
# Warning: The bot DOESN'T guarantee ALWAYS a profit and in case of market crash you can lose ALL your funds
# How does it work?
The bot finds the best cryptocurrencies to buy at each moment to resell them later. 

It uses an algorithm powered by AI to buy where an human would buy and at the same time trying to not stay with too much opened positions, so with it you don't have to worry about buying during the best moments.
# Settings
The bot leaves a high margin of customization to the user, to fit different strategies: you can change the settings whenever you think the market has changed, so do your own research to maximize the returns from it.

LEVERAGE

You can choose the leverage to use: higher the leverage higher the risk to incur in a loss of funds, but also higher the potential profit. 

Possible values: from 3 to 10. It is recommended to stay at 10 only if, after doing your own research, you think the market is in a good shape.

AMOUNT PER POSITION

You can choose how much to put at maximum in each position: in order to let the bot work well it is RECOMMENDED to have at LEAST 50 times the value you put here, so, if you choose 2 usdt it is RECOMMENDED that you have at least 100 usdt in the futures funds. However, it isn't a strict rule and so you can run the bot even with only 5 usdt (but don't expect that the bot will work well).

Possible values: it depends on the leverage you use. The minimum value is 12/LEVERAGE, so, if you choose as leverage 10 you can choose 1.2 usdt or over. The maximum value is 100 usdt

CLOSE

You can choose to close a position just by clicking a button: the bot is set to close them in the moment that it is the best for it, but if you want to close them before that moment, you can do it.

EXCLUDE

You can choose to exclude certain cryptocurrencies to be bought by the bot depending on your own research just by typing their ticker symbol (so BTC for bitcoin) on clicking on the button EXCLUDE.

INCLUDE

If you excluded a cryptocurrency, you can readd it to the list of the bot just by typing its ticker symbol and clicking on the button INCLUDE.

STOP

If you believe the market is entering in a crash you can stop the bot from buying other cryptocurrencies to resume it later, whenever you believe it's fine.

# Activation
To start the bot the first time you need to link it to an API key.
To create the API key go to https://www.binance.com/en/my/settings/api-management and be sure that the API key has a tick on: 
- Enable Futures


# Devs Fee
There is a fee of 5 usdt to activate the bot.

There is a fee of 10 usdt monthly to run the bot.

The fees must be paid manually directly by the user because the bot does NOT have the ability to withdraw funds (to be able to withdraw funds, the API key must have a tick on Enable Withdrawals, but, as written before, the bot doesn't require to have it).

If the fees are not paid the bot simply doesn't work. If, passed some months, you want to use again the bot, you have only to pay the monthly fee.

