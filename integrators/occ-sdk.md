---
description: >-
  Empowers integrators to seamlessly interact with protocol smart contracts,
  storage providers, encryption methods, and the Encryptor extension.
---

# OCC SDK

### OCC SDK

As a part of the immu3's infrastructure integrator stack, the OCC SDK provides abstractions to assist you with interacting with the OCC Protocol v.1 smart contracts in a Typescript/Javascript environment. The OCC SDK also simplifies the encryption process and remote storage access.

To begin, we recommend looking at wiki [Guides](https://wiki.4thtech.io/docs/integration/sdk) and GitHub [Repos](https://github.com/4thtech/sdk-js) which include runnable examples and walkthroughs of core usages. These guides will help you better understand how to use and integrate the OCC SDK into your application.

### Features

* Modular Packages: Typescript/Javascript stack including Encryption, Encryptor, Ethereum, Storage, Types, and Utils
* EVM Multi-chain Support: Ready-to-use compatibility with multiple Ethereum Virtual Machine (EVM) chains
* Method Usability Tests: Comprehensive tests to ensure functionality and usability
* Integrator Monetization: App owner-fee smart contract feature

### Packages

* Encryption: Allows for easy data encryption and decryption using various encryption methods
* Encryptor: Manages connection with the Encryptor extension
* Ethereum: Handles Ethereum blockchain transactions, smart contracts, and other blockchain-related functions
* Storage: Optimise storing and retrieving procedures, enhancing data management
* Types: Contains the type declarations used across all the other packages
* Utils: Provides utility functions and helpers that facilitate and enhance the functionality of the SDK

### Start Building

Each package comes with its unique usage instructions. To understand how to use a package, refer to the respective package directories for more detailed instructions and documentation. Typically, you would import a package as follows:

```
import { Mail } from '@4thtech-sdk/ethereum';
```

Use the imported package as required by your project. Please access GitHub for the latest guidelines.

{% hint style="success" %}
**Tip:** Experience seamless integration. Utilize method functions tests ([test example](https://github.com/4thtech/sdk-js/blob/main/packages/ethereum/src/lib/\_\_tests\_\_/chat.spec.ts)).
{% endhint %}

### Resources

{% embed url="https://github.com/4thtech/sdk-js" %}
