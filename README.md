# Lunar Path (Built for Base)

Lunar Path is a lightweight, read-only tool created to inspect and validate Base Sepolia. It helps developers quickly verify network status, check wallet balances, and validate testnet contract deployments.

---

## Key Features

Lunar Path allows you to:
- Verify your connection to Base Sepolia (chainId: 84532)  
- Check wallet balances and transaction details  
- Inspect deployed contracts on the testnet  
- Access direct explorer links for verification  

All actions are read-only, ensuring no changes to the blockchain.

---

## Repository Structure

- **app/lunar-path.ts**  
  The core script that connects to Coinbase Wallet and queries Base Sepolia RPC for onchain data.

- **contracts/**  
  Solidity contracts deployed on Base Sepolia for testnet validation:
  - `control.sol` — A minimal deployment contract  
  - `arrays.sol` — A contract that accesses data by index

- **package.json**  
  Dependency management for this project.

---

## How It Works

Lunar Path connects to Coinbase Wallet using the Coinbase Wallet SDK and queries the Base Sepolia network using viem. It retrieves public blockchain data like balances, transaction counts, block details, and gas prices, providing explorer links for verification.

No transactions are signed or broadcast.

---

## License

MIT License  
Copyright (c) 2025 YOUR_NAME

---

## Author

GitHub: [musks-suburbs](https://github.com/musks-suburbs)  

Email: 01_musks.suburbs@icloud.com

---

## Testnet Deployment (Base Sepolia)

These contracts were deployed on Base Sepolia for testing and validation.

Network: Base Sepolia  
chainId (decimal): 84532  
Explorer: [sepolia.basescan.org](https://sepolia.basescan.org)

Contract control.sol address:  
0x56192825Dc8dCC01e2956d9cbEbd94891086423C

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0x56192825Dc8dCC01e2956d9cbEbd94891086423C)
- [Code Verification](https://sepolia.basescan.org/0x56192825Dc8dCC01e2956d9cbEbd94891086423C/0#code)

Contract arrays.sol address:  
0x9225F320298e940Ea1B7305c8eABb63e3261309d

Deployment and verification:
- [Deployment Link](https://sepolia.basescan.org/address/0x9225F320298e940Ea1B7305c8eABb63e3261309d)
- [Code Verification](https://sepolia.basescan.org/0x9225F320298e940Ea1B7305c8eABb63e3261309d/0#code)

These testnet deployments are used to ensure that the network and Base tooling work as expected.
