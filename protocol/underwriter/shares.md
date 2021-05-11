---
description: >-
  The shares system manages the creation and redemption of share tokens that
  track deposits by underwriters.
---

# Shares

## Inheritance

Shares.sol inherits [ERC20Upgradeable](https://github.com/OpenZeppelin/openzeppelin-contracts-upgradeable/blob/master/contracts/token/ERC20/ERC20Upgradeable.sol), Storage, and [Conversion](conversion.md)

## Methods

### getUnits

Returns multiplication unit used for share price calculations to avoid floating point math

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Multiplication unit |
{% endtab %}
{% endtabs %}

```javascript
function getUnits() public view returns (uint256)
```

### 

### getSharePrice

Returns the current price per pool share

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Price Per Share |
{% endtab %}
{% endtabs %}

```javascript
function getSharePrice() public view returns (uint256)
```

### 

### buyShares

Buy shares from the pool

{% tabs %}
{% tab title="Params" %}
| Data Type | Variable Name | Description |
| :--- | :--- | :--- |
| uint256 | \_amount | Amount of currencyToken to buy shares with |
{% endtab %}

{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Number of shares minted |
{% endtab %}
{% endtabs %}

```javascript
function buyShares(uint256 _amount) internal returns (uint256)
```

### 

### sellShares

Sell shares to the pool and also grabs any swapped credit tokens and gov tokens

{% tabs %}
{% tab title="Params" %}
| Data Type | Variable Name | Description |
| :--- | :--- | :--- |
| uint256 | \_shares | Amount of shares to sell |
{% endtab %}

{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of underlying tokens paid out |
| uint256 | Amount of credit tokens paid out |
{% endtab %}
{% endtabs %}

```javascript
function sellShares(uint256 _shares) internal returns (uint256, uint256)
```

