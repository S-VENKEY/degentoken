# Token Contract README

This README provides an overview of the Token contract implemented in Solidity. The contract includes functionalities for managing tokens and redeeming/converting them into hair wax products.

## Overview

The Token contract is an ERC20-compliant token with additional functionalities for managing token minting, burning, transferring, and redeeming/converting tokens into hair wax products.

## Contract Features

### ERC20 Implementation

The contract extends the ERC20 standard, providing functionalities such as:

- Token creation (`_mint`)
- Token transfer (`_transfer`)
- Token burning (`_burn`)
- Balance inquiry (`balanceOf`)

### Ownership

The contract uses the Ownable pattern from OpenZeppelin, allowing the contract owner to perform administrative tasks such as minting tokens.

### Token Minting and Burning

- `mintTokens`: Allows the contract owner to mint new tokens and distribute them to specified addresses.
- `burnTokens`: Allows users to burn a specified amount of tokens, reducing their balance.

### Token Transfer

- `transferTokens`: Allows users to transfer tokens to other addresses.

### Hair Wax Redemption and Conversion

The contract introduces functionalities related to hair wax products:

- `redeemHairWax`: Allows users to redeem tokens for hair wax products based on specified brands and quantities. Tokens are burnt upon redemption, and the corresponding quantity of hair wax is allocated to the user.
- `convertToHairWax`: Allows users to convert tokens to hair wax products. Tokens are burnt upon conversion, and the specified quantity of hair wax is added to the user's balance.

## Usage

1. **Deploying the Contract**: Deploy the Token contract on the Ethereum blockchain.
2. **Interacting with the Contract**:
   - Mint tokens using the `mintTokens` function.
   - Burn tokens using the `burnTokens` function.
   - Transfer tokens to other addresses using the `transferTokens` function.
   - Redeem tokens for hair wax products using the `redeemHairWax` function.
   - Convert tokens to hair wax products using the `convertToHairWax` function.

## Requirements

- Solidity ^0.8.0
- OpenZeppelin Contracts v4.0.0 (ERC20, Ownable)

## License

This contract is released under the MIT License.
