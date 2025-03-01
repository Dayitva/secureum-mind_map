# 100 - [Function ID collision between proxy, implementation in proxy-based upgradeable contracts](Function%20ID%20collision%20between%20proxy,%20implementation%20in%20proxy-based%20upgradeable%20contracts.md)
Malicious proxy contracts may exploit function ID collision to invoke unintended proxy functions instead of delegating to implementation functions. Check for function ID collisions. (see [here](https://github.com/crytic/slither/wiki/Upgradeability-Checks#functions-ids-collisions) and [here](https://forum.openzeppelin.com/t/beware-of-the-proxy-learn-how-to-exploit-function-clashing/1070))
___
## Slide Screenshot
![0100.png](../images/pitfalls_and_best_practices101/100.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags