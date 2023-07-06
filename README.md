# Create a Token

## Description

This is a smart contract for handling of tokens implemented in solidity. This smart contract allows for the creation, destruction and storing details of the tokens.

## Getting Started

### Requirements

1. Firstly, create a smart contract with name as MyToken.
2. This contract has some public variables to store the details about the tokens:
   * `tokenName`: A variable of string type to store the name of token.
   * `tokenAbbrv`: A variable of string type representing the abbreviation of token.
   * `totalSupply`: A variable of unsigned integer type representing the total supply of tokens.
3. The contract has a mapping of addresses to balances:
   * `balances`: A mapping that associates addresses with their corresponding token balances.
4. The contract has a mint function that increases the total supply and the balance of the "sender" address by a given value:
   * Parameters:
     * `_address`: The address to which the tokens will be minted.
     * `_value`: The number of tokens to be minted.
   * Behaviours:
     * Increases the `totalsupply` and balance of `_address` will be incremented by the `_value`.
5. The contract has a burn function that decreases the total supply and the balance of the "sender" address by a given value:
   * Parameters:
     * `_address`: The address from which the tokens will be burned.
     * `_value`: The amount of tokens to be  burned.
   * Behaviours:
     * Check if the balance at the `_address` is greater than or equal to `_value`
     * If true, decrease the `totalSupply` and balance at `_address` by `_value`
       
### Executing program

1. Deploy the `MyToken` contract to a supported Ethereum network.
2. Once deployed, you can interact with the contract by calling the following functions:
   * `Mint`: Used to Create new tokens and assigns them to a specified address.
     * Parameters:
       * `_address`: The address to which the tokens has to be minted.
       * `_value`: The numbers of tokens to be minted.
   * `Burn`: Destruct existing tokens by reducing the total supply and balance at the specified address.
     * Parameters:
       * `_address`: The address from which the tokens will be burned.
       * `_value`: The number of tokens to be burned.
   * `balances`: By providing the address to this, you will get the number of tokens available at the provided address.

## Authors

Mohand Sai Reddy

21BCS11845@cuchd.in

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
