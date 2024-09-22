<h1 align="center" style="font-weight: bold;">Fund Seed 💻


[![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/navendu-pottekkat/awesome-readme?include_prereleases)](https://img.shields.io/github/v/release/navendu-pottekkat/awesome-readme?include_prereleases)
[![GitHub last commit](https://img.shields.io/github/last-commit/navendu-pottekkat/awesome-readme)](https://img.shields.io/github/last-commit/navendu-pottekkat/awesome-readme)
[![GitHub issues](https://img.shields.io/github/issues-raw/navendu-pottekkat/awesome-readme)](https://img.shields.io/github/issues-raw/navendu-pottekkat/awesome-readme)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/navendu-pottekkat/awesome-readme)](https://img.shields.io/github/issues-pr/navendu-pottekkat/awesome-readme)
[![GitHub](https://img.shields.io/github/license/navendu-pottekkat/awesome-readme)](https://img.shields.io/github/license/navendu-pottekkat/awesome-readme)
</h1>

<p align="center">This is a decentralized crowdfunding application with NextJS and Solidity. In this dapp peoples can create campaigns or donate to them.
</p>

<br>
<h2 id="Video">💻 Video</h2>

https://github.com/boradesanket13/FundSeed/assets/79108273/9c5be52c-a316-496c-984a-15c6e25e2100

<br>

<p align="center">
 <a href="#Video">Video</a>
<a href="#Features">Features</a>
<a href="#technologies">Technologies</a>
<a href="#Screenshots">Screenshots</a>
<a href="#started">Getting Started</a>
<a href="#colab">Collaborators</a>
<a href="#contribute">Contribute</a> 
</p>



<h2 id="Features">💻 Features</h2>

- Dark Theme
- Responsive UI
- Wallet Authentication
- Create Campaign
- Donate or Withdraw Ethereum
- Decentralized

<h2 id="Project Details">💻 Project Details</h2>

- Developed an ```Ethereum Blockchain```-based Decentralized Finance (```DeFi```) application focused on fundraising for startups, allowing users to create and donate to crowdfunding campaigns using ```Ether```.
- Designed and implemented smart contracts using ```Solidity``` to securely handle campaign creation, donations, and withdrawals on the blockchain.
- Integrated ```Metamask``` for wallet authentication, providing a seamless login experience for users.
- Built a responsive and dynamic user interface with ```Next.js```, and ```TailwindCSS```, ensuring smooth navigation across all devices.
- Leveraged ```Hardhat``` as the Ethereum development environment and ```Waffle``` for smart contract testing.
- Used ```Ethers.js``` for interacting with smart contracts and handling Ethereum-based transactions.
- Implemented features like campaign creation, Ethereum donation processing, and withdrawal functionality, ensuring a decentralized and secure environment.
- Additionally, provided a dark theme for enhanced user experience and implemented wallet authentication for secure access.

<h2 id="technologies">💻 Technologies</h2>

- [Solidity](https://soliditylang.org/) - Smart Contract Language
- [React](https://reactjs.org/) - JavaScript library for UI
- [NextJS](https://nextjs.org/) - React Framework
- [TailwindCSS](https://tailwindcss.com/) - CSS Framework
- [Hardhat](https://hardhat.org/) Ethereum Development Environment
- [Waffle](https://ethereum-waffle.readthedocs.io/en/latest/) Smart Contract Test Library
- [Ethers](https://docs.ethers.org/v5/) Smart Contract Interaction Library
- [React Icons](https://react-icons.github.io/react-icons/) - Icon Library

 
<h2 id="Screenshots">💻 Screenshots</h2>

 
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





<h2 id="started">🚀 Getting started</h2>
[(Back to top)](#table-of-contents)

Here you describe how to run your project locally
 
<h3>Prerequisites</h3>

Here you list all prerequisites necessary for running your project. For example:

- [NodeJS](https://nodejs.org/en/download/package-manager)
- [Git](https://www.git-scm.com/download/win)
 
<h3>Cloning</h3>

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
cd client
npm run dev
```





 
<h2 id="colab">🤝 Collaborators</h2>

<p>Special thank you for all people that contributed for this project.</p>
<table>
<tr>


<td align="center">
<a href="https://github.com/boradesanket13">
<img src="https://avatars.githubusercontent.com/u/79108273?v=4" width="100px;" alt="Sanket Borade Profile Picture"/><br>
<sub>
<b>Sanket Borade</b>
</sub>
</a>
</td>

</tr>
</table>
 
<h2 id="contribute">📫 Contribute</h2>
 ## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
 ## License

Distributed under the MIT License. See [MIT License](https://opensource.org/licenses/MIT) for more information.
