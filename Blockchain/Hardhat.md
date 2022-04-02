```
const domainContractFactory = await hre.ethers.getContractFactory('Domains');
```
This will actually compile our contract and generate the necessary files we need to work with our contract under the artifacts directory.

```
const domainContract = await domainContractFactory.deploy();
```
What's happening here is Hardhat will create a local Ethereum network for us, but just for this contract. Then after the script completes, it will destroy that local network. So, every time you run the contract it will be a fresh blockchain. Whats the point? It's kinda like refreshing your local server every time so you always start from a clean slate which makes it easy to debug errors.

```
await domainContract.deployed();
```
We'll wait until our contract is officially mined and deployed to our local blockchain! That's right, hardhat actually creates fake "miners" on your machine to try its best to imitate the actual blockchain.