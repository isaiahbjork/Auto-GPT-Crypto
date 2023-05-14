# Auto-GPT Crypto Plugin 📈

⚠️ WARNING: NOT 100% COMPLETE

The AutoGPT Crypto Plugin is a software tool that enables traders to connect their Crypto wallet or exchange to Auto-GPT.


[![GitHub Repo stars](https://img.shields.io/github/stars/isaiahbjork/Auto-GPT-Crypto-Plugin?style=social)](https://github.com/isaiahbjork/Auto-GPT-Crypto-Plugin/stargazers)

<h2 align="center"> 💖 Help Support Auto-GPT Plugin's Development 💖</h2>
<p align="center">
If you can spare a coffee, you can help to cover the costs of developing Auto-GPT Plugins and help to push the boundaries of fully autonomous AI!
Your support is greatly appreciated. Development of this free, open-source project is made possible by all the <a href="https://github.com/isaiahbjork/Auto-GPT-Crypto-Plugin/graphs/contributors">contributors</a> and <a href="https://github.com/sponsors/isaiahbjork">sponsors</a>. If you'd like to sponsor this project and have your avatar or company logo appear below <a href="https://github.com/sponsors/isaiahbjork">click here</a>.

Crypto Donations: 0x2457e8746EFa5894b70aE06a1b391474bc928B05
</p>

## 💡 Key Features:
- **Get ETH Balance**
- **Get Wallet Token Holdings**
- **Get Wallet NFT Holdings**
- **Get Coin/NFT of The Day**
- **Create Wallet**
- **Send ETH & MATIC**
- **Get New Tokens From Dextools**
- **Telegram Crypto Groups Listener**
- **NFT Metadata**
- **Transaction Data**
- **Signals (Pivot Points, Moving Averages, Technical Indicators)**
- **CoinMarketCap Airdrops**
- **Currency Convertor**
- **Recent Crypto Social Feed**
## 🔜 Upcoming:
- **Stake Tokens** (In-Progress)
- **Swap Tokens**  (In-Progress)
- **Send Tokens**  (In-Progress)
- **Purchase NFT**  (In-Progress)
- **Trade on Exchanges**  (In-Progress)
- **Crypto News**  (In-Progress)
- **Indicators**  (In-Progress)
- **Fetch Candlesticks**  (In-Progress)
- **Search Top Holders**  (In-Progress)
- **Get Coins By Market Cap**  (In-Progress)
- **Get Crypto Influencers**  (In-Progress)


**Blockchains**
- ETH
- BSC
- Fantom
- Avalanche
- Polygon
- Arbitrum
- Syscoin
- Optimism
## 🔧 Installation

Follow these steps to configure the Auto-GPT Crypto Plugin:

### 1. Clone the Auto-GPT-Crypto-Plugin repository

Clone this repository and navigate to the `Auto-GPT-Crypto-Plugin` folder in your terminal:

```bash
git clone https://github.com/isaiahbjork/Auto-GPT-Crypto-Plugin.git
```

### 2. Install required dependencies

Execute the following command to install the necessary dependencies:

```bash
pip install -r requirements.txt
```

### 3. Package the plugin as a Zip file

Compress the `Auto-GPT-Crypto-Plugin` folder or [download the repository as a zip file](https://github.com/isaiahbjork/Auto-GPT-Crypto-Plugin/archive/refs/heads/master.zip).

### 4. Install Auto-GPT

If you haven't already, clone the [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT) repository, follow its installation instructions, and navigate to the `Auto-GPT` folder.

You might have to run this in the Auto-GPT file if you get an error saying "No Moudle Found".

```bash
pip install web3 eth-account eth-abi ccxt telethon uniswap-python
```

### 5. Copy the Zip file into the Auto-GPT Plugin folder

Transfer the zip file from step 3 into the `plugins` subfolder within the `Auto-GPT` repo.

### 6. Locate the `.env.template` file

Find the file named `.env.template` in the main `/Auto-GPT` folder.

### 7. Create and rename a copy of the file

Duplicate the `.env.template` file and rename the copy to `.env` inside the `/Auto-GPT` folder.

### 8. Edit the `.env` file

Open the `.env` file in a text editor. Note: Files starting with a dot might be hidden by your operating system.

### 9. Add Crypto configuration settings

Append the following configuration settings to the end of the file:

```ini
################################################################################
### CRYPTO
################################################################################
ETHERSCAN_API_KEY=
POLYSCAN_API_KEY=
ETH_WALLET_ADDRESS=
ETH_WALLET_PRIVATE_KEY=
LUNAR_CRUSH_API_KEY=
TELEGRAM_API_ID=
TELEGRAM_API_HASH=
FCS_API_KEY=
CMC_API_KEY=
### Exchanges
EXCHANGES=
EXCHANGE_NAME_SECRET=
EXCHANGE_NAME_API_KEY=
```
- Create a [Etherscan](https://etherscan.io) account.
- Create a [Polyscan](https://polyscan.io) account.
- Create a [LunarCrush](https://lunarcrush.com) account.
- Create a [FCS](https://fcsapi.com) account.
- Create a [CoinMarketCap](https://coinmarketcap.com/api/) account.
- Set `INFURA_API_KEY` to your Infura account ID.
- Set `ETHERSCAN_API_KEY` to your Etherscan API Key.
- Set `LUNARCRUSH_API_KEY` to your LunarCrush API Key.
- Set `FCS_API_KEY` to your FCS API Key.
- Set `CMC_API_KEY` to your CoinMarketCap API Key.
- Set `ETH_WALLET_ADDRESS` to your Ethereum Wallet Address.
- Set `ETH_WALLET_PRIVATE_KEY` to your Ethereum mnemonic.
- Set `EXCHANGES` to the crypto exchanges where you have an account. Review available [exchanges](/src/auto_gpt_crypto/exchanges.txt). (Example: binance,kraken,bybit)
- Set `EXCHANGE_NAME_API_KEY` to your Exchange API Key. (Must be capital letters.)
- Set `EXCHANGE_NAME_SECRET` to your Exchange Secret. (Must be capital letters.)

`Telegram Group Listener Setup`
1. Create a [Telegram](https://telegram.com) account.
2. Go to [https://my.telegram.org/auth](https://my.telegram.org/auth).
3. Login and create an application.
4. Set `TELEGRAM_API_ID` to your Telegram App ID.
5. Set `TELEGRAM_API_HASH` to your Telegram App Hash.
6. Join this [Telegram Group](https://t.me/DEXTNewPairsBot).
7. You will be prompted to enter your phone number and code when you start up Auto-GPT. Make sure you enter your country code without the (+).
8. You will get an error if you don't enter "n".
```
WARNNG Plugin TelegramClient found. But not in the allowlist... Load? (y/n): n
```
### 10. Allowlist Plugin

In your `.env` search for `ALLOWLISTED_PLUGINS` and add this Plugin:

```ini
################################################################################
### ALLOWLISTED PLUGINS
################################################################################
#ALLOWLISTED_PLUGINS - Sets the listed plugins that are allowed (Example: plugin1,plugin2,plugin3)
ALLOWLISTED_PLUGINS=AutoGPTCryptoPlugin
```

### 11. Review Available Commands
You can review the available commands [here](/src/auto_gpt_crypto/commands.txt).

## 🧪 Test the Auto-GPT Crypto Plugin

Experience the plugin's capabilities by testing it for
