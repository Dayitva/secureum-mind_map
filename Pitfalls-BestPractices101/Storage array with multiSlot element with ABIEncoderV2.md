# 79 - [Storage array with multiSlot element with ABIEncoderV2](Storage%20array%20with%20multiSlot%20element%20with%20ABIEncoderV2.md)
Storage arrays containing structs or other statically sized arrays are not read properly when directly encoded in external function calls or in _abi.encode()_. This is due to a compiler bug introduced in _v0.4.16_ and fixed in _v0.5.10_. (see [here](https://docs.soliditylang.org/en/v0.8.9/bugs.html))

___
## Slide Screenshot
![079.png](../images/pitfalls_and_best_practices101/079.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags