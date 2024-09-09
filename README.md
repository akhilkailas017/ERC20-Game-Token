# GameT Token (GTE) - ERC20 Smart Contract

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)

## Overview

`GameT` (symbol: `GTE`) is an ERC20 token built on the Ethereum blockchain. This smart contract implements a fungible token that adheres to the ERC20 standard, providing essential functionality for creating and managing tokens in a decentralized and secure manner. The contract is developed using OpenZeppelin's secure and battle-tested ERC20 library.

## Contract Details

- **Token Name**: GameT
- **Token Symbol**: GTE
- **Total Supply**: 100 GTE (100 * 10^18 in wei)
- **Decimals**: 18
- **Standard**: ERC20
- **License**: MIT

## Features

- **Admin-Controlled Minting**: The contract owner (admin) has the authority to mint new tokens to any specified address.
- **Secure ERC20 Implementation**: Built on top of OpenZeppelin's ERC20 standard to ensure robust and secure token functionality.

## Functions

### Constructor

The constructor initializes the token with a name (`Game`), symbol (`GTE`), and assigns the contract deployer as the `admin`. It also mints an initial supply of 100 GTE to the deployer's address.

### Modifiers

- **`onlyAdmin`**: Ensures that only the contract admin can call certain functions, such as minting new tokens.

### Public Functions

- **`safeMint(address to, uint256 value) public onlyAdmin`**: Allows the admin to mint new tokens to a specified address.

## Usage

### Deploying the Contract

To deploy the contract, use Remix or any other Ethereum development environment that supports Solidity. Make sure to set the Solidity compiler version to `0.8.23`.

## Verified Contract Address

The contract is deployed and verified at the following address:

- **Verified Contract Address**: `0x01c7E7095eD33C8058f04057D7EA20c9F216b5D6`
- **Verified Contract URL**: https://sepolia.etherscan.io/address/0x01c7E7095eD33C8058f04057D7EA20c9F216b5D6#code

## Security

This contract follows best practices for secure smart contract development. It is highly recommended to conduct further audits and due diligence before deploying on the mainnet or using it in a production environment.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
