# MyToken Smart Contract

## Overview

`MyToken` is an ERC-20 token contract implemented in Solidity. It extends the OpenZeppelin ERC-20 and Ownable contracts to create a basic token with minting, burning, and transferring capabilities.

## Features

- **Token Details:**
  - The contract stores information such as the title and code of the token.

- **Minting:**
  - The owner can mint new tokens and allocate them to a specified address.

- **Burning:**
  - Token holders can burn a portion of their own tokens, reducing the total supply.

- **Transferring:**
  - Token holders can transfer a portion of their tokens to another address.

## Getting Started

### Prerequisites

- Solidity Development Environment
- Truffle or Hardhat (for deployment and testing)

### Deployment

1. Deploy the contract to a blockchain network of your choice.
2. Ensure to set the initial owner's address when deploying.

### Usage

- Mint new tokens:
  ```solidity
  function mint(address _to, uint256 _portion) public onlyOwner
  ```

- Burn tokens:
  ```solidity
  function burn(uint256 _portion) public
  ```

- Transfer tokens:
  ```solidity
  function transfer_tk(address _to, uint256 _portion) public
  ```

### Testing

- Implement and execute tests using Truffle or Hardhat.

## Notes

- This contract is a basic implementation and may need additional features and security measures for production use.
- Always ensure proper testing and auditing before deploying smart contracts on a live network.
- Be cautious when using the `onlyOwner` modifier, as it grants exclusive access to certain functions.

## License

This smart contract is released under the UNLICENSED license.



