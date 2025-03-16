# Adding new token
The JSON schema for the tokens includes: address, name, decimals, symbol, logoURI, official homepage, MarketCap link, existing Markets.

Follow the steps below to add a new token：
1) Fork this repo.
2) change the JSON file `tokenlist.json`, adding such as: (PLEASE DO NOT REMOVE EXISITING TOKENS)
```
{
      "address": "TLmhyosmKNxuGwLHVcwZ8YEBFiV7atBU8m",
      "symbol": "DBT",
      "name": "DueBankToken",
      "decimals": 18,
      "logoURI": "https://ibb.co/h1cFYgBp",
      "homepage": "https://duebank.io/",
      "MarketCapLink": "https://coinmarketcap.com/currencies",
      "existingMarkets": [
          {
              "source": "sunswap",
              "pairs": [
                  "DBT/USDT",
                  "DBT/TRX",
                  
              ]
          },
          {
              "source": "DUEBANK",
              "pairs": [
                  "DBT/USDT"
              ]
          },
          {
              "source": "SUNSWAP",
              "pairs": [
                  "DBT/USDT"
              ]
          }
    ]
}
```
* `address`[Required]: your token address.
* `symbol`[Required]: your token symbol.
* `name`[Required]: your token name.
* `logoURI`[Required]: the logo URI of your token.
* `homepage`[Required]: the home page of your token.
* `MarketCapLink`[Optional]: the coinmarketcap or coingecko link for your token.
* `existingMarkets`[Required]: where to trade with your token.
3) Submit PR with the changed JSON file.


