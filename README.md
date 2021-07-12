<p align="center">
<img src="https://github.com/CrypticMuze/Foodies_Website/blob/master/images/logo.png" alt="FoodiesLogo" height=250px width=250px/>
</p>

# Foodies Website
## About the Project

  This is a responsive website made using HTML. CSS, and Bootstrap 5 for a restarant

## Live Demonstartion of the Project

  LIVE Demonstration: https://youtu.be/fShgkQZcTa0

## Installation

1. Clone repo on your local system

```bash
git clone https://github.com/MishraLokesh/Health_Hub.git
```
2. Open a terminal on your localhost and install the dependencies

```bash
npm install
```
3. Create a Metamask account (if you do not already possess one) and use the Rinkeby Faucet (Our project is deployed on the Rinkeby Test Network) to obtain some test ETH in your metamask wallet.

```
https://faucet.rinkeby.io/ 
```
4. Add your personal 12-word mnemonic and Infura API

```
Goto Health_Hub/ethereum/deploy.js
```
```bash
#In the deploy.js file (lines 11-18) make the following changes to the file -->
let provider = new HDWalletProvider({
  mnemonic: {
  phrase: '#Enter 12 Word mnemonic here',
  },
  #// providerOrUrl: `https://rinkeby.infura.io/v3/${process.env.infura_API}`,
  providerOrUrl: '#Use the format of the Infura API token above and add your own',
  chainId: '4'
  });
```
5. Update your Metamask Wallet account address 

```
Goto Health_Hub/ethereum/factory.js
```
```bash
#In the factory.js file (lines 5 -8) make the following changes to the file -->
const instance = new web3.eth.Contract(
  JSON.parse(JSON.stringify(Factory.abi)),
  '#Enter your Metamask wallet account address here'
);
```
6. Open a terminal on your localhost and deploy the development live server

```bash
npm run dev
```
You're good to go! HealthHub should open on the live server.

## Want to Contribute?
To contribute to this project:
1. Fork this repo
2. Make desired changes after cloning it on your local system.
3. Generate a pull request.

Note: Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change. Please make sure to update tests as appropriate.

## Connect with the Collaborators
1. Lokesh Mishra - [LinkedIN](https://www.linkedin.com/in/lokesh-mishra-0807/) || [GitHub](https://github.com/MishraLokesh) || [Instagram](https://www.instagram.com/lokesh.mishra__/)

2. Aman Anand - [LinkedIN](https://www.linkedin.com/in/amanxanand/) || [GitHub](https://github.com/aman-anand1906) || [Instagram](https://www.instagram.com/aman_anand_619/")

## License
Distributed under the [MIT](https://choosealicense.com/licenses/mit/) license.
