# 39 - [Dangerous shadowing](Dangerous%20shadowing.md)
Local variables, state variables, functions, modifiers, or events with names that shadow (i.e. override) builtin Solidity symbols e.g. _now_ or other declarations from the current scope are misleading and may lead to unexpected usages and behavior. (see [here](https://github.com/crytic/slither/wiki/Detector-Documentation#builtin-symbol-shadowing))
___
## Slide Screenshot
![039.png](../images/pitfalls_and_best_practices101/039.png)
___
## Slide Text
- Solidity Built-in Shadowing
- Built-in: now, assert, etc.
- Names: Variables/Functions/Modifiers
- Override Behavior -> Dangerous/Unexpected
___
## References
- [Youtube Reference](https://youtu.be/fgXuHaZDenU?t=1449)
___
## Tags