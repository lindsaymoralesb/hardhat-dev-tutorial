# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a Hardhat Ignition module that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat ignition deploy ./ignition/modules/Lock.js
```
# Hardhat Learning Practice

1. Create an Alchemy account and a a dev wallet.
3. Create a .env file in the root of the project. Include the following variables:

```ALCHEMY_API_KEY```: API Key found on Alchemy account.

```PRIVATE_KEY```: Your dev wallet private key.

```ETHERSCAN_API_KEY```: API Key from etherescan account.

4. Update the ```hardhat.config.js``` file to include the env variables and networks.
5. Compile contract with ```npx hardhat compile```.
6. Deploy contract by running ```npx hardhat ignition deploy ./ignition/modules/Lock.js```. To choose a specific network use ```--network <network-name>```.
7. Verify contract with ```npx hardhat ignition deploy ignition/modules/Lock.js --network optimismSepolia --verify```