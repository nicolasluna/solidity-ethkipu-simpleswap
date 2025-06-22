# 🌀 SimpleSwap Smart Contract

This project implements a simple decentralized token swap system inspired by Uniswap, written in Solidity.

It contains two main contracts:

- `CustomToken`: A basic ERC-20 token with minting functionality.
- `SimpleSwap`: A simple automated market maker (AMM) that supports:
  - Adding liquidity
  - Removing liquidity
  - Swapping tokens
  - Querying exchange price
  - Calculating output amount for swaps

---

## 📦 Contracts Overview

### 🪙 CustomToken

A standard ERC-20 token contract that allows public minting.

#### Functions

- `constructor(string memory name, string memory symbol)`
  - Deploys a token with the given name and symbol.
- `mint(address to, uint256 amount)`
  - Mints `amount` tokens to the `to` address.

---

### 🔁 SimpleSwap

A basic AMM liquidity pool for two ERC-20 tokens. It allows users to provide liquidity and perform token swaps.

#### Constructor

```solidity
constructor(address _tokenA, address _tokenB)

