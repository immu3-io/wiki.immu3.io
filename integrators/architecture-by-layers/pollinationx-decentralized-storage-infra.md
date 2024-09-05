---
description: >-
  While the OCC SDK integrators can utilize custom storage options, the
  PollinationX decentralized storage infra is set as a default.
---

# PollinationX Decentralized Storage Infra

### Let's Start

Because there was no available out-of-the-box solution, PollinationX (i.e. PX) was developed by a separate team within the CR Systems. PX also acts as a stand-alone solution, otherwise powering various integrator email, messaging and data file transfer use cases.&#x20;

### Features

* Self-custodial storage
* Communication data is accessible only to the private key owner
* Integrator [APIs](https://wiki.pollinationx.io/developer-section/api-reference) and [SDK](https://wiki.pollinationx.io/developer-section/pollinationx-sdk) tooling
* IPFS, BTFS, and FileCoin (phases 1 & 2) support
* [Multi-chain](https://wiki.pollinationx.io/overview/supported-networks-and-storages) availability
* Based on EVM, TypeScript and Solidity frameworks&#x20;
* Monetization via data package dynamic [PX NFTs](https://wiki.pollinationx.io/overview/px-storage-nft) and PX Bandwidth

### Usage with the OCC SDK

For detailed usage instructions of this package, please refer to the [wiki](https://wiki.4thtech.io/docs/sdk/storage).

However, a brief overview is provided below:

```
import { PollinationX } from '@4thtech-sdk/storage';
```

After importing, you can use the package as required by your project.

### Resources

{% embed url="https://wiki.pollinationx.io/" %}

{% embed url="https://github.com/4thtech/sdk-js/tree/main/packages/storage" %}

{% embed url="https://github.com/pollinationx/" %}

{% embed url="https://www.npmjs.com/package/@pollinationx/core" %}
