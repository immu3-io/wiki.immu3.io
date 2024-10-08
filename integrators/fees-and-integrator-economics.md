---
description: >-
  Total user cost equals the sum of the L1/L2 transaction gas, the protocol fee
  and the storage cost.
---

# Fees & Integrator Economics

### Let's Start

Web3 mainly works based on the PAYGO (i.e. pay-as-you-go) transaction model, meaning the user has to pay for every mail, message, or data-sharing transaction. To make on-chain communication more viable, work is being done that will parallel to PAYGO also enable subscription-based models, so the users can pay a monthly subscription fee to access block space and communicate without the hurdle of paying for every transaction.

## Fees within the Protocol

Parallel to the underlying L1/L2 transaction gas cost, the service fees (i.e. protocol fees) are also settled on the smart contract level and are applicable for every mail, message or data file-sharing transaction. Total user cost equals the sum of the L1/L2 transaction gas and service fees and the cost of decentralized storage. Both, the gas and service fees converge and manifest as one end-user communication transaction fee. Fees are handled by the \[[AppFeeManager](architecture-by-layers/occ-protocol-v.1.md#appfeemanager-smart-contract)] smart contract.&#x20;

### Fee Table

{% tabs %}
{% tab title="Blockchain Fees" %}
<table><thead><tr><th width="278.66666666666663">Smart Contract Methods</th><th>Gas Limit</th><th>*Estimated Price in FTM</th><th>*Estimated Price in ROSE</th></tr></thead><tbody><tr><td><code>[Users]</code> Register Encryptor</td><td>145000</td><td>≈ 0.0059 FTM</td><td>≈ 0.014 ROSE</td></tr><tr><td><code>[Mail]</code> Send Mail</td><td>610000</td><td>≈ 0.025 FTM</td><td>≈ 0.061 ROSE</td></tr><tr><td><code>[Mail]</code> Send Data file Package</td><td>610000</td><td>≈ 0.025 FTM</td><td>≈ 0.061 ROSE</td></tr><tr><td><code>[Chat]</code> Send Message</td><td>*500000</td><td>≈ 0.02 FTM</td><td>≈ 0.05 ROSE</td></tr><tr><td><code>[Chat]</code> Create Group</td><td>*1025625</td><td>≈ 0.04 FTM</td><td>≈ 0.1 ROSE</td></tr><tr><td><code>[PX]</code> Mint free package or new storage</td><td>3800000</td><td>≈ 0.15 FTM</td><td>≈ 0.38 ROSE</td></tr><tr><td><code>[PX]</code> Mint Bandwidth</td><td>860000</td><td>≈ 0.03 FTM</td><td>≈ 0.086 ROSE</td></tr><tr><td><code>[PX]</code> Upgrade Package</td><td>1240000</td><td>≈ 0.05 FTM</td><td>≈ 0.12 ROSE</td></tr></tbody></table>
{% endtab %}

{% tab title="Service Fees" %}
| dApp              | Smart Contract | Base Fee                 | dApp Fee                 | Total                          | Bandwidth                |
| ----------------- | -------------- | ------------------------ | ------------------------ | ------------------------------ | ------------------------ |
| BlockCommunicator | `[Mail]`       | TBD                      | TBD                      | /                              | /                        |
| BlockCommunicator | `[Chat]`       | TBD                      | TBD                      | /                              | /                        |
| W3XShare App      | `[Mail]`       | \~0.0075$ FTM, ROSE... ≡ | \~0.0925$ FTM, ROSE... ≡ | \~**0.1$** ETH, FTM, ROSE... ≡ | 2                        |
| 4P Super App      | `[Mail]`       | \~0.0075$ FTM, ROSE ≡    | \~0.0025$ FTM, ROSE ≡    | \~**0.01$** FTM, ROSE ≡        | 1 (json) + X attachments |
| 4P Super App      | `[Chat]`       | \~0.0025$ FTM, ROSE ≡    | \~0.0025$ FTM, ROSE ≡    | \~**0.005$** FTM, ROSE ≡       | /                        |
{% endtab %}

{% tab title="PX sNFT Price" %}
<table><thead><tr><th>Size</th><th>Bandwidth Limit</th><th width="182">Estimated price in $</th><th>Estimated Price in FTM</th><th>Estimated Price in ROSE</th></tr></thead><tbody><tr><td><code>100MB</code></td><td>25 uploads</td><td>Free</td><td>Free</td><td>Free</td></tr><tr><td><code>1GB</code></td><td>50 uploads</td><td>≈ 5$</td><td>≈ 12 FTM</td><td>≈ 80 ROSE</td></tr><tr><td><code>5GB</code></td><td>150 uploads</td><td>≈ 15$</td><td>≈ 35 FTM</td><td>≈ 240 ROSE</td></tr><tr><td><code>20BG</code></td><td>400 uploads</td><td>≈ 30$</td><td>≈ 70 FTM</td><td>≈ 470 ROSE</td></tr></tbody></table>
{% endtab %}

{% tab title="PX Bandwidth Price" %}
| Bandwidth  | Estimated price in $ | Estimated Price in FTM | Estimated Price in ROSE |
| ---------- | -------------------- | ---------------------- | ----------------------- |
| 10 uploads | ≈ 1$                 | ≈ 3 FTM                | ≈ 16 ROSE               |
{% endtab %}

{% tab title="Resources" %}
<table><thead><tr><th width="163.66666666666663">Function</th><th width="196">GAS Tracker</th><th width="207">Unit Converter</th><th>Token</th></tr></thead><tbody><tr><td>Fantom</td><td><a href="https://ftmscan.com/gastracker">Fantom GasTracker</a></td><td><a href="https://ftmscan.com/unitconverter">Fantom UnitConverter</a></td><td>FTM</td></tr><tr><td>Oasis Sapphire</td><td>/</td><td>/</td><td>ROSE</td></tr></tbody></table>
{% endtab %}
{% endtabs %}

{% hint style="info" %}
**\*Note:** Crypto prices are estimated and calculated based on; (1) Fantom 41 GWei, and; (2) Oasis 100 GWei gas price. The "Send message" gas limit is based on the length of the message. The "Create Group" gas limit depends on the number of members in the group and the encryption variable. Table calculation is based on a two-member encrypted group. References to USD prices are made for approximate fiat value illustration purposes only.
{% endhint %}

### User cost calculation estimate per message transaction

Let's assume that:&#x20;

> Blockchain fees = \~0.009$ FTM ≡
>
> Service base-fee = \~0.0025$ FTM ≡
>
> Service dApp-owner-fee  = \~0.0025$ FTM... ≡
>
> **Total user cost = \~0.014$ FTM... ≡**

## Integrator Economics

OCC Protocol v.1 build-in monetization layers enable independent integrator economics, permitting developers to focus on application UI/UX features. `Level-1` integrators can set the desired protocol base fees, while `Level-2` integrators can set and manage their protocol dApp-owner fees.

### Monetization Schematic

<figure><img src="../.gitbook/assets/IMMU3-FEES-24.png" alt=""><figcaption></figcaption></figure>
