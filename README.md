# Decentralised-petshop
(Mainly done for blockbash hackathon)

## Description
Decentralised Petshop is a blockchain-based pet adoption platform built on the Ethereum blockchain using smart contracts. The project allows users to adopt pets and manage pet ownership in a decentralized, secure, and transparent way. The use of blockchain ensures that ownership records are tamper-proof and that transactions are secure.

The petshop leverages Ethereum for smart contract development and integrates web technologies like HTML, CSS, JavaScript, and Web3.js for the front-end interface, making the platform user-friendly and accessible for anyone with an Ethereum wallet.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Smart Contracts](#smart-contracts)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features
- **Decentralized Ownership**: Pets are available for adoption on the blockchain, and ownership records are secured with smart contracts.
- **Pet Adoption**: Users can adopt pets by making a transaction on the Ethereum network.
- **Blockchain Transparency**: All pet adoptions and ownership transfers are recorded on the blockchain for transparency and immutability.
- **Smart Contracts**: The system uses Solidity smart contracts to manage pet adoption processes, ensuring that the process is automated and tamper-proof.

## Installation
Follow these steps to set up and run the Decentralised Petshop on your local machine.

### Prerequisites
- [Node.js](https://nodejs.org/) (for the front-end and Web3 integration)
- [Truffle Suite](https://www.trufflesuite.com/truffle) (for compiling, deploying, and testing smart contracts)
- [Ganache](https://www.trufflesuite.com/ganache) (for running a personal Ethereum blockchain)
- [MetaMask](https://metamask.io/) (browser extension to interact with the Ethereum blockchain)

### Steps to Install

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/gingerjabami/Decentralised-petshop.git
   cd Decentralised-petshop
   ```

2. **Install Dependencies**:
   Install Node.js packages:
   ```bash
   npm install
   ```

3. **Set Up Truffle**:
   - Install Truffle globally if you haven't already:
     ```bash
     npm install -g truffle
     ```
   - Compile and deploy the smart contracts:
     ```bash
     truffle compile
     truffle migrate --network development
     ```

4. **Set Up Ganache**:
   - Open Ganache and create a new workspace to simulate an Ethereum blockchain.
   - Make sure the network settings in Truffle (truffle-config.js) are set to match Ganache’s default configuration.

5. **Run the Front-End**:
   Start the front-end application by running:
   ```bash
   npm start
   ```
   The app should be accessible on `http://localhost:3000` in your browser.

## Usage
Once the application is running, you can use the Decentralised Petshop platform to adopt pets and view adoption history:

1. **Connect MetaMask**: Make sure you have MetaMask installed and connected to Ganache or any Ethereum test network.
2. **Adopt a Pet**: Use the platform’s UI to adopt a pet. This will trigger a blockchain transaction to record the adoption in the smart contract.
3. **View Pet Ownership**: The platform will display the adoption records stored on the blockchain for transparency.

## Smart Contracts
The core functionality of the Decentralised Petshop is powered by the following smart contracts:

- **Petshop.sol**: This smart contract handles pet adoption, ownership transfer, and querying adoption details.
  
### Example Contract Functions:
- `adoptPet(address _owner, uint256 _petId)`: Allows users to adopt a pet.
- `getOwner(uint256 _petId)`: Returns the current owner of a pet.
- `getAdoptionHistory(uint256 _petId)`: Retrieves the full adoption history of a pet.

You can find the smart contracts in the `contracts/` folder.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For any questions or feedback, feel free to reach out to me at [gingerjabami@gmail.com](mailto:gingerjabami@gmail.com).

You can also open an issue on GitHub if you encounter problems or have suggestions.

```

