# 24 - [Function Mutability](Function%20Mutability.md)
Function Mutability Specifiers: [Functions](Functions.md) can be specified as being `pure` or view:

1. `view` functions can read contract state but cannot modify it. This is enforced at runtime via `STATICCALL` opcode. The following are considered state modifying:
	1. Writing to [state variables](State%20Variables.md) 
	2. [Emitting](Emit.md) events
	3. Creating other contracts 
	4. Using [selfdestruct](selfdestruct.md) 
	5. Sending Ether via calls 
	6. Calling any function not marked `view` or `pure` 
	7. Using [low-level calls](Low-level%20Calls.md) 
	8. Using inline assembly that contains certain opcodes.
2. `pure` functions can neither read contract state nor modify it. The following are considered reading from state: 
	1. Reading from [state variables](State%20Variables.md) 
	2. Accessing `address(this).balance` or `<address>.balance`
	3. Accessing any of the members of `block`, `tx`, `msg` (with the exception of `msg.sig` and `msg.data`) 
	4. Calling any function not marked `pure` 
	5. Using inline assembly that contains certain opcodes.

3. It is not possible to prevent functions from reading the state at the level of the [EVM](../Ethereum101/EVM.md). It is only possible to prevent them from writing to the state via `STATICCALL`. Therefore, only `view` can be enforced at the EVM level, but not `pure`.

___
## Slide Screenshot
![024.png](../images/solidity101/024.png)
___
## Slide Deck
- View or Pure
- View: Read State
	- Not Modify -> `STATICCALL`
- Pure: Not Modify
	- Not Read -> !EVM
- Mutability: Write/Read
	- Security Implications
___
## References
- [Youtube Reference](https://youtu.be/TCl1IcGl_3I?t=326)
___
## Tags
[System Operations](../Ethereum101/System%20Operations.md)
[Solidity By Example - View and Pure Functions](https://solidity-by-example.org/view-and-pure-functions/)
___
## Solidity by Example
```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.3;  
contract ViewAndPure {
	uint public x = 1;  
	
	// Promise not to modify the state.
	function addToX(uint y) public view returns (uint) {
		return x + y;
	}
	
	// Promise not to modify or read from the state.
	function add(uint i, uint j) public pure returns (uint) {
		return i + j;
	}
}
```