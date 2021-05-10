---
description: This contract communicates with the defaultector contract and manages payouts
---

# Claims

## Inheritance

Claims.sol inherits Storage and MarketStatus

## Events

{% tabs %}
{% tab title="ClaimTimeChanged" %}
This event is fired when a successful claim is filed and the _claimTime_ variable is changed to the current block number.

| Data Type | Variable |
| :--- | :--- |
| uint256 | oldClaimTime |
| uint256 | newClaimTime |
{% endtab %}
{% endtabs %}

## Methods

### checkAndPayDefault

Connects with defaultector contract and attempts to redeem creditTokens for underlyingTokens

{% tabs %}
{% tab title="Params" %}
| Data Type | Variable Name | Description |
| :--- | :--- | :--- |
| uint256 | \_amount | Amount of protected tokens that are attempting to be claimed |
{% endtab %}

{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| bool | If a payout event has been triggered |
| uint256 | Amount of currencyTokens paid out to the policyholder |
{% endtab %}
{% endtabs %}

```javascript
function getTotalCapacity() public view returns (uint256)
```



