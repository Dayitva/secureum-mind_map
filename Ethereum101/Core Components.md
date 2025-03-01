# 8 - [Core Components](Core%20Components.md)

Ethereum’s core components:
  
1. P2P network: Ethereum runs on the Ethereum main network, which is addressable on TCP port 30303, and runs a protocol called ÐΞVp2p.
2. [Transaction](Transaction.md)s: Ethereum transactions are network messages that include (among other things) a sender, recipient, value, and data payload.
3. State machine: Ethereum state transitions are processed by the Ethereum Virtual Machine [EVM](EVM.md), a stack-based virtual machine that executes bytecode (machine-language instructions). [EVM](EVM.md) programs, called "smart contracts," are written in high-level languages (e.g., Solidity or Vyper) and compiled to bytecode for execution on the [EVM](EVM.md).
4. Data structures: Ethereum’s state is stored locally on each node as a database (usually Google’s LevelDB), which contains the transactions and system state in a serialized hashed data structure called a Merkle Patricia Tree.

___
## Slide Screenshot
![008.png](../images/ethereum101/008.png)
___
## Slide Text
- Transaction: Sender, [Recipient](Recipient.md), [Value](Value.md), [Data](Data.md)
- State Machine -> [EVM](EVM.md)
- HLLs (Solidity) -> Bytecode
- Data Structures
- Merkle Patricia Tree
___
## References
- [Ethereum Book: Chapter 01 - What is Ethereum](https://github.com/ethereumbook/ethereumbook/blob/develop/01what-is.asciidoc)