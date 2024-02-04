# Vault Contract

The `Vault` contract provides a secure and efficient way to deposit and withdraw ERC20 tokens while minting and burning corresponding shares for the deposited tokens.

## Overview

The contract consists of two main functionalities:

1. **Deposit:** Users can deposit ERC20 tokens into the vault, receiving shares in return. These shares represent ownership of the deposited tokens within the vault.

2. **Withdraw:** Users can withdraw their deposited tokens by burning their shares. The withdrawn tokens are sent back to the user's address.

## Contracts

### Vault.sol

This contract manages the deposit and withdrawal of ERC20 tokens.

- **Functions:**
  - `deposit(uint _amount) external`: Allows users to deposit ERC20 tokens into the vault, receiving shares in return.
  - `withdraw(uint _shares) external`: Allows users to withdraw their deposited tokens by burning their shares.

### ERC20.sol

This is a basic ERC20 token contract used by the vault.

- **Functions:**
  - `transfer(address recipient, uint amount) external`: Transfers tokens from the sender's account to the recipient's account.
  - `approve(address spender, uint amount) external`: Approves the spender to spend a certain amount of tokens on behalf of the owner.
  - `transferFrom(address sender, address recipient, uint amount) external`: Transfers tokens from one account to another if the sender has been approved to spend tokens on behalf of the owner.
  - `mint(uint amount) external`: Mints new tokens and adds them to the total supply.
  - `burn(uint amount) external`: Burns tokens, removing them from the total supply.

## License

Both contracts are provided under the MIT License.

## Usage

To use the `Vault` contract, deploy it and then interact with it through the provided functions, depositing and withdrawing ERC20 tokens as needed.

Make sure to have the corresponding ERC20 tokens before interacting with the vault.

## Author

Roshan Pasha

roshanpasha232@gmail.com
