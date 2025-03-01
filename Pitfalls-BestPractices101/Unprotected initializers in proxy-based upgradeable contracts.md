# 95 - [Unprotected initializers in proxy-based upgradeable contracts](Unprotected%20initializers%20in%20proxy-based%20upgradeable%20contracts.md)
Proxy-based upgradeable contracts need to use _public_ initializer functions instead of constructors that need to be explicitly called only once. Preventing multiple invocations of such initializer functions (e.g. via _initializer_ modifier from OpenZeppelin’s _Initializable_ library) is a must. (see [here](https://docs.openzeppelin.com/upgrades-plugins/1.x/writing-upgradeable#initializers) and [here](https://github.com/crytic/slither/wiki/Upgradeability-Checks#initializer-is-not-called))

___
## Slide Screenshot
![095.png](../images/pitfalls_and_best_practices101/095.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags