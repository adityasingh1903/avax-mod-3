# Tokenized Asset Smart Contract

The Tokenized Asset Smart Contract is a Solidity-based smart contract that represents a tokenized asset with a fixed supply. It allows the contract owner to mint new tokens, transfer tokens between addresses, and burn tokens (remove them from circulation).

## Contract Details

- Contract Name: TokenizedAsset
- Solidity Version: ^0.8.0
- License: MIT

## Getting Started

1. Install a compatible Ethereum development environment, such as Remix or Truffle.
2. Create a new Solidity file and paste the TokenizedAsset contract code into it.
3. Deploy the contract to an Ethereum blockchain (testnet or mainnet) of your choice.

## Smart Contract Functions

### Constructor

The constructor initializes the contract with the following parameters:

- `givenName`: The name of the tokenized asset.
- `givenSymbol`: The symbol of the tokenized asset.
- `initialAssetUnits`: The initial total supply of asset units.

### Transfer Asset

Function Signature: `function transferAsset(address recipient, uint units) public`

This function allows users to transfer a specified number of asset units to another address (`recipient`) if they have enough balance.

### Burn Asset

Function Signature: `function burnAsset(uint units) public`

This function allows the contract owner to burn (remove from circulation) a specified number of asset units.

### Mint Asset

Function Signature: `function mintAsset(address recipient, uint units) public ownerOnly`

This function allows the contract owner to mint (create) new asset units and assign them to a specified recipient.

## Author

Aditya singh

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

