# PoS & EVM Compatibility

The crux of developing on Polygon is simple: develop the exact way that you do on Ethereum, except change the deployment RPC that you're using to that of Polygon mainnet / mumbai. The smart contracts are almost all the same\*, the frontends are almost all the same\*.

**Regarding consensus**, Polygon validators continuously monitor a contract on Ethereum chain called _**StateSender**_. Each time a registered contract on Ethreum chain calls this contract, it emits an event. Using this event Polygon validators relay the data to another contract on Polygon chain. This _**StateSync**_ mechanism is used to send data from Ethereum to Polygon. Polygon validators also periodically submit a hash of all transactions on Polygon chain to Ethereum chain. This _**Checkpoint**_ can be used to verify any transaction that happened on Polygon. Once a transaction is verified to have happened on Polygon chain, action can be taked accordingly on Ethereum.

#### **🦕 Already have a dApp?**

*   **Migrating from Ethereum chain (or any EVM based chain for that matter)**

    Deploy all your smart contracts directly on Polygon chain. You don't have to worry about the underlying architecture, as long as it is EVM compatible!

    [Deploying your dApp on Polygon](https://docs.polygon.technology/docs/integrate/quickstart)
*   **Using Polygon as a faster transactions layer**

    Using Polygon as a transactions layer in your DApp deployed on Mainnet, you can get started with getting your tokens mapped by us.
* **To reduce fees even further,** check out this [guide](https://docs.polygon.technology/docs/develop/metatransactions/getting-started).

#### **🌱 Building a new dApp on Polygon?**

* Feel free to check out some of the [learning resources](../readme/cooking-with-polygon/learning-resources.md) or go straight down to [recipes](../recipes/) to get started with example dApps.



\*Note: oracle contracts and token addresses may be different from chain to chain. Please be sure to use the right contract or token address for Polygon Mainnet / Mumbai when deploying.
