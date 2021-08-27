# Ethereum Marketplace DApp

### Author : Michael Francis

This repository contains an Ethereum Marketplace DApp. It is a basic code for POC of my project.  Users can list items for sale and other users can buy them with Ether.  The smart contracts were developed in [Solidity](https://solidity.readthedocs.io/en/v0.4.24/) using the [Truffle](https://github.com/trufflesuite/truffle) framework.  The user interface was developed using [React](https://reactjs.org/)

## Steps to Install and Run:
*(Assuming you've already installed Node.js, ganache-cli and Truffle and enabled MetaMask extension in your browser.)*

Clone this repository:
```
git clone https://github.com/Mike-64/Farm2Home.git
```
Change directory to ```marketplace``` folder and install all requisite npm packages (as listed in ```package.json```):
```
cd marketplace
npm install
```
Compile smart contracts:
```
truffle compile
```
This creates the contract artifacts in folder ```abis```.

The ```contracts``` folder must be linked to appear under ```src```.

In separate terminal/shell, launch Ganache:
```
ganache-cli
```
Copy the mnemonic phrase from the Ganache console. Use it to import this account using seed phrase into MetaMask in your browser.  Before importing select network ```Localhost 7545``` in MetaMask.

Migrate contracts to ganache:
```
truffle migrate
```

To execute smart contract tests:
```
truffle test
```

Launch application in development mode on http://localhost:3000:
```
npm start
```
## Before Launching Application

Make sure to have the metamask enabled and logged into a metamask wallet else the application returns a blank page.

