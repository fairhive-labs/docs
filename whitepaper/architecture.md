---
description: >-
  PoLN's architecture employs smart contracts on Ethereum-compatible networks,
  ensuring decentralized operation, wide interoperability, and potent business
  dynamics.
---

# ⏳ (PEND) Architecture Overview

{% hint style="warning" %}
**Disclaimer Regarding Architecture Diagrams**

Please be advised that the architecture diagrams presented in this document may no longer represent the current structure or design of the PoLN protocol.

Over time, as the protocol has evolved, certain details and elements within these diagrams might have been updated or changed.

Therefore, they might contain outdated or erroneous information.

We recommend cross-referencing with the most recent official documentation or contacting the PoLN team directly for the latest and most accurate architectural insights.
{% endhint %}

***

It ‘s an **amazing solution** if you want to **decentralize backend services**.

There are also **many Ethereum compatible projects** providing, today, the **capability** **to** **work** **with** different **Ethereum blockchains**, supporting a kind of interoperability with new protocols and new projects.

**On-chain** backend services (_smart contracts_) will be developed using **solidity**, deployed on testnet and then on mainnet.

**Off-chain** services (_secured rest api_) will be developed using **golang**, tested and deployed on **Docker/Kubernetes** cloud clusters.

They will also access the smart contract services.

**Frontend** will leverage [**metamask**](https://metamask.io/download/) and coinbase wallet plugins into an **Angular** application (_webapp_) using [**ethers.js**](https://docs.ethers.io/) open library.

<figure><img src="https://miro.medium.com/v2/resize:fit:1400/1*370PTuGSwp8JzjygYRsXdw.jpeg" alt="" height="332" width="700"><figcaption><p>PoLN’s web3 design</p></figcaption></figure>

**All code sources will be open** and hosted on fairhive-lab’s G**ithub.**

Frontend and Rest-API images will be built and deployed thanks to devops features of G**ithub** and **CircleCI.**

Rest-API services will be deployed **on Heroku** and **AWS.**