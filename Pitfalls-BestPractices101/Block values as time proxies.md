# 18 - [Block values as time proxies](Block%20values%20as%20time%20proxies.md)
_block.timestamp_ and _block.number_ are not good proxies (i.e. representations, not to be confused with smart contract proxy/implementation pattern) for time because of issues with synchronization, miner manipulation and changing block times. (see [here](https://swcregistry.io/docs/SWC-116))
___
## Slide Screenshot
![018.png](../images/pitfalls_and_best_practices101/018.png)
___
## Slide Text
- On-chain Time
- block.timestamp
- block.number
- Miner Influence & Synchronization & Unpredictable
- Risk Awareness
- Alternative Oracles
___
## References
- [Youtube Reference](https://youtu.be/OOzyoaYIw2k?t=1607)
___
## Tags