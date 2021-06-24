# How Risk Harbor Works

Each Risk Harbor **Policy** manages a market for a single token deposited in a specific decentralized finance protocol. For example, one Risk Harbor policy allows users to underwrite risk for USDC tokens deposited in Compound. There are two types of agents in each market: [**Underwriters**](https://www.investopedia.com/terms/u/underwriter.asp#:~:text=Key%20Takeaways-,An%20underwriter%20is%20any%20party%20that%20evaluates%20and%20assumes%20another,types%20of%20debt%20security%20trading.) ****and [**Potential Policyholders**](https://www.sciencedirect.com/topics/social-sciences/policyholder)**.** Underwriters agree to cover a Potential Policyholder's loss in the event of a hack or attack on the protocol in exchange for premiums paid upfront.  ****This type of financial derivative is known in traditional financial markets as a [**Credit Default Swap \(CDS\)**. ](https://www.investopedia.com/terms/c/creditdefaultswap.asp)

Anyone can underwrite a Policy as long as they are willing to take on the risk. Similarly, Anyone can purchase a policy as long as they are willing to pay the premium.

![Protocol Diagram](../.gitbook/assets/image%20%285%29.png)

The automated claim evaluation process tracks the evolution of public system state variables on the blockchain to determine whether or not to pay out a claim. Those variables differ from protocol to protocol and therefore must also vary from Policy to Policy. For example, the Policy covering USDC in Compound tracks the ratio of outstanding claim tokens \(cUSDC\) to USDC. But a protocol that covered Eth in AAVE would track different system state variables. 

In general, the claim is valid when The Underlying-To-Claim-Ratio Falls below a predetermined `loss_threshold`:

$$
\text{Underlying-To-Claim-Ratio} = \frac{\text{UnderlyingTokens}}{\text{ClaimTokens}}<\text{Loss-Threshold}
$$







\*\*\*\*

