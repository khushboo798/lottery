# lottery
# Savings Vault Smart Contract

## Overview

The **Savings Vault** smart contract allows users to deposit and withdraw ETH securely. Each user’s balance is tracked, and only the contract owner can withdraw the total contract balance. The contract ensures that deposits are safe and that users can withdraw only the amount they’ve deposited.

### Key Features:
- Users can deposit ETH into the contract.
- Users can withdraw their ETH balances at any time.
- Only the owner can withdraw the contract’s total balance.
- The contract logs each deposit and withdrawal event.
- The contract provides functions to view balances and check the contract's balance.

## Table of Contents
- [Contract Details](#contract-details)
- [Deployment Instructions](#deployment-instructions)
- [Usage Instructions](#usage-instructions)
- [View Functions](#view-functions)
- [Contract Address](#contract-address)
- [License](#license)

## Contract Details

### Key Functions:
- `deposit()`: Allows users to deposit ETH into the vault.
- `withdraw(uint256 amount)`: Allows users to withdraw ETH from the vault.
- `ownerWithdraw(uint256 amount)`: Allows the owner to withdraw the total ETH balance from the contract.
- `getContractBalance()`: Allows anyone to check the total balance of the contract.
- `getUserBalance(address user)`: Allows users to check their balance in the vault.

### Events:
- `Deposited(address indexed user, uint256 amount)`: Emitted when a user deposits ETH.
- `Withdrawn(address indexed user, uint256 amount)`: Emitted when a user withdraws ETH.

## Deployment Instructions

### Prerequisites:
- [Node.js](https://nodejs.org/) installed
- [Truffle](https://www.trufflesuite.com/truffle) or [Hardhat](https://hardhat.org/)
