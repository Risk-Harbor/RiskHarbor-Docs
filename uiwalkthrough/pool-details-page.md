# Pool Details Page

### **Order Box** 

To the right is a box where users interact with the protocol. At the top of that box are four clickable tabs that allow users to navigate between the three types of interactions available to them: **Protect**, **Underwrite**, **Stake**, and **Claim.**

**Protect:** Here, users can purchase policies from the protocol. After entering an amount, the protocol will automatically compute the **premium** based on the available underwriting capital at each price point. These premiums are paid upfront in the credit token.

* _Payout_  - The payout that a policyholder would receive if they filed a valid claim
* _Premium_ - The total premium denominated in the protected token

**Underwrite**

* _Deposit -_ Underwriters can deposit their capital by selecting ‘Deposit’ from the dropdown menu on the underwrite tab. To deposit, the underwriter enters an amount into the text box and chooses a price point to deposit at either by using the slider or entering the price point directly. The user can view their current returns and their optimal returns if policyholders used all of the available capital at that price point.
* _Withdraw -_ Underwriters can withdraw their capital at any time as long as there will continue to be enough underwriting capital at that price point to cover the outstanding policies at that price point. To do this, the user enters the amount of non-utilized underwriter shares that they wish to withdraw and selects the price point at which they want to withdraw.
* _Current Premium_ -The premiums that underwriters will receive for underwriting at that price point given the current utilization
* _Optimal Premium_ - The premiums that underwriters would receive if policyholders utilized 100% of the available underwriting capital at that price point

**Stake** Is a feature that allows underwriters in Risk Harbor to stake their Risk Harbor claim tokens to earn tickets that will be redeemable for Risk Harbor governance tokens in the future. Users who underwrite at lower price points receive higher weights on staking rewards, so be aware that you may receive low staking rewards if you stake at a high price point.

* _Stake -_ Users enter the amount they wish to stake and press stake.
* _Unstake_ - Users can unstake staked capital by entering the amount they wish to withdraw and clicking unstake.
* _Select Position -_ Users can select which positions they want to stake from a dropdown menu.

**Claim**

* _Payout_ - The payout amount denominated in the underwriting token.

### **Key Attributes:**

_Protected Token_ - The claim Token that redeems to the underlying token through the protected DeFi protocol.

_Underlying Token_ - The token that underwriters stake, which is used to pay out valid claims after hacks or attacks occur.

_Currency Token_ - The token that the Protected Token can be claimed for when a hack occurs.

_Default Ratio_ - Once the underlying-to-claim ratio falls below the Default Ratio, policyholders can redeem their claim tokens for underwriting tokens through the Risk Harbor claims mechanism.

_Payout Ratio_ - When a user files a claim, they receive underwriting tokens equal to the protected amount multiplied by the payout ratio.

_Expiration Date_ - The expiration block number and estimated date of expiration

_Other Pools_ - Other relevant pools are displayed here

### **Pool List Page**

This page displays all available pools. In addition, the table of pools lists critical metrics about each pool, such as the Protected Token, Underwriting Token, Premiums, Utilization, and Expiration Date in GMT. A user will also have the ability to sort/filter by each metric as well.

