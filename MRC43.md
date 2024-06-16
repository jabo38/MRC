# Protocol Owned Liquidity Upgrade to 2.0 Post Bootstrapping

## Update to "Building the Foundation: Phased AMM Deployment in Morpheus"
This MRC builds on a great work from MRC 9 to describe the phases of deploying the Protocol Owned Liquidity into the Uniswap AMM just after the bootstrapping period. 
https://github.com/MorpheusAIs/MRC/blob/main/IMPLEMENTED/MRC09.md

For the bootstrapping period the POL providing liquidity positions of both ETH and MOR made sense. 
But given there is now plenty of MOR tokens claimed & generally available for trading, it would seem logical to move toward the following POL pattern.

## Upgraded Protocol Owned Liquidity Pattern
- 1. stETH is collected and swapped to wETH.
- 2. 75% of the resulting wETH is used to swap for MOR from the Uniswap pool.
- 3. The remaining 25% of wETH would be paired with the 25% MOR as a full range liquidity position on Uniswap.
- 4. The 50% remaining MOR that were purchased are held in the POL and NOT deposited back into liquidity or burned. 

## Burning & Tail Emissions
- This approach can be the basis for implementing the Burn Function described in the white paper.
- The 50% of the MOR held in the PoL can be locked for 16 years. In order to function as the basis for [the #2 epoches Tail Emissions](https://github.com/MorpheusAIs/Docs/blob/main/!KEYDOCS%20README%20FIRST!/WhitePaper.md#tail-emissions-of-mor).
- The other 50% of the MOR held in the PoL can be sent to a permenent burn address and destroyed forever.

## Conclusion
This would seem to be most aligned with the spirit of the original design and white paper, as it would provide liquidity for MOR sellers. 
Both short term with the immediate buy of MOR, and long term with the full range wETH liquidity position. 
By withdrawing MOR purchased by POL and perodically removing MOR resulting from the wETH LP position it makes MOR ever more scarce.
This way the PoL to would continue to deepen, and would add even more demand pressure as 75% would be swapped, and make it more scarce.