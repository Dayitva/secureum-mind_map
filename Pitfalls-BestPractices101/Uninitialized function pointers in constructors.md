# 69 - [Uninitialized function pointers in constructors](Uninitialized%20function%20pointers%20in%20constructors.md)

Calling uninitialized function pointers in constructors of contracts compiled with _solc_ versions _0.4.5-0.4.25_ and _0.5.0-0.5.7_ lead to unexpected behavior because of a compiler bug. (see [here](https://github.com/crytic/slither/wiki/Detector-Documentation#uninitialized-function-pointers-in-constructors))
___
## Slide Screenshot
![069.png](../images/pitfalls_and_best_practices101/069.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags