# Purchasing & Filing a Claim

To purchase protection on Risk Harbor, you need to already own part of the position that you want to protect since premiums are paid in the credit token that you receive when you enter a position in the protected protocol.  For example, if you want to purchase protection in the BarnBridge cUSDC pool you need to have some bb\_cUSDC already. 

### Step 1\) Navigate to the pool page

Head to the Risk Harbor home page [https://app.riskharbor.com/home](https://app.riskharbor.com/home)

![Risk Harbor Home Page](../.gitbook/assets/image%20%2812%29.png)

Navigate to the pool page that you want to purchase from

![Barnbridge Compound Pool Page](../.gitbook/assets/image%20%2818%29.png)

You should be on the **Protect** tab automatically but if not, click on it in the box on the right. 

### Step 2\) Purchase

Enter the amount of protection you want and click Purchase. This is a two-step process. First, you will need to approve the transfer of the premiums to the contract and then approve the purchase function



## Filing a claim

### Step 1\) Click on the claim tab

Click claim in the box on the right and enter the amount of protection that you want to claim. 

![](../.gitbook/assets/image%20%2829%29.png)

### Step 2\) Approve Credit Token Transfer

To prevent flash loan attacks, filing a claim is a three-step process that must take place over more than one block. First, the user approves sending their credit tokens to the contract.

### Step 3\) Start Swap

Then the user starts the swap and the protocol checks the validity of the claim.

### Step 4\) Finish Swap

Finally, the user calls finish swap and the protocol sends the currency tokens to the claimant.



