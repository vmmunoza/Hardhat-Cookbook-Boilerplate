# Hardhat-Cookbook-Boilerplate
Steps to run, compile and deploy a smart contract on Metis, using the Hardhat boilerplate of Cookbook


## Steps:

1. Choose a contract from the Cookbook library and download the Hardhat version. 
2. Open the downloaded folder with Remix, open a new terminal and run `npm install`
3. Edit the .env file adding your Wallet private key.
4. Uncomment the Metis piece of code on the hardhat.config.js file
5. Go to the deploy.js file and edit the constructorArgs with parameter set according to the specic case of your contract.
6. Compile with the command `npx hardhat compile`
7. Deploy to Metis Andromeda mainnet with the command `npx hardhat run --network metisAndromeda scripts/deploy.js`
8. Check the contract deployment on the Andromeda or Routescan Explorer and paste the contract address you get on your terminal after deploy.



# Cookbook.dev Readme info:

## Find any smart contract, build your project faster

Get ready-to-use Hardhat projects directly from https://www.cookbook.dev/?utm=code



## Please follow these 4 steps for a local deploy


### Step 1: Install

Run "npm i " to install dependencies in package.json


### Step 2: Compile

Run "npm run compile" to compile your contracts.

### Step 3: Add arguments

Add arguments to the constructorArgs array in the deploy.js file and save.  If you do not need any arguments leave the array empty.

### Step 4: Deploy to Local

Run "npm run deploy" to deploy your contracts to a local VM for testing.


## Please follow these steps for a testnet deploy, after compiling


### Step 1: Fill out your .env file

Fill out your .env file with your infura key of your chosen testnet and the private key from the account you wish to deploy from. DO NOT share this private key with anyone else, and be sure that your .env is ignored by .gitignore so that it is not pushed to github. 

NOTE: Use this calculator: https://www.alchemy.com/gwei-calculator in order to calculate any token values and get the correct precision. 1 ETH = 1000000000000000000 WEI


### Step 2: Deploy to a testnet using an rpc

Run "npx hardhat run --network (your-network) scripts/deploy.js" in your terminal if you are using a testnet. Please replace NAME_OF_NETWORK with the name of the testnet you are using by it's name in the hardhat.config.js file.


Example Contracts and Projects

- [Simple Token](https://www.cookbook.dev/contracts/simple-token?utm=code)
- [Azuki EFC721A NFT](https://www.cookbook.dev/contracts/Azuki-ERC721A-NFT-Sale?utm=code)
- [Uniswap Labs](https://www.cookbook.dev/libraries/Uniswap-V4-HookBook?utm=code)

[Search for 100s of other contracts](https://www.cookbook.dev/search?q=&categories=Contracts&sort=popular&filter=&page=1&utm=code)
