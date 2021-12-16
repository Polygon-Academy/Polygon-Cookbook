# Installation

You'll need to download:

****[**Node**](https://nodejs.dev/learn/how-to-install-nodejs)

****[**Git**](https://git-scm.com/downloads)****

**Yarn**

It is recommended to install Yarn through the [npm package manager](http://npmjs.org), which comes bundled with [Node.js](https://nodejs.org) when you install it on your system.

Once you have npm installed you can run the following both to **install** and **upgrade** Yarn:

```
npm install --global yarn
```

**Web3.js**

This can be done using the following methods:

* npm: `npm install web3`
* yarn: `yarn add web3`
* pure js: link the `dist/web3.min.js`

After that you need to create a web3 instance and set a provider.

Most Ethereum-supported browsers like MetaMask have an [EIP-1193](https://eips.ethereum.org/EIPS/eip-1193) compliant provider available at `window.ethereum`.

For web3.js, check `Web3.givenProvider`.

If this property is `null` you should connect to a remote/local node.

```
// In Node.js use: const Web3 = require('web3');

const web3 = new Web3(Web3.givenProvider || "ws://localhost:8545");
```

**React**

[Create React App](https://github.com/facebookincubator/create-react-app) is a comfortable environment for **learning React**, and is the best way to start building **a new** [**single-page**](https://reactjs.org/docs/glossary.html#single-page-application) **application** in React.

It sets up your development environment so that you can use the latest JavaScript features, provides a nice developer experience, and optimizes your app for production. You’ll need to have [Node >= 14.0.0 and npm >= 5.6](https://nodejs.org/en/) on your machine. To create a project, run:

```
npx create-react-app my-app
cd my-app
npm start
```

****[**Truffle / Ganache**](http://trufflesuite.com/docs/truffle/getting-started/installation)****

```
npm install -g truffle
```



