# ERC20 Solidity Contract

This is a basic ERC20 Solidity contract developed using the OpenZeppelin library. 

## Description

The project includes two main contracts: ERC20 and Ownable. The ERC20 contract defines a standard token interface, while the Ownable contract makes sure that only the contract owner can execute certain functions.

The ERC20 contract includes basic functionality such as transferring tokens, approving allowances, and checking balances. The contract also includes additional functionality provided by the OpenZeppelin library such as token burning, which allows for the removal of tokens from circulation.

## Prerequisites

- Solidity ^0.8.9
- OpenZeppelin ^4.4.0

## Deployment

To deploy the contract, simply copy the code to a Solidity compiler and run the contract. The contract requires that you specify the token name and symbol in the constructor function. Once the contract is deployed, the contract owner can mint new tokens using the `mint` function.
