# 78 - [Dynamic constructor arguments clipped with ABIEncoderV2](Dynamic%20constructor%20arguments%20clipped%20with%20ABIEncoderV2.md)
A contract's constructor which takes structs or arrays that contain dynamically sized arrays reverts or decodes to invalid data when ABIEncoderV2 is used. This is due to a compiler bug introduced in _v0.4.16_ and fixed in _v0.5.9_. (see [here](https://docs.soliditylang.org/en/v0.8.9/bugs.html))

___
## Slide Screenshot
![078.png](../images/pitfalls_and_best_practices101/078.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags