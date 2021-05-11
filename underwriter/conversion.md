---
description: >-
  This contract allows for the conversion of any amount of tokens between
  creditToken and currencyToken equivalents.
---

# Conversion

## Inheritance

Conversion.sol inherits Storage

## Methods

### creditToCurrency

Convert amount of creditTokens to currencyToken

{% tabs %}
{% tab title="Params" %}
| Data Type | Variable Name | Description |
| :--- | :--- | :--- |
| uint256 | \_amount | Amount of creditTokens |
{% endtab %}

{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of currencyTokens |
{% endtab %}
{% endtabs %}

### 

### currencyToCredit

Convert amount of currencyToken to creditTokens

{% tabs %}
{% tab title="Params" %}
| Data Type | Variable Name | Description |
| :--- | :--- | :--- |
| uint256 | \_amount | Amount of currencyTokens |
{% endtab %}

{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of creditTokens |
{% endtab %}
{% endtabs %}

```javascript
function creditToCurrency(uint256 _amount) public view returns (uint256)
```

