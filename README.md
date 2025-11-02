# Proposal for QBOND
## Overview of QBOND’s functionality
The Qbond smart contract is implemented through the tokenization of staked positions. Each epoch issues tokens named MBNDXXX (XXX - epoch number), which represent staked position tokens. The maximum number of tokens in the Qubic network is 52, since rewards for staking in Qearn are distributed 52 weeks after the token is issued — at which point the token is burned. The core idea behind the Qbond smart contract lies in the tokenization of staking positions. This approach not only provides a better user experience (tokens are visible directly in the wallet) and easier trading, but also enables the creation of a DeFi ecosystem built upon these assets. 

For example, the announced Qloan smart contract will be able to use MBND tokens as collateral. At present, the MBND token is considered the most stable asset, as it offers a predictable yield by the end of its lifecycle — making it a perfect fit for use as collateral.
 
# Future problem of token issuance fees
Due to the introduction of high fees for calling the token issuance function (and based on current discussions, these fees may become significantly large), the Qbond smart contract’s lifespan may be limited. This situation requires immediate adjustments, specifically addressing the issue of expensive token issuance — and this must be done as soon as possible.

Currently, we see two potential solutions, the first option we are proposing to you in this proposal is :

* Pre-mint tokens in advance (Until the next halving). This would provide time to rethink and develop an alternative approach to the smart contract mechanism. 

If this solution is rejected, we will submit the second solution to you.

# Add "Emergency Unlock" Feature

We want to add an "emergency unlock" function on QBOND's smart contract in order to foster a more solid and secure Liquid Staking Token (LST) in Qubic's ecosystem. It consists of :

* At unlock action, the smart contract tries to sell user's MBND tokens on the marketplace if there's any bid higher than the value they would receive from unlocking directly in QEARN
* If no such favorable bid exists, the SC then burns the MBND tokens and unlocks the original funds from QEARN, releasing the user from a trapped position

This way, the protocol doesn't makes unnecessary unlocks, preserving the maximum amount of QUs locked in QEARN, while still securing the investor from potentially catastrophic financial losses.

## Rationale
The proposed function is specially useful in exceptional scenarios where there's no liquidity on MBND's secondary market, or when liquidation on the secondary market causes a loss to user's capital.

For example : 
* Consider that the average APY for locking QUs is 10% and, thus, MBND tokens are being traded around this APY in the secondary market.
* Now, an investor locks 1bn QUs via QBOND, expecting similar returns; however, due to a late surge of deposits in that epoch, the final APY plummets to an abnormally low 3%.

In that case, we have the following : 
* A QEARN user, facing this 3% APY, could simply unlock their funds, losing virtually nothing, and waiting for a more favorable epoch.
* The QBOND user, if he wants to liquidate, is trapped in a loss position. Their only exit is the marketplace, which is saturated with MBND tokens from other epochs offering the standard 10% APY. To compete, they would've to sell their 3% APY bond at a massive discount, pricing it so the buyer effectively earns a 10% yield.

Being more precise, the calculation for this discount is : 

1bn × (1.03/1.10) ​≈936 millions de QUs

The price he would've to sell in order to offer buyers a 10% APY. This forces the investor into a -6.4% capital loss, just to access his funds.

If the "emergency unlock" function is added, the user could simply directly unlock in QEARN, not incurring in losses and completely extinguishing any risk related to the secondary market (be it illiquidity, be it being trapped in a liquidation that causes him bigger losses than simply unlocking).

## Benefits
By giving liquidity to staked QUs, MBND tokens unlocks capital in Qubic's network; bringing a lot of benefits for the whole ecosystem, such as :

* __Enhanced capital utilization across the ecosystem :__

As the same capital can be utilized in other activities (trading, providing liquidity, lending, collateralizing loans, derivatives, etc), on-chain activity is boosted, generating, for all other protocols, more utilization, fees and burn mechanisms, as well as increased liquidity and volume.
* __Lower opportunity cost of staking :__

 With a less onerous approach to staking, users would be more prone to lock their QUs, which, in turn, potentializes all the benefits of locking (that is, lower circulating supply, long-term compromise, etc).
* __Enable and enhance DeFi across the network :__

 It dissolves the user's conflict of either directing capital to staking or to DeFi, creating a synergy and complementarity between the two. By enabling this dynamic, it makes possible to develop in the network, in an efficient way, a lot DeFi protocols that weren't possible before.
* __Enable new financial strategies and instruments :__

 Liquid staking empower users to more efficiently use their capital, be it for risk-mitigation or for leveraged strategies; it's essential for leveraged staking, restaking, lending, basis trading, derivative markets and other yield farming strategies.

 With these benefits, there's no doubt Qubic network would attract more users and, consequentially, more capital. Businesses would be more incentivized in building in the network, creating financial protocols that, thanks to Qubic's infrastructure and architecture — that gives its protocols unparalleled advantage regarding speed and fees —, can even outcompete more stablished businesses in other networks  

 Our goal is to support the growth of the Qubic ecosystem, which is why we strive to make our projects attractive, user-friendly, and truly valuable. 




