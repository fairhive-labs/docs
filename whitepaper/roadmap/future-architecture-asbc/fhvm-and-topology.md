---
description: >-
  Deploying a decentralized network means providing a virtual machine (VM) that
  can be installed on nodes interacting on a peer-to-peer (P2P) basis.
---

# FHVM and topology

The PoLN virtual machine (**polnvm**) will be the key component of this topology.

It will **host and protect the PoLN's blockchain** and **process application specific transactions**.

But some data or services do not necessarily need to be stored or implemented on a decentralized network.

As illustrated below, few “centralized” assets will be implemented and hosted on fairhive-labs’ cloud in order to provide additional secured _off-chain_ services.

<figure><img src="https://miro.medium.com/v2/resize:fit:1400/0*1hQhXIVTXKx_OOb0" alt="" height="254" width="700"><figcaption></figcaption></figure>

Also, for development and testing purposes, **different** **execution** **environments** will be set up thanks to:

* **Kubernetes** clusters, orchestrating containers deployment and availability,
* Multiple **networks** (mainnet and testnet).
