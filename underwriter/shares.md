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

**Returns:** \(uint256\) _Multiplication unit_

```javascript
function getUnits() public view returns (uint256)
```

### 

### getSharePrice

Returns the current price per pool share

**Returns:** \(uint256\) _Price per share_

```javascript
function getSharePrice() public view returns (uint256)
```

### 

### buyShares

Buy shares from the pool

**Params:** \(uint256\) \_amount _Amount of currencyToken to buy shares with_

**Returns:** \(uint256\) _Number of shares minted_

```javascript
function buyShares(uint256 _amount) internal returns (uint256)
```

### 

### sellShares

Sell shares to the pool and also grabs any swapped credit tokens and gov tokens

**Params:** \(uint256\) \_shares Amount of shares to sell

**Returns:** \(uint256\) _Amount of underlying tokens paid out_

**Returns:** \(uint256\) _Amount of credit tokens paid out_

```javascript
function sellShares(uint256 _shares) internal returns (uint256, uint256)
```

