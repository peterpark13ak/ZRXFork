This repository is forked from [0x-monorepo](https://github.com/0xProject/0x-monorepo)

## Usage

Node version 6.x or 8.x is required.

Most of the packages require additional typings for external dependencies.
You can include those by prepending the `@0x/typescript-typings` package to your [`typeRoots`](http://www.typescriptlang.org/docs/handbook/tsconfig-json.html) config.

```json
"typeRoots": ["node_modules/@0x/typescript-typings/types", "node_modules/@types"],
```

## Contributing

We strongly recommend that the community help us make improvements and determine the future direction of the protocol. To report bugs within this package, please create an issue in this repository.

#### Read our [contribution guidelines](./CONTRIBUTING.md).

### Install dependencies

Make sure you are using Yarn v1.9.4. To install using brew:

```bash
brew install yarn@1.9.4
```

Then install dependencies

```bash
yarn install
```

You will also need to have Python 3 installed, in order to build and run the tests of `abi-gen`'s command-line interface, which is integrated with the yarn build, yarn test, and yarn lint commands described below. More specifically, your local pip should resolve to the Python 3 version of pip, not a Python 2.x version.

### Build

To build all packages:

```bash
yarn build
```

To build a specific package:

```bash
PKG=@0x/web3-wrapper yarn build
```

To build all contracts packages:

```bash
yarn build:contracts
```

### Watch

To re-build all packages on change:

```bash
yarn watch
```

To watch a specific package and all it's dependent packages:

```bash
PKG=[NPM_PACKAGE_NAME] yarn watch

e.g
PKG=@0x/web3-wrapper yarn watch
```

### Clean

Clean all packages:

```bash
yarn clean
```

Clean a specific package

```bash
PKG=0x.js yarn clean
```

### Rebuild

To re-build (clean & build) all packages:

```bash
yarn rebuild
```

To re-build (clean & build) a specific package & it's deps:

```bash
PKG=0x.js yarn rebuild
```

### Lint

Lint all packages:

```bash
yarn lint
```

Lint a specific package:

```bash
PKG=0x.js yarn lint
```

### Run Tests

Run all tests:

```bash
yarn test
```

Run a specific package's test:

```bash
PKG=@0x/web3-wrapper yarn test
```

Run all contracts packages tests:

```bash
yarn test:contracts
```
### Deployed Contracts on Matic Mainnet

- ERC20Proxy successfully deployed at 0x66dc3b01f674b6c960cf60f3fb78e16342553cab
- ERC721Proxy successfully deployed at 0xb5d157ef45d8bfc9c413d00d0e902fe6a3ddbf8b
- ZRXToken successfully deployed at 0x93719d8478d238c5996806a733e2068e0ead0b0e
- WETH9 successfully deployed at 0x6f3b2e10972cd42219f4108e72e9e15a616e5ba9
- Exchange successfully deployed at 0x08330ac7b7f4a6695f41e3b8419113534cd61df0
- DummyERC20Token successfully deployed at 0xc2c84b533a9518241e73d525afc89c3c57769e9f
- DummyERC20Token successfully deployed at 0x48de9fa861a51ffe9fe0c614348d6e556034803b
- DummyERC20Token successfully deployed at 0x280c9ece1db286bea1c717849e0fc03bc38f7f8d
- DummyERC20Token successfully deployed at 0x20489f8affb46e30931a456fbbb4d92d9b655bf8
- DummyERC20Token successfully deployed at 0x46bf061ff7248cd33f060be98aa2fa57f0b9ce1f
- DummyERC721Token successfully deployed at 0xbc5c7781f1e45c906195833a9a9967a19f175cc3
- ERC1155Proxy successfully deployed at 0xade2af52f3dbe515e4abae89cfad06e6e60ff049
- StaticCallProxy successfully deployed at 0xc3bf2397eac18ff4107f6edf68e62aff1b11990d
- MultiAssetProxy successfully deployed at 0x636168180a78687127ee8479893f0a2f5eb7a640
- Forwarder successfully deployed at 0x995fde61633433fdb6d2c6f7ca885255d526f5c7
- OrderValidator successfully deployed at 0xab979e26f455465b094778b4717918e64d06c2dc
- DutchAuction successfully deployed at 0xb399ee7b4cb4344958bc47652b886c63493e3e42
- AssetProxyOwner successfully deployed at 0x8b8ebd096ed2ba7f415b5c185511eee8be59f814
- CoordinatorRegistry successfully deployed at 0x9928a61ad210ae32e129d94195f27c556d33f963
- Coordinator successfully deployed at 0x8b259a94e4b23816b2751c04dc03f9953ed91034
- DevUtils successfully deployed at 0x35a6d26072d5b25c6dff261c756b0bf142e7c21b