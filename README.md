# zk-Paymaster

**Connecting zkSync Native Account Abstraction with Chainlink Price Feeds**

## Overview

This project introduces a zkSync Paymaster that seamlessly integrates zkSync's native account abstraction with the security and convenience of Chainlink Price Feeds.

## Functionality

The Paymaster allows users to pay gas fees using their preferred ERC20 tokens instead of the network's native cryptocurrency. Leveraging zkSync’s account abstraction and Chainlink’s price feeds on the zkSync Era Sepolia testnet, the Paymaster converts gas fees from ETH into ERC20 tokens like LINK or USDC.

## Problem Addressed

Traditional blockchains typically require gas fees to be paid in the network’s native cryptocurrency (e.g., ETH on Ethereum). This creates several challenges:

1. **User Inconvenience**: Users who primarily hold and use ERC20 tokens must also manage ETH for gas fees, complicating their experience.
   
2. **Barrier to Entry**: New users may be discouraged by the need to acquire and manage multiple tokens, particularly if they don’t understand why a different token is needed for fees.
   
3. **Liquidity Challenges**: Users may not always have ETH on hand, necessitating additional transactions and dealing with volatile prices to acquire it.

### Solution

Paying gas fees with ERC20 tokens solves these issues by:

1. **Improving User Experience**: Users can pay fees in the same tokens they are already transacting with, simplifying their wallet management.
   
2. **Reducing Barriers to Entry**: New users find it easier to engage with blockchain applications when they don't need to worry about acquiring additional tokens for fees.
   
3. **Better Liquidity Management**: Users can keep their funds in their preferred tokens without needing to convert to ETH, minimizing extra steps and costs.

Chainlink’s Price Feeds provide accurate and reliable price data, ensuring fair and transparent conversion of gas fees from ETH to ERC20 tokens, making the process more user-friendly and secure.

## How It Was Built

The core of this project is the `ERC20ChainlinkPaymaster.sol` contract, written in Solidity and deployed using the Atlas IDE. 

A simple Greeter contract and a Vue.js front-end demonstrate the functionality of this Paymaster, utilizing Chainlink Data Feeds both on-chain and off-chain to determine the required amount of ERC20 tokens for gas fees.

## Team

We are 7685labs, a diverse team (small team of 10 ppl) with expertise across all aspects of development, from GenAI to design. We also have a dedicated member focusing on smart contracts.

Connect with us on [X](https://x.com/7685labs).

## Installation Guide

To get started:

1. Clone the repository:

   ```bash
   git clone https://github.com/labs7685/Zk-paymaster/
   ```

2. Start the project:

   ```bash
   yarn
   yarn dev
   ```

3. Open your browser and navigate to the displayed localhost URL to interact with the front-end.
