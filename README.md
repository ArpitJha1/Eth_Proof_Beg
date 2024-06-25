MyToken Smart Contract

Welcome to the MyToken smart contract repository! This smart contract, written in Solidity, defines a basic ERC-20-like token with minting and burning functionalities. Below is an overview of the contract's structure and features.
Table of Contents

    Overview
    Features
    Functions
    Usage
    License

Overview

This Solidity contract provides a simple implementation of a token on the Ethereum blockchain. It includes the following core components:

    Public variables for the token's name, abbreviation, and total supply.
    A mapping to track the balance of each address.
    Functions to mint and burn tokens, adjusting the total supply and the balances accordingly.

Features

    Token Details: Public variables store the details about the token.
        tokenName: The name of the token, set to "ETHEREUM".
        tokenAbb: The abbreviation of the token, set to "ETH".
        totalSupply: The total supply of the token, initialized to 0.

    Balance Mapping: A mapping that associates addresses with their token balances.

    Mint Function: A function to increase the total supply and the balance of a specified address.

    Burn Function: A function to decrease the total supply and the balance of a specified address, with a check to ensure the address has enough balance.

Functions
mint(address add, uint value) public

Increases the total supply of the token and the balance of the specified address.

    Parameters:
        add: The address of the recipient.
        value: The amount of tokens to mint.

burn(address add, uint value) public

Decreases the total supply of the token and the balance of the specified address, ensuring the address has enough tokens to burn.

    Parameters:
        add: The address of the token holder.
        value: The amount of tokens to burn.

Usage

To interact with this contract, you can use any Ethereum development environment, such as Remix or Truffle. Here is a basic outline of how to use the contract:

    Deploy the Contract: Deploy the MyToken contract to the Ethereum network.
    Mint Tokens: Call the mint function to increase the token supply and assign tokens to a specific address.
    Burn Tokens: Call the burn function to decrease the token supply by removing tokens from a specific address.

Author

Arpit Anand

License

This project is licensed under the MIT License. See the LICENSE file for details.
