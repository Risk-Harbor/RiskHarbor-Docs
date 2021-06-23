# Pool Details Page

### **Order Box** 

On the right side of the screen users are presented with a box that allows them to interact with the protocol. At the top of that widget are four clickable tabs that allow users to navigate between the three types of interactions available to them: **Protect**, **Underwrite**, **Stake**, and **Claim**

**Protect:** Here users can purchase policies from the protocol. After entering an amount, the protocol will automatically compute the **premium** based on the available underwriting capital at each price point. This will be paid upfront in the credit token.

* _Payout_ The payout that a policyholder would receive if they filed a valid claim.
* _Premium_ The total premium denominated in the protected token

**Underwrite**

* _Deposit -_ Underwriters can deposit their capital by selecting ‘Deposit’ from the dropdown menu on the underwrite tab. To deposit, the underwriter enters an amount into the text box and chooses a price point to deposit at either by using the slider or entering the price point directly. The user will be able to view their returns as well as their optimal returns if policyholders used all of their available capital at that price point.
* _Withdraw -_ Underwriters can withdraw their capital at any time as long as there will continue to be enough underwriting capital at that price point to cover the outstanding policies at that price point. To do this, the user simply enters the amount of non-utilized underwriter shares that they wish to withdraw and selects the price point that they wish to withdraw at.
* _Current Premium_ The premiums that underwriters will receive for underwriting at that price point given the current utilization.
* Optimal Premium The premiums that underwriters would receive if policyholders utilized 100% of the available underwriting capital at that price point.

**Stake** Is a feature that allows underwriters in Risk Harbor to stake their Risk Harbor claim tokens in order to earn tickets that will be redeemable for Risk Harbor governance tokens in the future. Users who underwrite at lower price points receive higher weights on staking rewards so be aware that if you stake at a high price point you may receive low staking rewards.

* _Stake -_ Users enter the amount they wish to stake and press stake.
* _Unstake_ - Users can unstake staked capital by entering the amount that they wish to withdraw and clicking unstake.
* _Select Position -_ Users can select which positions they want to stake from a dropdown menu.

**Claim**

* _Payout_ - The payout amount denominated in the underwriting token.

### **Key Attributes:**

_Protected Token_ - The claim Token that can be redeemed for the underlying token through the protected DeFi protocol.

_Underlying Token_ - The token deposited in the protocol that the Protected token can be redeemed for.

_Currency Token_ - The token that the Protected Token can be claimed for when a hack occurs.

_Default Ratio_ - Once the underlying-to-claim ratio falls below the Default Ratio, policyholders can redeem their claim tokens for underwriting tokens through the Risk Harbor claims mechanism.

_Payout Ratio_ - When a user files a claim, they receive underwriting tokens equal to the protected amount multiplied by the payout ratio.

_Expiration Date_ - The expiration block number and estimated date of expiration

_Other Pools_ - Other relevant pools are displayed here

### **Pool List Page**

This page will portray all available pools that a user can participate in. The table of pools lists key metrics about each pool such as the Protected Token, Underwriting Token, Premiums, Utilization, and Expiration Date in GMT. A user will also have the ability to sort/filter by each metric as well.

