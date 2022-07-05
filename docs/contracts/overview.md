# Overview

## Vault creation

````
function createVault(

        string memory name,

        string memory symbol,

        address _assetAddress,

        bool is1155,

        bool allowAllItems

    ) external virtual override returns (uint256)
````

Anyone can create a vault by calling createVault. When the vault is created, a funding token (vToken) is deployed and the vault ID is returned.




## Minting
````
function mint(

        uint256[] calldata tokenIds,

        uint256[] calldata amounts     ) external override virtual returns (uint256)

````
The mint function allows you to mint a vToken for each NFT provided to the fund.

Calling this method requires granting the approval of the NFT ID to the contract address.



## Redeeming

````
function redeem(uint256 amount, uint256[] calldata specificIds)

    external

    override

    virtual

    returns (uint256[] memory)
````

The redeem function allows users to use their NFTX fund tokens to redeem NFTs from the appropriate vault in a pseudo-random fashion.

Calling this method needs to grant the approval of the Erc20 to the contract address


## vToken (Fund Tokens)
For each fund on NFTX, a vToken proxy clone contract is deployed as a means of minting/redemption through that fund. Each vToken is a standard ERC20.

