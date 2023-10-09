# ERC20 Solidity Smart Contract

This is the implementation of the standard ERC20 token in Solidity. It can be used as a foundation for creating your own token contracts on the Ethereum network.

## IERC20.sol

This file contains the interface for the ERC20 token. It declares the functions that a contract must implement in order to be considered an ERC20 token.

The functions declared in the interface are as follows:

- `totalSupply()`: returns the total supply of the token.
- `balanceOf(address account)`: returns the balance of the specified account.
- `transfer(address recipient, uint amount)`: transfers a given amount of the token to the specified recipient.
- `allowance(address owner, address spender)`: returns the amount of tokens that the spender is allowed to spend on behalf of the owner.
- `approve(address spender, uint amount)`: allows the spender to spend a specified amount of tokens on behalf of the owner.
- `transferFrom(address sender, address recipient, uint amount)`: transfers a specified amount of tokens from one account to another on behalf of a third-party spender.

The interface also declares two events:

- `Transfer(address indexed from, address indexed to, uint value)`: emitted when tokens are transferred from one account to another.
- `Approval(address indexed owner, address indexed spender, uint value)`: emitted when the allowance of a spender is changed.

## ERC20.sol

This file contains the implementation of the ERC20 token. It implements the functions declared in the interface and defines additional variables and functions to handle the token supply and transfers.

The contract defines the following variables:

- `totalSupply`: the total supply of the token.
- `balanceOf`: a mapping of token balances for each account.
- `allowance`: a mapping of allowances for each account and spender.
- `name`: a string representing the name of the token.
- `symbol`: a string representing the symbol of the token.
- `decimals`: the number of decimal places used to display the token value.

The contract implements the following functions:

- `transfer`: transfers a given amount of the token to the specified recipient.
- `approve`: allows the spender to spend a specified amount of tokens on behalf of the owner.
- `transferFrom`: transfers a specified amount of tokens from one account to another on behalf of a third-party spender.
- `mint`: mints a given amount of new tokens and assigns them to the calling account.
- `burn`: burns a given amount of tokens from the calling account.

## License

This code is licensed under the MIT license.
