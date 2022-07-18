# Overview
实施方案（代码）
重要功能、参数、用法


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
任何人都可以通过调用createVault来创建一个金库。当创建金库时，会部署一个资金令牌（vToken），并返回金库ID。

## Minting
````
function mint(
uint256[] calldata tokenIds,
uint256[] calldata amounts     ) external override virtual returns (uint256)
````
mint函数允许你为提供给基金的每个NFT铸造一个vToken。
调用此方法需要给合约地址授予该NFT ID的approval

## Redeeming
````
function redeem(uint256 amount, uint256[] calldata specificIds)
external
override
virtual
returns (uint256[] memory)
````
赎回功能允许用户使用他们的NFTX基金代币从适当的金库中以伪随机方式赎回NFTs。
调用此方法需要给合约地址授予该Erc20的approval

## vToken (Fund Tokens)
对于BootstrapNFT上的每一个基金，都会部署一个vToken代理克隆合约，作为通过该基金进行造币/赎回的手段。每个vToken都是一个标准的ERC20。
