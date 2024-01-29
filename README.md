# PayLater 

## Overview

The PayLaterContract is a simple smart contract written in Solidity, a programming language for developing smart contracts on the Ethereum blockchain. This contract allows users to add products to a virtual shopping cart and tracks the total number of products purchased. Additionally, it includes a reward mechanism based on the total products purchased.

## Contract Functions

### 1.addToCart(uint256 _productId, uint256 _price) external

This function allows users to add products to the shopping cart by specifying the product ID and price. The price must be divisible by 100, indicating that the "Pay later" option is available for this product. The function ensures that a product with the same ID has not been added previously.

### 2.PurchaseReward(uint256 _productsPurchased) external

Users can trigger this function to update the total number of products purchased. If the total products purchased exceed 25, the transaction will be reverted with a message indicating that 500 "Super coins" have been credited to the user's wallet.

## License

This smart contract is released under the MIT License. See the SPDX-License-Identifier in the contract file for details.

## Author 

Gagan
 
johnwickvk4321@gmail.com
