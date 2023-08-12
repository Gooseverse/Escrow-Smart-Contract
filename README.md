# Escrow Smart Contract

This is a simple Escrow smart contract written in Solidity. It allows users to deposit and withdraw ETHscriptions (ETH) and charges a 2% fee on each withdrawal. The collected fees are tracked and can be transferred to a designated wallet address when a certain threshold is reached.

## Getting Started

### Prerequisites

Make sure you have the following software installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### Installation

1. Clone the repository:

git clone https://github.com/Gooseverse/escrow-smart-contract.git
cd escrow-smart-contract


2. Install the required dependencies:

npm install

3. Compile the smart contract:

npx hardhat compile


## Usage

1. Deploy the smart contract to a local Hardhat network:

npx hardhat run scripts/deploy.js --network localhost

2. Interact with the smart contract using the provided scripts in the `scripts` directory.

### Scripts

- `deposit.js`: Deposit ETH into the Escrow contract.
- `withdraw.js`: Withdraw ETH from the Escrow contract.
- `collectFees.js`: Collect accumulated fees from the contract (owner-only).
- `recordFee.js`: Record a fee amount in the contract (owner-only).
- `getBalance.js`: Get the balance of an account in the contract.

## Configuration

Update the `feeReceiver` address in the `deploy.js` script to set the address that will receive the collected fees.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
