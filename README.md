# Proposal for QBOND
## Overview of QBOND’s functionality
The Qbond smart contract is implemented through the tokenization of staked positions. Each epoch issues tokens named MBNDXXX (XXX - epoch number), which represent staked position tokens. The maximum number of tokens in the Qubic network is 52, since rewards for staking in Qearn are distributed 52 weeks after the token is issued — at which point the token is burned. The core idea behind the Qbond smart contract lies in the tokenization of staking positions. This approach not only provides a better user experience (tokens are visible directly in the wallet) and easier trading, but also enables the creation of a DeFi ecosystem built upon these assets. 

For example, the announced Qloan smart contract will be able to use MBND tokens as collateral. At present, the MBND token is considered the most stable asset, as it offers a predictable yield by the end of its lifecycle — making it a perfect fit for use as collateral.


## Future problem of token issuance fees
Due to the introduction of high fees for calling the token issuance function (and based on current discussions, these fees may become significantly large), the Qbond smart contract’s lifespan may be limited. This situation requires immediate adjustments, specifically addressing the issue of expensive token issuance — and this must be done as soon as possible.

Currently, we see two potential solutions, the first option we are proposing to you in this proposal is :

* Pre-mint tokens in advance (Until the next halving). This would provide time to rethink and develop an alternative approach to the smart contract mechanism. 

If this solution is rejected, we will submit the second solution to you.
