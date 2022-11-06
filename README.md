# Blockchain-Enabled Access Control (BEACON)

Create a .env file in the top-level directory with these environment variables

```
API_URL = "<goerli API URL>"
MUMBAI_API_URL = "<Polygon Mumbai API URL>"
WALLET_ADDRESS_1 = "<Metamask wallet address>"
PRIVATE_KEY_1 = "<Private key for WALLET_ADDRESS_1>"
WALLET_ADDRESS_2 = "<Metamask wallet address>"
PRIVATE_KEY_2 = "Private key for WALLET_ADDRESS_2"
EVTOKEN_CONTRACT_ADDRESS = "<Address to deployed EVToken.sol>"
SUBJECT_ATTRIBUTE_CONTRACT_ADDRESS = "<Address to deployed SubjectAttribute.sol>"
POLICY_MANAGEMENT_CONTRACT_ADDRESS = "<Address to deployed PolicyManagement.sol>"
OBJECT_ATTRIBUTE_CONTRACT_ADDRESS = "<Address to deployed ObjectAttribute.sol>"
ACCESS_CONTROL_CONTRACT_ADDRESS = "<Address to deployed AccessControl.sol>"
```

compile smart contracts:
```
$ npx hardhat compile
```

deploy smart contracts:
```
$ npx hardhat run scripts/deploy.js --network <network name defined in hardhat.config.js>
```

contracts addresses deployed on Arbitrum Nitro Testnet:

```
(base) ➜  soulbound-beacon git:(main) ✗ npx hardhat run scripts/deploy.js --network goerli
SoulboundNFT contract deployed to address: 0x8E33Fb04CA3ac99caD20d5c2B9f7f6B843f84C88
SubjectAttribute contract deployed to address: 0x8F102a4C779f3475eB3D0b86F08214E5CCeFf3AE
PolicyManagement contract deployed to address: 0xc00144d9dfcb6328B9C35fc16efF1F0935c6cbfA
ObjectAttribute contract deployed to address: 0x01b71373A7513228b145e6a15354797597638022
AccessControl contract deployed to address: 0xF53B79b11bB73D96A9e9B54b32eA46aaB5129397
```
