# CHANGELOG

## Smartdex Contracts v1

- Clone the 0x-monorepo and install node dependencies
```
 $ git clone https://github.com/0xProject/0x-monorepo.git
 $ cd 0x-monorepo/
 $ yarn install
```
- Build migrations package and all other monorepo packages that it depends on, run the following from the monorepo root directory
- Deploy the contracts to Matic mainnet
- Open packages/contract-addresses/src/index.ts, append Matic to network id list and put the deployed address in the corresponding fields
- Build contract-addresses package and all other monorepo packages that it depends on