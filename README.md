# DegenToken

## Overview
DegenToken is an ERC20 token designed for Degen Gaming, allowing players to earn and redeem tokens for in-game items and rewards.

## Description
This contract implements the following functionality:
* Minting: Only the owner can mint new tokens and distribute them to players as rewards.
* Transferring: Players can transfer their tokens to others.
* Redeeming: Players can redeem their tokens for items in the in-game store.
* Checking Balance: Players can check their token balance at any time.
* Burning: Anyone can burn tokens they own that are no longer needed.

## Getting Started

### Installation
```
* git clone https://github.com/Boluchel/Degen-Token-.git
* npm install
```
### Deployment
```
npx hardhat compile
```

## Contract Address
* DegenToken Contract Address: 0xaEC882d4cfB71A74d1c2E7cE132E0708436E3EC6

## Functions
### mintDegenTokens(address _player, uint256 _amount)
* Access: Public
* Description: Mints new tokens and distributes them to the specified player.

### burnDegenTokens(uint256 amount)
* Access: Public
* Description: Burns the specified amount of tokens owned by the caller.

### transferDegenToken(address to, uint256 amount)
* Access: Public
* Description: Transfers the specified amount of tokens to the specified address.

### getDegenBalance(address _playerAddress)
* Access: Public View
* Description: Returns the token balance of the specified player.

### viewMarketplace()
* Access: External Pure
* Description: Returns a string describing the available items in the marketplace.

### redeemMarketPlaceItem(uint8 _itemToredeem)
* Access: External
* Description: Redeems the specified item from the marketplace using the caller's tokens.

### canUserPlay()
* Access: External View
* Description: Returns a boolean indicating whether the caller can play the game.

## Authors
Banwo Boluwatife

## License

This project is licensed under the MIT License
