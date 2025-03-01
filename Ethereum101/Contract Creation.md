# 42 - [Contract Creation](Contract%20Creation.md)

Contract creation transactions are sent to a special destination address called the zero address i.e. `0x0`. 

A contract creation transaction contains a data payload with the compiled bytecode to create the contract. 

An optional ether amount in the [Value](Value.md) field will create the new contract with a starting balance.

___
## Slide Screenshot
![042.png](../images/ethereum101/042.png)
___
## Slide Text
- Tx Result -> Creation [Transaction](Transaction.md)
- Create tx -> Sent to special 0 address (0x0)
- Data Payload -> Contract Bytecode
- Value -> Optional Starting Contract Ether Balance
 ___
## References
- [EIP-170: Contract code size limit](https://eips.ethereum.org/EIPS/eip-170)
- [Youtube Reference](https://youtu.be/ltvTIr4K63s?t=77)