# 50 - [Critical address change](Critical%20address%20change.md)
Changing critical addresses in contracts should be a two-step process where the first transaction (from the old/current address) registers the new address (i.e. grants ownership) and the second transaction (from the new address) replaces the old address with the new one (i.e. claims ownership). 

This gives an opportunity to recover from incorrect addresses mistakenly used in the first step. If not, contract functionality might become inaccessible. (see [here](https://github.com/OpenZeppelin/openzeppelin-contracts/issues/1488) and [here](https://github.com/OpenZeppelin/openzeppelin-contracts/issues/2369))
___
## Slide Screenshot
![050.png](../images/pitfalls_and_best_practices101/050.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags