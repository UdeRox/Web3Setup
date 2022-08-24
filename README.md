# Web3Setup
Setup initial setup with web3 and solidity contract 

Compile the Project
npx hardhat compile

# Run local hardhat node
npx hardhat node

# Deploying contracts to local hardhat network for testing
npx hardhat run --network localhost scripts/deploy.js

# Intracting with contracts
npx hardhat console --network localhost
const Box = await ethers.getContractFactory('Box');
const box = await Box.attach('0x5FbDB2315678afecb367f032d93F642f64180aa3')

# Querying the state of a transaction
await box.retrieve()
# Sending a transaction
await box.store(42)

# Interaction with contract Programmetcially
npx hardhat run --network localhost ./scripts/index.js
# Run local test, 
npx hardhat test
# Use circleci for the CICD

#Test deployment
