# interactive-smart-contract

Create a .env file in the root folder with the following variables:

- ETHEREUM_NETWORK = "sepolia"
- INFURA_API_KEY = "https://sepolia.infura.io/v3/<API-KEY\>" (for details: https://docs.infura.io/infura/networks/ethereum/how-to/choose-a-network)
- MNEMONIC = "\<YOUR-MNEMONIC\>"
- SIGNER_PRIVATE_KEY = "\<Private-Key\>"

Use `npx truffle migrate --network sepolia` to migrate the smart contract into the sepolia network

Look for the address of the migrated smart contract in the console output and add it into your .env file.

- DEMO_CONTRACT = "0x..." (address of the smart contract)

Afterwards you can use `node .\call.js` to call your smart contract.

Note: Currently I am facing `Error: Invalid JSON RPC response: {"size":0,"timeout":0}`. Maybe it will work for you..
