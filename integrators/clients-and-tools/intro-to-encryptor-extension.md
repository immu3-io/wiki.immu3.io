---
description: >-
  Fully self-custodial Chrome extension that enables E2E AES-256-GCM highly
  secure encryption of on-chain communications by user-owned private keys.
cover: ../../.gitbook/assets/Encryptor-Mockup.jpg
coverY: 108
---

# Intro to Encryptor extension

### True Self-custodial communication encryption

Used by Immu3 stack-enabled end-users, the Encryptor extension adds a communication encryption layer currently unsupported by major Web3 wallets. It enables the ECDH key agreement protocol, creating an elliptic curve key pair and computing the shared secret key between the sender and receiver. Similar to a Web3 wallet, it allows users to save their private key seed phrases, which can be used to restore their Encryptor at any time or on any device.

{% hint style="success" %}
**Note:** Encryptor is an open-source, self-custodial Chrome extension built with Vite, Vue, and Manifest v3. It enables end-to-end AES-256-GCM encryption of on-chain communications using user-owned private keys, providing advanced and highly secure encryption.
{% endhint %}

### How to install it?

{% embed url="https://youtu.be/TjMTM35-o4M" %}

### Google Chrome Install

{% embed url="https://chrome.google.com/webstore/detail/encryptor/feolajpinjjfikmmeknkdjbllbppojij?authuser=3&hl=en-GB" %}

### Direct Install

1. Check if your `Node.js` version is >= **14**.
2. Change or configure the name of your extension on `src/manifest`.
3. Run `npm install` to install the dependencies.

### Developing

run the command

```
$ cd encryptor-extension

$ npm run dev
```

#### Chrome Extension Developer Mode

1. set your Chrome browser 'Developer mode' up
2. click 'Load unpacked', and select `extension/build` folder

#### Normal FrontEnd Developer Mode

1. access `http://localhost:3000/`
2. when debugging the popup page, open `/popup.html`
3. when debugging the options page, open `/options.html`

### Packing

After the development of your extension run the command

```
$ npm build
```

Now, the content of `build` folder will be the extension ready to be submitted to the Chrome Web Store. Just take a look at the [official guide](https://developer.chrome.com/webstore/publish) for more info about publishing.

### Resources

{% embed url="https://github.com/4thtech/encryptor-extension" %}

{% embed url="https://github.com/4thtech/encryptor-extension/releases" %}
