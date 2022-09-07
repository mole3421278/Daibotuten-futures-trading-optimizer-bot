# <p align="center">DAIBOTUTEN<br>(a futures trading optimizer bot)</p>
A bot to automatize the futures trading on Binance (twin of [Benzaiboten](https://github.com/mole3421278/Benzaiboten-spot-trading-bot))
# Warning: The bot does NOT ALWAYS guarantee a profit and in case of market crash you can lose ALL your funds
# DO NOT USE during Black Swan events...
# How does it work?
The bot finds the best cryptocurrencies to buy at each moment to resell them later. 

It uses an algorithm powered by AI to buy where an human would buy and at the same time trying to not stay with too much opened positions, so with it you don't have to worry about buying during the best moments.

It also shows to the user three indicators: 
- The fear and greed index of the current and previous day (lower values stand for fear and higher values stand for greed)
- The whale movements on chain
- The whale liquidations on the major exchanges (so to not be confused it with your own liquidations)

Use them to maximize the profit stopping and resuming the bot in the right times, following your own strategy.

There is also a display of the balance, with a percentage about the daily profit (each day the percentage is reset): please, remember that opening and closing a position costs a small trading fee (paid to the exchange, not to the developers of the bot), so it's normal if the balance decreases a little (we are talking about cents...) during those operations.
You can click on the open positions you have to be redirected to the webpage of the chart.

Finally, the bot will notice you if a new version is available for the download.

# Settings
The bot leaves a high margin of customization to the user, to fit different strategies: you can change the settings whenever you think the market has changed, so do your own research to maximize the returns from it.

You can also leave the bot with its own standard settings if you are a newbie.


| Command  | Description | Possible Values |
| ------------- | ------------- | ------------- |
| **LEVERAGE** | To choose the leverage to use: higher the leverage higher the risk to incur in a loss of funds, but also higher the potential profit. | From 3 to 10. It is recommended to stay at 10 only if, after doing your own research, you think the market is in a good shape. |
| **AMOUNT PER POSITION** | To choose how much to put at maximum in each position: in order to let the bot work well it is RECOMMENDED to have at LEAST 50 times the value you put here, so, if you choose 2 usdt it is RECOMMENDED that you have at least 100 usdt in the futures funds. However, it isn't a strict rule and so you can run the bot even with only 5 usdt (but don't expect that the bot will work well). | It depends on the leverage you use. The minimum value is 12/LEVERAGE, so, if you choose as leverage 10 you can choose 1.2 usdt or over. The maximum value is 20 usdt. |
| **STOP LOSS** | To decide when to close a position in case of loss. The bot has its own mechanism to take care of the potential loss, but you can overwrite it with this command. | It depends on the leverage you use. The minimum value is 0% and it stands for "don't use stop loss" and the maximum value is 75/LEVERAGE%, so, if you choose as leverage 10 you can choose till 7.5% as stop loss. |
| **TAKE PROFIT** | To decide when to close a position in case of profit. The bot has its own mechanism to take care of the potential profit, but you can overwrite it with this command. | The minimum value is 0% and it stands for "don't use take profit" and the maximum value is 30%. |
| **PROFITS TO SPOT** | To send a percentage of the profits of the closed positions to spot. It works only on the profits, so, for example, if you used 2 usdt to open a position and you get back 3 usdt when you close it, then the percentage is referred only to 3-2=1 usdt | The minimum value is 0% and the maximum value is 100%. |
| **PROTECTED BALANCE** | to specify a percentage of the current balance under which the bot won't buy anything till two consecutive whale's short liquidations occur and an hour pass since the last of them. When this happens, then the bot will resume automatically to buy again and the percentage will be referred to the new current balance | The minimum value is 0% and the maximum value is 100% (but putting it to 100% is the same as to stop the bot...). |
| **DON'T BUY IF BTC IS** | To force the bot to NOT buy ANYTHING if the price of BTC is over a certain threshold starting from the time in which it is set. | The minimum value is -10% and the maximum value is 10%. Put it to 0.0% to disable this behaviour. |
| **DON'T BUY IF ALT IS** | To force the bot to NOT buy the cryptocurrency if its price is over a certain threshold starting from the time in which it is set. | The minimum value is -30% and the maximum value is 30%. Put it to 0.0% to disable this behaviour. |
| **DON'T BUY FOR** | To force the bot to NOT buy the cryptocurrency for a certain interval of time | The minimum value is 0 hours and the maximum value is 12 hours. Put it to 0.0 hours to disable this behaviour. |
| **BUY IF CRASH OF** | To force the bot to buy ONLY IF in the last hour the price crashed from the maximum value to the current one of at least the percentage chosen | The minimum value is 0.0% hours and the maximum value is (-)15%. Put it to 0.0 to disable this behaviour. |
| **STOP AT NEXT WHALE LONG LIQUIDATION** | To stop the bot when there is a new whale long liquidation. The whale long liquidations can be seen in the bottom part of the bot, together with the whale short liquidations. | |
| **CLOSE** | To close a position just by clicking a button: the bot is set to close them in the moment that it is the best for it, but if you want to close them before that moment, you can do it. | |
| **BLACKLIST** | To exclude certain cryptocurrencies to be bought by the bot depending on your own research just by typing their ticker symbol (so BTC for bitcoin) and then pressing ENTER. | All the tickers allowable to be traded in the futures that you haven't yet blacklisted (for example: ETH, BTC...). You can type ALL to blacklist every crypto, to whitelist only the ones that you want. Don't type other things here. |
| **WHITELIST** | To add again to the list of the bot a cryptocurrency that you excluded before just by typing its ticker symbol and then pressing ENTER. | All the tickers that you have previously blacklisted. You can type ALL to whitelist every crypto. Don't type other things here. |
| **STOP/RESUME** | To stop the bot with this button if you believe the market is entering in a crash from buying other cryptocurrencies to resume it later, whenever you believe it's fine. | |

Some parameters are settable even from the file settings_bot.txt with the **expert mode** (wiki of the expert mode: https://github.com/mole3421278/Daibotuten-futures-trading-optimizer-bot/wiki/Expert-mode)

# Activation
The bot can't be used from not authorized users.

# Requirements

The bot runs entirely in local, so it is important that the device where you install it has a good internet connection, otherwise you can incur in misbehaviour.

<p align="center"><img src="https://user-images.githubusercontent.com/91144525/138165305-9f8b626d-adcd-4cc1-b290-1302562da61c.png" width="720"></p>
<p align="center"><img src="https://user-images.githubusercontent.com/91144525/138165376-6e57d3c8-7cdb-4b77-919f-3e58ac107463.png" width="720"></p>
<p align="center"><img src="https://user-images.githubusercontent.com/91144525/139111881-63c9804c-28a9-4c0f-97cf-7e3bac19ba3d.png" width="720"></p>




# Notes

The bot uses the Hedge Mode to trade. Set it going to binance futures --> preference --> position mode.

It can be that there are some minor bugs here and there. Please, do report them if you find them to improve the project.

If you have proposals to improve the project don't hesitate to post them.

For the moment it is in development a version for Windows.

In the future it will be expanded:
- to other exchanges;
- to other OS (first of all Android).

Please, use this repository to check for the updates.

If you intend to use also [Benzaiboten](https://github.com/mole3421278/Benzaiboten-spot-trading-bot) you don't have to pay for it separately: the dev fee to pay is the same, so for 10 usdt per month you can use both of them.

For some examples of strategies go to https://github.com/mole3421278/Daibotuten-futures-trading-optimizer-bot/wiki/Guide-of-the-bot

If you want, participate in the activation lottery from Nov-08-2021 08:00:00 AM UTC to Nov-15-2021 10:00:00 PM UTC activating the bot using the Fantom Network. More details in: https://mole.gitbook.io/fantom-activation-lottery/

# Latest release

https://github.com/mole3421278/Daibotuten-futures-trading-optimizer-bot/releases/latest
