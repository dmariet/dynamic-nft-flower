# dynamic-nft-flower

## Overview
The Dynamic NFT Flower contract is an ERC721-compliant smart contract designed to represent a dynamic NFT (Non-Fungible Token) that simulates the growth stages of a flower. The contract facilitates the evolution of the NFT over time, transitioning through various stages of growth, from seed to sprout to bloom. Each growth stage of the flower is represented by a unique token URI stored on the IPFS (InterPlanetary File System) network.

## Features
- Implements the ERC721 standard for non-fungible tokens, enabling unique ownership and transferability of tokens.
- Utilizes the Chainlink AutomationCompatible interface for periodic updates and maintenance tasks.
- Dynamically updates the token URI to reflect the current growth stage of the flower.
- Supports the minting of new flower tokens with the initial seed stage.
- Allows users to manually trigger the growth of their flower tokens by calling the `growFlower` function.
- Implements automated upkeep checks and performs periodic growth updates using the Chainlink Keepers infrastructure.

## Contracts
- **Flower.sol:** Main smart contract implementing the functionality of the Dynamic NFT Flower.

## Usage
1. Deploy the Flower contract on the Sepolia blockchain.
2. Initialize the contract with the desired update interval for the flower growth stages.
3. Users can mint new flower tokens by calling the `safeMint` function.
4. The flower token evolves automatically over time, transitioning through different growth stages.
5. Users can manually trigger the growth of their flower tokens by calling the `growFlower` function.
6. Automated upkeep checks ensure that the flower continues to grow and update according to the specified interval.

## Deployment
- Network: Sepolia
- Token Name: Chainlink Bootcamp Flower 2024 (CFLO)

## Security Considerations
- Ensure that the contract owner address is secured and only accessible by authorized personnel.
- Validate inputs and perform appropriate checks to prevent unexpected behavior or exploits.
- Regularly review and audit the contract code to identify and address any potential security vulnerabilities.

## License
This contract is released under the MIT License.

