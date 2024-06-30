🚀 Token Solidity Smart Contract

This Solidity is a smart contract that implements a basic token system on the Ethereum blockchain. It allows for the minting and burning of tokens while keeping track of the total supply and individual balances.


🌟Features

•	Token Name: A human-readable name for the token.

•	Token Abbreviation: A short, symbolic abbreviation for the token.

•	Total Supply: The total number of tokens in circulation.

•	Minting: Create new tokens and assign them to a specific address.

•	Burning: Destroy tokens from a specific address.


📜 Contract Details

Public Variables

•	Token Name: The name of the token (e.g., "Token").

•	Token Abbreviation: A short abbreviation for the token (e.g., "TK").

•	Total Supply: The total number of tokens in circulation.


Mappings

•	accountBalances: A mapping from addresses to their respective balances.


Functions

'mint'

The mint function allows the creation of new tokens. It takes two parameters: an address and an amount. The function increases the total supply by the specified amount and credits the balance of the recipient address.


Parameters

•	'recipient' (address): The address to which the minted tokens will be credited.

•	'amount' (uint): The number of tokens to mint.

'burn'

The burn function allows the destruction of tokens. It takes two parameters: an address and an amount. The function decreases the total supply by the specified amount and deducts the balance of the sender address. The function ensures that the balance of the sender is greater than or equal to the amount to be burned.

Parameters

•	'account' (address): The address from which the tokens will be burned.

•	'amount' (uint): The number of tokens to burn.


Requirements

•	The balance of the sender must be greater than or equal to the amount to be burned.


🛠️ Usage

To use this contract, deploy it on the Ethereum blockchain using a development environment like Remix or Truffle. Once deployed, you can interact with the contract through its public functions:


Minting Tokens:

•	Call the mint function with the recipient address and the number of tokens to mint.

Burning Tokens:

•	Call the burn function with the account address and the number of tokens to burn.

Example

 // Minting 1000 tokens to address 0x123...
mint (0x123..., 1000);


// Burning 600 tokens from address 0x123...
burn (0x123..., 600);


🚀 Getting Started

Prerequisites

To interact with this contract, you will need:

•	An Ethereum wallet (e.g., MetaMask).

•	Some Ether to pay for gas fees.

•	A Solidity development environment (e.g., Remix, Truffle).


Installation

Clone the Repository:

https://github.com/piyush899998/Assessment-2-metacrafters/blob/main/assessment%202


Deploy the Contract:

•	Compile the contract in Remix.

•	Deploy the contract to the desired Ethereum network (e.g., Mainnet, Ropsten, Rinkeby).


Acknowledgments

•	Solidity Documentation

•	OpenZeppelin

