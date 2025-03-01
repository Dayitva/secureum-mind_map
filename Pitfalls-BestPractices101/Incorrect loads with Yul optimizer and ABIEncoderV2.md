# 82 - [Incorrect loads with Yul optimizer and ABIEncoderV2](Incorrect%20loads%20with%20Yul%20optimizer%20and%20ABIEncoderV2.md)
The Yul optimizer incorrectly replaces _MLOAD_ and _SLOAD_ calls with values that have been previously written to the load location. This can only happen if ABIEncoderV2 is activated and the experimental Yul optimizer has been activated manually in addition to the regular optimizer in the compiler settings. This is due to a compiler bug introduced in _v0.5.14_ and fixed in _v0.5.15_. (see [here](https://docs.soliditylang.org/en/v0.8.9/bugs.html))

___
## Slide Screenshot
![082.png](../images/pitfalls_and_best_practices101/082.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags