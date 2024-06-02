
# CrowdFunding dApp


https://github.com/boradesanket13/FundSeed/assets/79108273/9c5be52c-a316-496c-984a-15c6e25e2100


This is a decentralized crowdfunding application with NextJS and Solidity. In this dapp peoples can create campaigns or donate to them.

## :bulb: Features

- Dark Theme
- Responsive UI
- Wallet Authentication
- Create Campaign
- Donate or Withdraw Ethereum
- Decentralized

## :hammer_and_wrench: Built With

- [Solidity](https://soliditylang.org/) - Smart Contract Language
- [React](https://reactjs.org/) - JavaScript library for UI
- [NextJS](https://nextjs.org/) - React Framework
- [TailwindCSS](https://tailwindcss.com/) - CSS Framework
- [Hardhat](https://hardhat.org/) Ethereum Development Environment
- [Waffle](https://ethereum-waffle.readthedocs.io/en/latest/) Smart Contract Test Library
- [Ethers](https://docs.ethers.org/v5/) Smart Contract Interaction Library
- [React Icons](https://react-icons.github.io/react-icons/) - Icon Library


## :camera_flash: Screenshots

## 🚀Home Page
![1](https://github.com/boradesanket13/FundSeed/assets/79108273/bd895376-d4ef-4756-9c23-0a27415dfa86)

## 🚀Campaigns Page for Donators
![2](https://github.com/boradesanket13/FundSeed/assets/79108273/ed852e28-af7f-4d09-87fe-dda50893e1d1)

![3](https://github.com/boradesanket13/FundSeed/assets/79108273/c1febe70-4c83-493f-987f-6b7e9526cd3f)

## 🚀Single Campaign Page
![4](https://github.com/boradesanket13/FundSeed/assets/79108273/4ce1e33d-d3de-4b15-9d3a-529b690da8b4)

## 🚀Camapign Page for Fundraisers
![5](https://github.com/boradesanket13/FundSeed/assets/79108273/6bb78683-ec9a-4565-9baf-93a0a970bf06)

## 🚀Campaign Creation Page
![6](https://github.com/boradesanket13/FundSeed/assets/79108273/8a1c5056-b58a-43f8-97db-f0eaac17e4a9)

## 🚀Creaing the Campaign
![7](https://github.com/boradesanket13/FundSeed/assets/79108273/7af01052-5323-45dd-9313-dad2568f9f83)


## :triangular_flag_on_post: Getting Started

1. First of all you need to clone the repository
```shell
git clone https://github.com/boradesanket13/FundSeed.git
```
2. Install the dependencies in client folder
```shell
cd client
npm i
```

3. Install the dependencies in smart-contract folder
```shell
cd ..
cd smart-contract
npm i
```

4. After doing this you must create a project on [alchemy.com](alchemy.com) to assign the following environment variables.
5. [Get your Metamask private key](https://support.metamask.io/managing-my-wallet/secret-recovery-phrase-and-private-keys/how-to-export-an-accounts-private-key/#:~:text=On%20the%20'Account%20details'%20page,private%20key%20to%20your%20clipboard.)
6. Create .env file in client folder in below mentioned format 
```shell
NEXT_PUBLIC_API_BASE_URL=API url (You can use this: http://localhost:3000/api)
NEXT_PUBLIC_PROVIDER_URL=Alchemy url with your API key (For example: https://eth-sepolia.g.alchemy.com/v2/xxxxxxxxxxxxxxx)
NEXT_PUBLIC_CONTRACT_ADDRESS=Address of your contract (You will get this after deploy your contract)
NEXT_PUBLIC_PRIVATE_KEY=Your Metamask Private Key (Get it from point 5)
```

6. Create .env file in smart-contract in below mentioned format
```shell
ACCOUNT_PRIVATE_KEY=Metamask private key
PROJECT_ID=Alchemy API key
```

7. Deploy your smart contract
```shell
cd ..
cd smart-contract
npx hardhat run scripts/deploy.js --network sepolia
```

8. Copy the deplyed contract's address and assign it in client folder's env
9. Run your client
```shell
cd ..
cd smart-contract
npm run dev
```
