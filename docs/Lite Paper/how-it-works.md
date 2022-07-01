# How It Works

## Vault creation
Any project can create a vault for any NFT asset on Ethereum to lock the NFT aggregate assets pledged (deposited) by the users.
 
 
## Mint vToken
Any player can deposit eligible NFTs into the corresponding vault to mint alternative NFT-backed tokens called "vTokens". vToken represents a 1:1 claim to a random NFT from within the vault (1NFT=1vToken).

## Create a smart pool
Projects can use their minted vTokens to create a liquidity market for other users to trade. It allows projects to customize the weights of their funding pools. For example, a 90/10 liquidity pool can be created, in which 90% of the liquidity pool is vToken and 10% is reserve assets (such as USDC, ETH, etc.). As liquidity and trading volume build up, the NFT-backed vTokens enter a price discovery phase and discover the "floor price".
 
## Initial price discovery
BootstrapNFT constantly changes the weight of each asset in the pool. The weight is dynamic and change over the lifetime of the token sale. It keeps changing based on the programmed direction. For example, a sale that lasts 3 days, goes from 90%/10% vToken/USDC to 10%/90% vToken/USDC.
 
In the process of lowering the price, bidders will successively buy vTokens at a fair price. In a well-structured sale, the upward pressure on buying offsets the downward pressure on the pool, resulting in a price equilibrium. The initial price is determined by the lowest price in the Dutch auction. BootstrapNFT is helping establish a reliable initial price discovery for NFTs to make them more widely applicable to decentralized finance on Ethereum.
 
## Redeem NFT
### Targeted redemption
The specific NFTs are targeted-redeemed from the vault by paying a targeted redemption fee (usually 5%, 1.05 vTokens). You can also go to the liquidity pool to exchange and redeem without vToken.
 
### Random redemption
Enter the amount (integer) you want to redeem and approve the BootstrapNFT contract with a low or no fee. Once the approved transaction is confirmed, you can randomly redeem the desired amount of NFT from the vault.
