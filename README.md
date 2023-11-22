MyToken Smart Contract
This Solidity smart contract, named MyToken, is designed to implement a basic token system on the Ethereum blockchain. It allows for the creation and destruction of tokens, with the ability to check balances and the total supply. Below, you will find a detailed explanation of the contract and its functions.

Contract Details
Token Name: Ethereum
Token Abbreviation: ETH
Total Supply: 0 (initially)
Functions
1. mint(address _address, uint _value)
The mint function allows for the creation of new tokens. It takes two parameters:

_address: The address to which the new tokens will be credited.
_value: The amount of tokens to create and add to the balance of the specified address.
When you call this function, it increases the total supply by the specified _value and increments the balance of the _address by the same amount.

2. burn(address _address, uint _value)
The burn function works in the opposite manner of the mint function. It is used to destroy tokens, reducing the total supply and decreasing the balance of the specified address. The function takes two parameters:

_address: The address from which tokens will be deducted.
_value: The amount of tokens to destroy.
Before performing the burn, the function checks if the balance of the _address is greater than or equal to the _value. If the condition is met, it proceeds to deduct the tokens from both the total supply and the balance of the _address.

Usage Guidelines
To create new tokens, call the mint function with the desired _address and _value.
To destroy tokens, call the burn function with the desired _address and _value. Ensure that the _address has a sufficient balance to cover the burn.
You can check the total supply and balance of any address by directly querying the TotalSupply and balance variables.
This contract uses the Solidity version 0.8.18 and is subject to the MIT License.
Author
poonguzhali S

Licence
This project is licensed under the MIT License - see the LICENSE.md file for details.
