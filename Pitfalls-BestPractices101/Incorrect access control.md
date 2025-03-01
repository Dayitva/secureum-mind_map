# 4 - [Incorrect access control](Incorrect%20access%20control.md)
Contract functions executing critical logic should have appropriate access control enforced via address checks (e.g. owner, controller etc.) typically in modifiers. 

Missing checks allow attackers to control critical logic. (see [here](https://docs.openzeppelin.com/contracts/3.x/api/access) and [here](https://dasp.co/#item-2))

___
## Slide Screenshot
![04.png](../images/pitfalls_and_best_practices101/004.png)
___
## Slide Text
- Access to Functions
- Public/External Functions
- Addresses: Anyone/Owner/RBAC
- Correct Modifiers/Addresses -> Enforce Access
___
## References
- [Youtube Reference](https://youtu.be/OOzyoaYIw2k?t=411)
___
## Tags