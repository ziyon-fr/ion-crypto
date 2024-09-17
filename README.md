# ZIYON TOKEN SMART CONTRACT

This repository contains the smart contract for the ZIYON token (symbol: ION), implemented using the BEP-20 standard. The contract is written in Solidity and uses libraries and best practices such as SafeMath to ensure secure operations and prevent overflow. It is designed to be flexible and secure, with features including transaction control and permission management.

## Key Features

- **BEP-20 Standard**: The token adheres to BEP-20 specifications, providing compatibility with the Binance Smart Chain and other platforms that use this standard.
- **Total Supply**: The total token supply is fixed at 100 million, with 8 decimal places.
- **Permission Control**: Control functions such as `onlyOwner` allow only the contract owner to execute critical operations, such as transferring ownership or adjusting transaction limits.
- **Maximum Transaction Amount**: The contract imposes a transaction limit to prevent market manipulation, set at 100,000 tokens per transaction.
- **Security**: The contract uses the SafeMath library for all arithmetic operations, ensuring protection against overflow and underflow.
- **Transfer and Approval Events**: Full BEP-20 event support, including `Transfer` and `Approval`.

## Implemented Features

- **totalSupply**: Returns the total amount of tokens in circulation.
- **decimals**: Returns the number of decimal places used by the token.
- **symbol**: Returns the token symbol.
- **name**: Returns the token name.
- **getOwner**: Returns the address of the token owner.
- **balanceOf**: Returns the token balance of a given address.
- **transfer**: Transfers tokens from one address to another.
- **approve** and **allowance**: Manages permissions for a third party to spend tokens on behalf of another address.
- **transferFrom**: Allows token transfers using third-party permissions.

## Deployment Settings

The contract is pre-configured with the following default properties:

- Token Name: ZIYON
- Token Symbol: ION
- Decimal Places: 8
- Total Supply: 100,000,000 ION
- Maximum Transaction Amount: 100,000 ION

## How to Use

Clone the repository and deploy the contract using any Solidity development tool such as Remix, Truffle, or Hardhat.
