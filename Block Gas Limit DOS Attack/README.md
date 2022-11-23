## Block Gas Limit DOS Attack

In this project we'll see how an unbounted array(refunds array) can be prone to Block Gas Limit dos attack 

There is one more way for attacker to execute DOS attack on the refundsAll function:
 ie. If the refund address has no receive payable function.
Then the tranasaction will revert effectibly making Unexpected revert attack


This refundAll method call fails on Auction contract because  blockGasLimit is set to 10mil
(blockGasLimit: 10000000) and the transaction exceeds that limit with 21mil gas
as we can see from gasReporter.


