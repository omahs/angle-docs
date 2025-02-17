---
description: Common questions about getting and exchanging the Protocol's stablecoins
---

# FAQ - Stable Seekers and Holders

## What is agEUR backed by?

First, agEUR minted through the Core module is backed by the collateral that was used to mint it. Then, if this collateral is volatile, HA can open positions on the collateral stored in the Core module to protect it from changes in collateral/agEUR exchange rate. In case this is not enough, SLPs come to over-collateralize the Core module.

## Could I use the Angle Core module as a decentralized exchange?

Angle Core module can be used as a decentralized exchange where there is no slippage for swapping.

For example, if Angle's agEUR is backed by wETH and USDC, a user wishing to swap wETH against wBTC with no slippage can choose to come to Angle, swap wETH against agEUR, and then use these agEUR to redeem wBTC.

## What happens if I want a collateral that is not present in sufficient quantity against my agEUR?

Angle Core module leaves the choice to its users as for the collateral type they can get when burning their stablecoins.

It is however possible that there is an imbalance between the value of the different collateral pools backing a stablecoin. If 100 agEUR are backed by 10 DAI and 150 USDC, the transactions of users asking DAI against 100 agEUR will fail because there are not enough DAI in reserves to reimburse the users.

In this case, users will have to burn agEUR in exchange for USDC.

## Do I still own the collateral I bring to the Core module to mint agEUR?

No. Unlike in Maker's system, Angle Core module works with swaps from a user perspective, meaning that the collateral brought to get stablecoins no longer belongs to the person who brought it: it belongs to the Core module which keeps it in reserves and uses it to back the minted stablecoin.

## Are the agEUR minted borrowed from the Core module?

No, once the stablecoins are issued from the Core module, they are not considered as a debt from the person which issued it, and there is no need to reimburse or to pay interest to the Core module on it.

## Can I transfer my agEUR to other addresses?

Yes, Angle's agEUR is a standard ERC-20 tokens. They can be exchanged and transferred from one address to another.

This notably means that someone willing to get Angle's stablecoins may buy it on the open market (like on Uniswap) and without interacting with the protocol. The same goes for people willing to sell their stablecoins.

Note that having people buying on secondary markets creates an increasing pressure on the market price of the stablecoins, thus incentivizing people to issue new tokens to restore peg.
