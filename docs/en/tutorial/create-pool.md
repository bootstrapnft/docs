# Create pool

## Create a smart pool

Create a smart pool. You can set custom token symbols and names. You can also specify the initial supply of tokens, which is arbitrary.

 ![](../asset/14.png)


Creating a pool requires setting relevant parameters according to the purpose of the pool.

 ![](../asset/15.png)

* Swap can be paused - the controller can stop the transaction. 

* Transaction fees can be changed - Controllers can change transaction fees after deployment, ranging from 0.0001% to 10%.

* The weight can be changed - the controller can change the weights arbitrarily (transferring tokens to keep the price constant) 

* Tokens can be added/removed 

* LPs can be whitelisted - anyone can add liquidity to the pool after creation unless their addresses are added to the whitelist.

* The cap can be changed - this limits the total supply of pool tokens. 


The button will display "Unlock <Token Name>" for each token and prompt you to unlock each token, asking you to send a transaction to approve each token.


 ![](../asset/16.png)

 ![](../asset/17.png)




Once all tokens are approved, the button will display "Create" and pressing it will create the transaction.

 ![](../asset/18.png)


Tips:If the token you want to add is not listed on the token selector panel, you can add any custom token by pasting its address in the search field.

 ![](../asset/120.png)


IMPORTANT: Make sure the custom token you are adding is ERC20 compliant.



## Add liquidity
Click on "explore pools" and find the smart pool.

![](../asset/21.png)




Click "add liquidity" to add appropriate liquidity to the smart pool.

 
![](../asset/122.png)





## Set gradual weight
Set the drop ratio.

 
![](../asset/23.png)
