# Filing a Claim

Filing a claim on risk harbor requires three steps. First, the Policyholder approves a claim token transfer. Second, the Policyholder transfers their claim tokens to the Undewriter Contract by calling the`startSwap`function. Third, after waiting for at least one block, they call the`finishSwap`function. Finally, the `finishSwap` function checks that the claim is valid and if it is, sends the claim tokens to the underwriters and sends the payout to the policyholder. 

![](../.gitbook/assets/image%20%284%29.png)

Policyholders can file their claims directly through the web application.

