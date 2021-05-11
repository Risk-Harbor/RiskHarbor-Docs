---
description: This contract tracks the capacity and utilization of the protection pool
---

# Utilization

## Inheritance

Utilization.sol inherits Storage and [Conversion](conversion.md)

## Methods

### getTotalCapacity

Sees how much of the pool is being utilized in terms of currency tokens

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of currency token utilized |
{% endtab %}
{% endtabs %}

```javascript
function getTotalCapacity() public view returns (uint256)
```



### getTotalCapacityInCredit

Sees how much of the pool is being utilized in terms of credit tokens

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of currency token utilized |
{% endtab %}
{% endtabs %}

```javascript
function getTotalCapacityInCredit() external view returns (uint256)
```

### 

### getUtilizedAmount

Sees how much of the pool is being utilized in terms of currency tokens tokens

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of currency token utilized |
{% endtab %}
{% endtabs %}

```javascript
function getUtilizedAmount() public view returns (uint256)
```



### getUtilizedAmountInCredit

Sees how much of the pool is being utilized in terms of credit tokens 

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | _Amount of currency token utilized in creditTokens_ |
{% endtab %}
{% endtabs %}

```javascript
function getUtilizedAmount() public view returns (uint256)
```



### getWithdrawable

Sees how much of the currency pool token's are withdrawable

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| uint256 | Amount of currency tokens that you can withdraw |
{% endtab %}
{% endtabs %}

```javascript
function getUtilizedAmount() public view returns (uint256)
```



### isFull

Checks if pool is fully utilized or not

{% tabs %}
{% tab title="Returns" %}
| Data Type | Description |
| :--- | :--- |
| bool | If pool is full |
{% endtab %}
{% endtabs %}

```javascript
function getUtilizedAmount() public view returns (uint256)
```

