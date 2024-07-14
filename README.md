# defi-stable
It's a  Defi-StableCoin where users can deposit WETH and WBTC in exchange for a token that will be pegged to the USD.

# Decentralized Stable Coin (DSC)

A decentralized stable coin built using Solidity and Foundry. This project implements a stable coin with minting and fuzztests controlled by the contract owner.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contract Overview](#contract-overview)
- [Testing](#testing)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project demonstrates the implementation of a decentralized stable coin (DSC) using Solidity. The DSC is designed to be minted and burned by the contract owner. This project uses Foundry, a fast and modular toolkit for Ethereum application development.

## Features

- **Minting**: Only the owner can mint new DSC tokens.
- **Burning**: Only the owner can burn DSC tokens.
- **Transfer Restriction**: Transfers are not allowed to simulate a failed transfer scenario.
- **Access Control**: Owner-only functions for minting and burning.

## Prerequisites

- **Foundry**: Ensure you have Foundry installed. You can install it by following the instructions [here](https://book.getfoundry.sh/getting-started/installation.html).
- **Node.js**: Required for managing dependencies. Install it from [here](https://nodejs.org/).

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Build the project**:
    ```bash
    forge build
    ```

## Usage

### Deploying the Contract

You can deploy the contract using Foundry’s `forge` command:

```bash
forge create --rpc-url <YOUR_RPC_URL> --private-key <YOUR_PRIVATE_KEY> src/MockFailedMintDSC.sol:MockFailedMintDSC
