# Simple Multi-Sig Wallet

This repository contains a high-quality, flat-structured implementation of a Multi-Signature (Multi-Sig) wallet. It is designed for teams or individuals who want to secure their assets by requiring more than one person to authorize a transaction.

## Features
* **Threshold Security:** Set a specific number of required signatures (e.g., 2-of-3).
* **Transaction Proposal:** Any owner can propose a transfer.
* **Approval Flow:** Other owners can view and approve pending transactions.
* **Execution Logic:** Only executes once the required confirmation threshold is met.

## Getting Started
1. Open [Remix IDE](https://remix.ethereum.org/).
2. Deploy `MultiSigWallet.sol` providing a list of owner addresses and the required number of confirmations.
3. Use `submitTransaction` to propose a transfer.
4. Other owners call `confirmTransaction` using the transaction index.
5. Once the threshold is reached, anyone can call `executeTransaction`.

## License
MIT
