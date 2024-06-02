https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/165084d2-f40c-4bd2-bb54-fcaae466540f

# CrowdFunding dApp

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
![cf-ss-1](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/0db3daea-4ac2-469d-add6-396d91dbf210)
![cf-ss-2](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/d0d585bc-2327-4f4c-8c35-d6eecd512968)
![cf-ss-3](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/3d9aff93-3f39-44fe-8a6e-feb1dd1800d9)
![cf-ss-4](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/aa2272c6-5a91-46b0-aebd-c0fdd6b7e224)
![cf-ss-5](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/fbe3626d-9c1a-467d-ba03-5779acfc0762)
![cf-ss-6](https://github.com/ahmedsemih/CrowdFunding-dApp/assets/102798814/b99f46d8-a93c-4c07-8ae4-00474b6024bf)

## :triangular_flag_on_post: Getting Started

1. First of all you need to clone the repository
```shell
git clone https://github.com/boradesanket13/Nirman.git
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
ACCOUNT_PRIVATE_KEY - Metamask private key
PROJECT_ID - Alchemy API key
```

7. Deploy your smart contract
```shell
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
