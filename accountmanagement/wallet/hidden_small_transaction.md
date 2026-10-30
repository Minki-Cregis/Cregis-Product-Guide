# 隐藏小额交易说明

## 1. 功能说明

隐藏小额交易功能用于减少交易记录列表中的小额交易展示，帮助用户更清晰地查看主要交易记录。该功能按照代币及对应网络配置隐藏阈值，并根据交易记录中的交易金额进行判断是否隐藏。

## 2. 隐藏规则

当一笔交易记录的交易金额小于或等于该代币在对应网络下配置的隐藏阈值时，该交易记录将在客户端交易记录列表中隐藏；当交易金额大于隐藏阈值时，该记录正常显示。隐藏阈值以代币数量为单位，不是按美元、人民币等法币价值折算。该功能仅影响客户端交易记录的展示，不代表链上交易被删除、撤销或未发生。

## **3. 各代币隐藏阈值明细**

| 链名称                       | 代币名称       | 隐藏阈值     |
| ------------------------- | ---------- | -------- |
| Bitcoin                   | BTC        | 0.00001  |
| Dogecoin                  | DOGE       | 0.001    |
| BitcoinCash               | BCH        | 0.00001  |
| Ethereum Classic          | ETC        | 0.00001  |
| Ripple                    | XRP        | 0.00001  |
| Litecoin                  | LTC        | 0.00001  |
| DAI                       | DAI        | 0.00001  |
| FileCoin Mainnet          | FIL        | 0.00001  |
| SUI                       | SUI        | 0.00001  |
| Cardano                   | ADA        | 0.84907  |
| Aptos                     | APT        | 0.00001  |
| Sei                       | SEI        | 0.000001 |
| Ethereum                  | ETH        | 0.00001  |
| Ethereum                  | USDT       | 0.00001  |
| Ethereum                  | USDC       | 0.00001  |
| Ethereum                  | FET        | 0.00001  |
| Ethereum                  | PEPE       | 0.00001  |
| Ethereum                  | 1INCH      | 0.00001  |
| Ethereum                  | AAVE       | 0.00001  |
| Ethereum                  | CHZ        | 0.00001  |
| Ethereum                  | COMP       | 0.00001  |
| Ethereum                  | CRV        | 0.00001  |
| Ethereum                  | MANA       | 0.00001  |
| Ethereum                  | DYDX       | 0.00001  |
| Ethereum                  | ENS        | 0.00001  |
| Ethereum                  | GALA       | 0.00001  |
| Ethereum                  | MKR        | 0.00001  |
| Ethereum                  | OKB        | 0.00001  |
| Ethereum                  | STORJ      | 0.00001  |
| Ethereum                  | SUSHI      | 0.00001  |
| Ethereum                  | SAND       | 0.00001  |
| Ethereum                  | WBTC       | 0.00001  |
| Ethereum                  | WETH       | 0.00001  |
| Ethereum                  | YFI        | 0.00001  |
| Ethereum                  | CAKE       | 0.00001  |
| Ethereum                  | POL        | 0.00001  |
| Ethereum                  | cbBTC      | 0.00001  |
| Ethereum                  | CHR        | 0.00001  |
| Ethereum                  | PEOPLE     | 0.00001  |
| Ethereum                  | ENA        | 0.00001  |
| Ethereum                  | MX         | 0.00001  |
| Ethereum                  | BGB        | 0.00001  |
| Ethereum                  | YGG        | 0.00001  |
| Ethereum                  | CRO        | 0.00001  |
| Ethereum                  | BUSD       | 0.00001  |
| Ethereum                  | WXRP       | 0.00001  |
| Ethereum                  | ETHFI      | 0.00001  |
| Ethereum                  | aEthUSDT   | 0.00001  |
| Ethereum                  | JASMY      | 0.00001  |
| Ethereum                  | XCN        | 0.00001  |
| Ethereum                  | Ondo       | 0.00001  |
| Ethereum                  | WUSD       | 0.00001  |
| Ethereum                  | DAI        | 0.00001  |
| Ethereum                  | stETH      | 0.00001  |
| Ethereum                  | cbETH      | 0.00001  |
| Ethereum                  | MOVE       | 0.00001  |
| Ethereum                  | TURBO      | 0.00001  |
| Ethereum                  | Neiro      | 0.00001  |
| Ethereum                  | XYO        | 0.00001  |
| Ethereum                  | VRA        | 0.00001  |
| Ethereum                  | SOLVE      | 0.00001  |
| Ethereum                  | ANKR       | 0.00001  |
| Ethereum                  | FTM        | 0.00001  |
| Ethereum                  | AXS        | 0.00001  |
| Ethereum                  | AMP        | 0.00001  |
| Ethereum                  | KLCC       | 0.00001  |
| Ethereum                  | BBTC       | 0.00001  |
| Ethereum                  | PYUSD      | 0.00001  |
| Ethereum                  | STRK       | 0.00001  |
| Ethereum                  | MATIC      | 0.00001  |
| Ethereum                  | UNI        | 0.00001  |
| Ethereum                  | LINK       | 0.00001  |
| Ethereum                  | SHIB       | 0.00001  |
| Ethereum                  | AIX        | 0.00001  |
| BNB Smart Chain           | BNB        | 0.000001 |
| BNB Smart Chain           | USDT       | 0.001    |
| BNB Smart Chain           | MIX        | 0.00001  |
| BNB Smart Chain           | CDN        | 0.00001  |
| BNB Smart Chain           | CDN2       | 0.00001  |
| BNB Smart Chain           | DAO9       | 0.00001  |
| BNB Smart Chain           | TOK        | 0.00001  |
| BNB Smart Chain           | BABYLONG   | 0.00001  |
| BNB Smart Chain           | SINSO      | 0.00001  |
| BNB Smart Chain           | SAI        | 0.00001  |
| BNB Smart Chain           | SYNX       | 0.00001  |
| BNB Smart Chain           | AIX        | 0.00001  |
| BNB Smart Chain           | Marosca    | 0.00001  |
| BNB Smart Chain           | YTA        | 0.00001  |
| BNB Smart Chain           | DORA       | 0.00001  |
| BNB Smart Chain           | WETH       | 0.00001  |
| BNB Smart Chain           | BTCB       | 0.00001  |
| BNB Smart Chain           | XRP        | 0.00001  |
| BNB Smart Chain           | SBT        | 0.00001  |
| BNB Smart Chain           | KOMA       | 0.00001  |
| BNB Smart Chain           | BabyDoge   | 0.00001  |
| BNB Smart Chain           | Cheems     | 0.00001  |
| BNB Smart Chain           | DOGE       | 0.00001  |
| BNB Smart Chain           | BCH        | 0.001    |
| BNB Smart Chain           | ETC        | 0.001    |
| BNB Smart Chain           | NEAR       | 0.001    |
| BNB Smart Chain           | FET        | 0.001    |
| BNB Smart Chain           | 1INCH      | 0.001    |
| BNB Smart Chain           | LINK       | 0.001    |
| BNB Smart Chain           | CAKE       | 0.001    |
| BNB Smart Chain           | SUSHI      | 0.001    |
| BNB Smart Chain           | SHIB       | 0.001    |
| BNB Smart Chain           | UNI        | 0.001    |
| BNB Smart Chain           | AAVE       | 0.001    |
| BNB Smart Chain           | COMP       | 0.001    |
| BNB Smart Chain           | MKR        | 0.001    |
| BNB Smart Chain           | COW        | 0.00001  |
| BNB Smart Chain           | FROG       | 0.00001  |
| BNB Smart Chain           | ADA        | 0.00001  |
| BNB Smart Chain           | AIXT       | 0.00001  |
| BNB Smart Chain           | RAY        | 0.00001  |
| BNB Smart Chain           | BOB        | 0.00001  |
| BNB Smart Chain           | Worker     | 0.00001  |
| BNB Smart Chain           | PPT        | 0.00001  |
| BNB Smart Chain           | TST        | 0.00001  |
| BNB Smart Chain           | XLM        | 0.00001  |
| BNB Smart Chain           | C3Coin     | 0.00001  |
| BNB Smart Chain           | WSC        | 0.00001  |
| BNB Smart Chain           | WSC2       | 0.00001  |
| BNB Smart Chain           | WSCPoint   | 0.00001  |
| BNB Smart Chain           | M1         | 0.00001  |
| BNB Smart Chain           | WSC3       | 0.00001  |
| BNB Smart Chain           | WXZ        | 0.00001  |
| BNB Smart Chain           | LP         | 0.00001  |
| BNB Smart Chain           | TOAD       | 0.00001  |
| BNB Smart Chain           | GVC        | 0.00001  |
| BNB Smart Chain           | USDC       | 0.00001  |
| BNB Smart Chain           | BOTss      | 0.00001  |
| BNB Smart Chain           | PIKA       | 0.00001  |
| BNB Smart Chain           | DOT        | 0.00001  |
| BNB Smart Chain           | Mubarak    | 0.00001  |
| BNB Smart Chain           | AXT        | 0.00001  |
| Polygon                   | POL        | 0.001    |
| Polygon                   | USDT       | 0.001    |
| Polygon                   | AAC        | 0.00001  |
| Polygon                   | APPLE      | 0.00001  |
| Polygon                   | iNFTspace  | 0.00001  |
| Polygon                   | BGG        | 0.00001  |
| Polygon                   | USDC       | 0.00001  |
| Polygon                   | USDC       | 0.00001  |
| Polygon                   | DAI        | 0.00001  |
| Polygon                   | WUSD       | 0.00001  |
| Base                      | ETH        | 0.00001  |
| Base                      | USDC       | 0.00001  |
| Base                      | USDT       | 0.00001  |
| Base                      | XRP        | 0.00001  |
| Base                      | SEAM       | 0.00001  |
| Base                      | cbBTC      | 0.00001  |
| Tron                      | TRX        | 0.001    |
| Tron                      | USDT       | 0.00001  |
| Tron                      | USDC       | 0.00001  |
| Tron                      | USDJ       | 0.00001  |
| Tron                      | KLCC       | 0.00001  |
| Tron                      | SFE        | 0.00001  |
| Solana                    | SOL        | 0.00001  |
| Solana                    | USDT       | 0.00001  |
| Solana                    | USDC       | 0.00001  |
| Solana                    | TJRM       | 0.00001  |
| Solana                    | UTKD       | 0.00001  |
| Solana                    | UTK        | 0.00001  |
| Solana                    | WuKong     | 0.00001  |
| Solana                    | LUCE       | 0.00001  |
| Solana                    | MELANIA    | 0.00001  |
| Solana                    | WINH       | 0.00001  |
| Solana                    | BLAS       | 0.00001  |
| Optimism                  | ETH        | 0.00001  |
| Optimism                  | USDT       | 0.00001  |
| Optimism                  | USDC       | 0.00001  |
| Optimism                  | OptimismOP | 0.00001  |
| Optimism OP Stack BNB BSC | BNB        | 0.001    |
| Optimism OP Stack BNB BSC | USDT       | 0.00001  |
| Arbitrum                  | ETH        | 0.00001  |
| Arbitrum                  | USDT       | 0.00001  |
| Arbitrum                  | USDC       | 0.00001  |
| Avalanche                 | AVAX       | 0.00001  |
| Avalanche                 | USDT       | 0.00001  |
| Avalanche                 | USDC       | 0.00001  |
| Ton                       | TON        | 0.00001  |
| Ton                       | USDT       | 0.00001  |
| CETUS                     | CETUS      | 0.00001  |
| WAL                       | WAL        | 0.00001  |
| DEEP                      | DEEP       | 0.00001  |
| HIPPO                     | HIPPO      | 0.00001  |
| USDC Token                | USDC       | 0.00001  |
| EVER                      | EVE        | 0.001    |
| GDSToken                  | TRX        | 0.00001  |
| RENDER                    | RENDER     | 0.00001  |
| MEMEFI                    | MEMEFI     | 0.00001  |
