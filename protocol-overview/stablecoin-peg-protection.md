# Stablecoin Peg Protection

Tether’s legal troubles, FEI’s April price fluctuations, USDC’s delayed may attestations, and DAI’s flash loan vulnerabilities all demonstrate a troubling fact: the so-called ‘stablecoins’, on which the entire DeFi system runs on, aren't all that stable after all. This is particularly concerning for institutional investors who have a lower risk appetite than the common De-Fi power user with a high risk appetite. Without protection, the risk of stablecoins losing their pegs alone might be enough to prevent these more risk-sensitive investors from entering the DeFi space.

Risk Harbor’s newest offering: stablecoin peg protection promises to help investors manage the risk of stablecoin peg loss by offering risk transfer financial derivatives that allow users to exchange their devalued stablecoin for a different stablecoin if the one that they are holding loses its peg. Purchasing this protection means the policyholder is exposed to stable coin peg loss only if both the underlying stablecoin and the paid-out stablecoin lose their peg simultaneously.

**How It Works:**

Risk Harbor stablecoin protection relies on Uniswap v3’s Time Weighted Average Price \(TWAP\) oracle to evaluate claims. Whenever a claim is filed, the protocol queries Uniswap, computes the TWAP over the last hour based on that data, and checks if the TWAP is below the default price. If it is, then the claim is eligible to be paid out, otherwise, the claim is rejected.

**Computing the Time Weighted Average Price:**

In Uniswap v3, ticks are the prices that can act as upper and lower bounds on concentrated LP positions. Since these ticks are quite granular \(about 1 every basis point\), they act as a reasonable proxy for prices. They are particularly desirable as a stand-in for prices in a time-weighted average since compact price data means lower storage requirements and lower storage requirements lower gas costs. UniswapV3 improves on these storage requirements even further by first taking the $$\log_{1.0001}$$ of the tick before storing.

Taking the log has the additional benefit of making geometric mean computation much more gas efficient. The geometric mean is preferable to the arithmetic mean in this context since, as the Uniswap white paper mentions in a footnote, one of the common ways to model trading pairs are using geometric Brownian motion, and taking arithmetic means of such processes would result in overweighting changes at high price points where small percentage changes in price mean large absolute changes.

When computing the geometric mean itself, Uniswap offers another convenient solution. Instead of storing tick prices at each block, which would require significant computation for the smart contract calling the oracle in order to compute the TWAP from the data, UniswapV3 stores cumulative time-weighted ticks. This simplifies computing the geometric mean to a simple fraction

$$
\log_{1.0001}(\text{TWAP}) = \frac{c_2-c_1}{t_2-t_1}
$$

Which can be simplified to

$$
\text{TWAP} = 1.0001^{\frac{c_2-c_1}{t_2-t_1}}
$$

**Protection against impermanent loss for LPs in stablecoin pools**

One potential group of policyholders are liquidity providers on stablecoin only pools in decentralized exchanges. Not only do these LPs hold significant value in stablecoins in order to provide liquidity, but they are also exposed to the even greater potential downside from the loss of a stablecoin peg due to impermanent loss. This is particularly relevant to curve LPs who are providing liquidity to pools with more than two assets although it also applies to LPs in Uniswap pairs since it becomes more acute as liquidity becomes more concentrated around the stable price point. These LPs might wish to overinsure to protect further against impermanent loss. Since a stablecoin losing its peg would mean that their LP tokens would redeem to more of the stablecoin that had lost its peg.

**Protecting Non-USD stables**

This approach will seamlessly extend to other stablecoins on the ethereum network such as the bitcoin stables wBTC, renBTC, and sBTC or euro stablecoins.

