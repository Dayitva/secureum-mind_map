# 6 - [Unprotected call to selfdestruct](Unprotected%20call%20to%20selfdestruct.md)
A user/attacker can mistakenly/intentionally kill the contract. 

Protect access to such functions. 

(see [here](https://swcregistry.io/docs/SWC-106))

___
## Slide Screenshot
![06.png](../images/pitfalls_and_best_practices101/006.png)
___
## Slide Text
- `selfdestruct()` Unprotected
- Destroy/Remove Contract
- Unauthorized Call -> Contract Killed
- Access Control -> Authorized Users
___
## References
- [Youtube Reference](https://youtu.be/OOzyoaYIw2k?t=604)
___
## Tags
[selfdestruct](../Solidity101/selfdestruct.md)