# Blockchain Go Sample Project

This is a sample project demonstrating a basic implementation of a blockchain in Golang. **Note:** This project is not intended for production use.

## Features

- Create a blockchain
- Generate new wallet key-pairs
- Retrieve balances for addresses
- List all wallet addresses
- Print the entire blockchain
- Rebuild the UTXO set
- Send coins between addresses
- Start a mining node

## Build

To build the project, use the following command:

```bash
go build -o blockchain_go .
```

## Usage
After building the project, you can run the executable with the following commands:
```bash
./blockchain_go 
Usage:
  createblockchain -address ADDRESS - Create a blockchain and send genesis block reward to ADDRESS
  createwallet - Generates a new key-pair and saves it into the wallet file
  getbalance -address ADDRESS - Get balance of ADDRESS
  listaddresses - Lists all addresses from the wallet file
  printchain - Print all the blocks of the blockchain
  reindexutxo - Rebuilds the UTXO set
  send -from FROM -to TO -amount AMOUNT -mine - Send AMOUNT of coins from FROM address to TO. Mine on the same node, when -mine is set.
  startnode -miner ADDRESS - Start a node with ID specified in NODE_ID env. var. -miner enables mining
```
Disclaimer
This project is part of a great tutorial by Ivan Kuznetsov, which can be found [here](https://jeiwan.net/).