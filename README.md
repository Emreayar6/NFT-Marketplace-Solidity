# NFT Marketplace Contract

This is the project based developing smart contract via solidity. <br>

This Solidity contract implements an NFT marketplace. It allows users to list, buy, cancel, update listings, and withdraw proceeds from sales. The contract supports the ERC721 token standard.

## Contract Details

- Contract Name: NftMarketplace
- SPDX License Identifier: MIT

## Error Messages

- `NftMarketplace__PriceMustBeAboveZero`: Price must be greater than zero.
- `NftMarketplace__NotApprovedForMarketPlace`: NFT is not approved for listing.
- `NftMarketplace__AlreadyListed`: NFT is already listed for sale.
- `NftMarketplace__NowOwner`: Current user is not the owner of the NFT.
- `NftMarketplace__NotListed`: NFT is not listed for sale.
- `NftMarketplace__PriceNotMet`: Sent value does not match the listed price of the NFT.
- `NftMarketplace__NoProceeds`: No proceeds available for withdrawal.
- `NftMarketplace__TransferFailed`: Failed to transfer funds during withdrawal.

## Structures

### Listing

A struct representing a listing in the marketplace.

- `price`: Price of the listed item.
- `seller`: Address of the seller.

## Events

- `ItemListed`: Emitted when an item is listed for sale.
- `ItemBought`: Emitted when an item is bought.
- `ItemCanceled`: Emitted when a listing is canceled.
- `ItemUpdated`: Emitted when a listing is updated.

## Storage

- `s_listings`: A mapping of NFT addresses and token IDs to their respective listings.
- `s_proceeds`: A mapping of seller addresses to the amount earned.

## Modifiers

- `notListed`: Checks if an NFT is not already listed for sale.
- `isListed`: Checks if an NFT is listed for sale.
- `isOwner`: Checks if the current user is the owner of an NFT.

## Functions

- `listItem`: Lists an NFT for sale in the marketplace.
- `buyItem`: Buys an NFT from the marketplace.
- `cancelListing`: Cancels a listing in the marketplace.
- `updateListing`: Updates the price of a listed item.
- `withdrawProceeds`: Withdraws the proceeds from sales.
- `getListing`: Retrieves the listing information for an NFT.
- `getProceeds`: Retrieves the amount of proceeds available for a seller.

The contracts have been deployed to Sepolia Testnet. <br>

"NftMarketplace.sol"

```
0xFBe58999cb796443F07fb9a229dC1c2DD0E175f5
```

"BasicNft.sol"

```
0x65860F72252b3a91163b3D370A85EBA9eE30474c
```
