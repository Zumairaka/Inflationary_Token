# CinemaDraft Token Contract

CinemaDraft token contract is a reflection token contract that used IBEP20 interface and Reflect.finance reflection mechanism. The contract code is inspired from Safemoon contract and has made the necessary modifications to make the tokenomics easier to chage, make the code easier to maintain and fix some of the issues reported in the Safemoon audit.

# EasyAuction Contract

EasyAuction should become a platform to execute batch auctions for fair initial offerings and token buyback programs. Batch auctions are a market mechanism for matching limit orders of buyers and sellers of a particular good with one fair clearing price.
Already in traditional finance, batch auctions have established themselves as a tool for initial offerings, and in the blockchain ecosystem, they are expected to become a fundamental DeFi building lego brick for price-discovery as well.
The EasyAuction platform is inspired by the auction mechanism of the Gnosis Protocol v1, which has shown a significant product-market fit for initial dex offerings (IDOs) (cp. sales of DIA, mStable, etc…). EasyAuction improves significantly the user experience for IDOs, by settling up arbitrary many bids with a single clearing price instead of roughly 28 orders and thereby making the mechanism fairer, easier to use, and more predictable.
Given the emerging regulations for IDOs and utility sales - see MiCA -, EasyAuction is intending to comply with them and enabling new projects a safe start without legal risks.

## Instructions

Install dependencies

```
npm install
```

Running tests

```
npx hardhat test
```

Deploy

For deployment, paste your keys and other details as mentioned below in a dotenv.
```
GAS_PRICE_GWEI = 30000
INFURA_KEY = "write your infura key"
MNEMONIC = 12 word recovery phrase
MY_ETHERSCAN_API_KEY = 
PK = private key 
To deploy on the BSC mainnet, write "binancesmartchain" in place of $NETWORK.
```

```
npx hardhat run scripts/sample-script.js --network $NETWORK

```
