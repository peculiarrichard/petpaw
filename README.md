### PetPaw - A decentralized social media application for pet lovers to mint their pets as NFTs. Users can browse cute photos of their favorite pets, see details of a specific pet, create a post and earn NFTs.

Installation & Set Up 

1. First step is to add metamask plugin to your supported browser (chrome).

There may be problems with installing certain packages if they are not well-maintained. If you encounter any issues during the installation process, you can check some developer communities for help or reach out to me.

2. Create a Polygon Matic testnet in metasmask. Open your metamask extension, click on Settings > Networks >Add Network > save

Fill out the following information:
Network Name: MATIC Mumbai
New RPC URL: https://rpc-mumbai.matic.today
Chain ID: 80001
Current symbol: MATIC
Block explorer URL: https://mumbai-explorer.matic.today

3. You will need to fund this wallet. Visit https://faucet.matic.network/ to access free funds. Just input your wallet address and you will receive about 0.2 MATIC in not time. 

4. Next step is to download the repository. You can clone directly from github with the command: git clone {repo link}
In your terminal, cd petpaw

5. install node dependencies with 

```
npm install
```
6. In your terminal, make sure you are in the project root directory and run the command 
```
truffle compile.
```
You should see something like 
Compiled successfully using:
  -solc version

7. We are going to use the GUI method to set up lacal blockchain with Truffle Ganache 
> If you don't have Ganache installed, visit https://trufflesuite.com/ganache/ to download
> After installation, create a workspace and add the truffle-config.js file of this project under "add project"
> When the workspace is open, the local ganache blockchain network should be active on the specified port and network ID.
Run this command:
```
truffle migrate
```
8. Deploy to the Polygon Mumbai Testnet by running the command:
```
truffle migrate --network matic
```

If you're deploying it for the second time or more, use the --reset flag to avoid JSON errors: `truffle migrate --network matic --reset`.

9. Run `npm start` to start the frontend application on `localhost:3000`

10. You should now be able to interact with the DApplication. 

## How it was made
PetPaw makes use of the following softwares:
* Deployed smart contracts on the `Polygon (Matic)` Mumbai test network.
* `Truffle & MetaMask` for testing
* Storage of files (pet pictures) with the `IPFS NFTStorage` [IPFS](https://nft.storage/) platform.
* `Solidity ` for smart contract.
* `OpenZeppelin` Library to customize smart contract
* Develop, deploy, and run tests the application with `Ganache` (local blockchain)
* `React Js` to create components for single-page applications.
* `Material-UI` to build faster, beautiful, and more accessible React applications.

## Developer

- [Peculiar Richard](https://github.com/peculiarrichard)

## Refrences
-[Figment](https://learn.figment.io/)