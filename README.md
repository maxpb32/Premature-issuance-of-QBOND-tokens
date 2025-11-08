# Proposal to allow Pre-mint tokens to Qbond

## Proposal
Allow early issuance of MBND tokens.

> Option 0: no

> Option 1: yes

## Overview of QBOND’s functionality
The Qbond smart contract is implemented through the tokenization of staked positions. Each epoch issues tokens named MBNDXXX (XXX - epoch number), which represent staked position tokens. The maximum number of MBND tokens in the Qubic network is 52, since rewards for staking in Qearn are distributed 52 weeks after the token is issued — at which point the token is burned. The core idea behind the Qbond smart contract lies in the tokenization of staking positions. This approach not only provides a better user experience (tokens are visible directly in the wallet) and easier trading, but also enables the creation of a DeFi ecosystem built upon these assets. 

For example, the announced Qloan smart contract will be able to use MBND tokens as collateral. At present, the MBND token is considered the most stable asset, as it offers a predictable yield by the end of its lifecycle — making it a perfect fit for use as collateral.
 
# Future problem of token issuance fees
Due to the introduction of high fees for calling the token issuance function (and based on current discussions, these fees may become significantly large), the Qbond smart contract’s lifespan may be limited. This situation requires immediate adjustments, specifically addressing the issue of expensive token issuance — and this must be done as soon as possible, otherwise the smart contract won't be able to continue functioning.

In order to maintain an uninterrupted correct functioning of the smart contract,we propose the following temporary adjustment :

* Pre-mint tokens in advance (Until the next halving). This would provide time to rethink and develop an alternative approach to the smart contract mechanism, more aligned and adapted to this new chapter that Qubic's smart contract are breaking into. 

## Benefits of proposed changes
These changes guarantees that Qubic's network have a solid solution for Liquid Staking Token (LST) for investors, giving liquidity to staked QUs and boosting Qubic's ecosystem by unlocking idle capital; some of the benefits a secure and fully functional LST brings for the whole ecosystem are :

* __Enhanced capital utilization across the ecosystem :__

As the same capital can be utilized in other activities (trading, providing liquidity, lending, collateralizing loans, derivatives, etc), on-chain activity is boosted, generating, for all other protocols, more utilization, fees and burn mechanisms, as well as increased liquidity and volume.
* __Lower opportunity cost of staking :__

 With a less onerous approach to staking, users would be more prone to lock their QUs, which, in turn, potentializes all the benefits of locking (that is, lower circulating supply, long-term compromise, etc).
* __Enable and enhance DeFi across the network :__

 It dissolves the user's conflict of either directing capital to staking or to DeFi, creating a synergy and complementarity between the two. By enabling this dynamic, it makes possible to develop in the network, in an efficient way, a lot DeFi protocols that weren't possible before.
* __Enable new financial strategies and instruments :__

 Liquid staking empower users to more efficiently use their capital, be it for risk-mitigation or for leveraged strategies; it's essential for leveraged staking, restaking, lending, basis trading, derivative markets and other yield farming strategies.

With these benefits, there's no doubt Qubic network would attract more users and, consequentially, more capital. Businesses would be more incentivized in building in the network, creating financial protocols that — thanks to Qubic's infrastructure and architecture, that gives protocols in its network unparalleled advantage regarding speed and fees — could even outcompete more stablished businesses in other networks.

 Our goal is to support the growth of the Qubic ecosystem, which is why we strive to make our projects attractive, user-friendly, and truly valuable. 




