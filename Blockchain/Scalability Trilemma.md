![](https://vitalik.ca/images/sharding-files/trilemma.png)
The scalability trilemma says that there are three properties that a blockchain try to have, and that, **if you stick to "simple" techniques, you can only get two of those three**. The three properties are:

-   **Scalability**: the chain can process more transactions than a single regular node (think: a consumer laptop) can verify.
-   **Decentralization**: the chain can run without any trust dependencies on a small group of large centralized actors. This is typically interpreted to mean that there should not be any trust (or even honest-majority assumption) of a set of nodes that you cannot join with just a consumer laptop.
-   **Security**: the chain can resist a large percentage of participating nodes trying to attack it (ideally 50%; anything above 25% is fine, 5% is definitely _not_ fine).

Now we can look at the three classes of "easy solutions" that only get two of the three:

-   **Traditional blockchains** - including Bitcoin, pre-PoS/sharding Ethereum, Litecoin, and other similar chains. These rely on every participant running a full node that verifies every transaction, and so they have decentralization and security, but not scalability.
-   **High-TPS chains** - including the DPoS family but also many others. These rely on a small number of nodes (often 10-100) maintaining consensus among themselves, with users having to trust a majority of these nodes. This is scalable and secure (using the definitions above), but it is not decentralized.
-   **Multi-chain ecosystems** - this refers to the general concept of "scaling out" by having different applications live on different chains and using cross-chain-communication protocols to talk between them. This is decentralized and scalable, but it is not secure, because an attacker need only get a consensus node majority in one of the many chains (so often <1% of the whole ecosystem) to break that chain and possibly cause ripple effects that cause great damage to applications in other chains.

**Sharding is a technique that gets you all three.** A sharded blockchain is:

-   **Scalable**: it can process far more transactions than a single node
-   **Decentralized**: it can survive entirely on consumer laptops, with no dependency on "supernodes" whatsoever
-   **Secure**: an attacker can't target a small part of the system with a small amount of resources; they can only try to dominate and attack the whole thing

The rest of the post will be describing how sharded blockchains manage to do this.