[![build status](https://github.com/jsappme/node-binance-trader/workflows/CI/badge.svg)](https://github.com/jsappme/node-binance-trader/actions?query=workflow%3ACI "build status")
[![Donate NIM](https://www.nimiq.com/accept-donations/img/donationBtnImg/light-blue-small.svg)](https://wallet.nimiq.com/nimiq:NQ38SDPGREC3USTALLCT87GQTCUYFH5L6PCQ)

<h1 align="center">Node Binance Trader NBT</h1>

<h4 align="center">NBT is a Cryptocurrency Trading Strategy & Portfolio Management Development Framework for <a href='https://www.binance.com/en/register?ref=CRQ7Y5TF' target="_new">Binance</a>.</h4>

## Table of contents

1. **[Documentation 📖](#documentation)**
1. **[Technical overview 👨‍💻](#technical-overview)**
1. **[Disclaimer 📖](#disclaimer)**
1. **[Donate 🙏](#donate)**
1. **[Getting in touch 💬](#getting-in-touch)**
1. **[Final Notes](#final-notes)**

## Documentation

- **[Quick start guide 🚀](./docs/GETTING-STARTED.md)**: bootstrap using Heroku
- **[Manual setup guide 👨‍💻](./docs/GETTING-STARTED-MANUALLY.md)**: bootstrap using your own client
- **[Web socket API specification 📡](./docs/WEB-SOCKET-API-SPECIFICATION.md)**

## Technical overview

<img src="docs/images/nbt_diagram.png">

NBT includes 3 main JS scripts:

* the **server**:

  * to track a selection of asset pairs and record all [Binance](https://www.binance.com/en/register?ref=CRQ7Y5TF) api data (candles, depths, trades) into a Postgres database.
  * to detect buy or sell signals
  * (optional) to send trading signals to the NBT Hub / [Bitcoin vs. Altcoins](https://bitcoinvsaltcoins.com) to monitor performances and auto trade those signals (virtually or for real).

* the **trader**: [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/jsappme/node-binance-trader)

  * this script allows you to auto trade the signals received from the NBT hub or your own server. this script can run locally or on cloud services like Heroku. This new auto trader script allows you to trade with leverage when the pair is available for margin trading.

* the **backtest** :

  * to backtest your strategies on the historical tick data (Postgres database) recorded by the server.

## Disclaimer

> No owner or contributor is responsible for anything done with this bot.
> You use it at your own risk.
> There are no warranties or guarantees expressed or implied.
> You assume all responsibility and liability.

## Binance Account - Get 10% discount on fees!

Don't you have a **Binance** account yet?  
Register using the **referal link** below and get a **10% discount on fees** for **all** your trades!

[**https://accounts.binance.com/en/register?ref=IMNOXVUY**](https://accounts.binance.com/en/register?ref=IMNOXVUY)  


## Enjoy - Donate - Buy me a beer!  =]

Thank you for using Binance to Google Sheets add-on!  
I really hope you enjoyed and loved it as much as I love to use it everyday.

If your love is strong enough, feel free to share it with me!  =D  
I will much appreciate any contribution and support to keep working on it.  
I have several ideas for new features, so much more could come!

You can send any token through the **Binance Smart Chain** (BSC/BEP20) to the address:  
`0x51CeC0bB36BacC9765e1A5fa67b84810DeF607Ae`
---

## Final Notes

Feel free to fork and add new pull request to this repo.
If you have any questions/suggestions, or simply you need some help building your trading bot, or mining historical data or improving your strategies using the latest AI/ML algorithms, please feel free to <a href="mailto:herve76@gmail.com" target="_blank">contact me</a>.
