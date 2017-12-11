# Understanding Forks
*A Brief Intro to Blockchains Forks*

Bitcoin is a distributed and unified ledger that is verified by all the full nodes in the Bitcoin Network.  Full nodes all agree to enforce a similar set of rules so as to maintain a unified version of the Bitcoin ledger.  For example, 1 mb block size is a rule that Bitcoin full nodes currently enforce.  If a 2mb block is submitted, then any node that chooses to download this block is left behind and eventually left out of the Bitcoin Network because their version of the Bitcoin ledger doesn’t match up with the rest.  

The Bitcoin ledger is also updated with a new “block,” or record of Bitcoin transactions, by miners every 10 minutes or so.  This creates a chain of “blocks” that is constantly being extended; hence the name “blockchain.”  For the most part, maintaining a unified ledger via consensus is fairly easy.  A miner adds a block and the full nodes verify it.  However, a fork may occur when the full nodes must make a choice between two different versions of the blockchain floating around in the Bitcoin Network.  This ultimately creates a “split” and can happen in one of two ways: through the process of mining and through the implementation of new software which changes the set of rules the full nodes agree to enforce.    

For the purposes of Chainsplit, we will be focusing only on the latter definition which can be further categorized as Hard Forks and Soft Forks.

## Hard Forks

A **hard fork** occurs when all of the full nodes in the Bitcoin network are required to update their software to implement new rules.  Those who choose not to download the new software will no longer be part of the new network.  Should different groups of miners and full nodes choose to support both chains, the blockchain “splits” into two.  However if only one is supported, only one remains.

*Example:*
+ Bitcoin Cash is an example of a hard fork where both chains survived.

+ Bitcoin XT is an example of a hard fork but was insufficiently supported to continue.

## Soft Forks

A **soft fork** occurs when when a new set of rules are introduced within the old set of rules.  This type of fork is “backward compatible” meaning only mining full nodes are required to implement them.  An example of a hypothetical soft fork would be to decrease the blocksize from 1mb to 750 kb.  The 750 kb rule would exist within the 1mb rule enforced by non-mining nodes.  Therefore, the 750 dk rule would only need to be enforced by mining nodes which would then be accepted by non-mining nodes.  

*Example:*
+ Segwit is an example of a soft fork.  


## Conclusion

Forks aren't inherently a bad thing.  In fact, they can be necessary to implement new code to improve Bitcoin.  However, there are situations where forks can be disruptive.  These are known as "contentious forks" and occur when groups of people disagree on the rules of consensus.  We will go into why these contentious forks are detrimental in our next article.
