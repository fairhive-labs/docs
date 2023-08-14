---
description: >-
  This is not the purpose of this document to explain what DevOps is but it’s
  important to share information regarding the FHVM delivery.
---

# DevOps CI/CD

Basically, _DevOps_ is a practice combining software development (_Dev_) and IT Operations (_Ops_) and this proven practice is at the present time widely adopted by modern organizations.

_DevOps_ usually includes the concept of _CI/CD_ (_Continuous Integration / Continuous Delivery_).

_CI/CD_ is used by software developers for build, testing and deployment automation.

<figure><img src="https://miro.medium.com/v2/resize:fit:1400/0*TG0oLqE-a27hlfii" alt="" height="361" width="700"><figcaption><p><em>Image source:</em> <a href="https://devopedia.org/devop"><em>https://devopedia.org/devop</em></a></p></figcaption></figure>

Automatic deployment is not really relevant assuming a decentralized network.

But continuous delivery is a good fit for the community, especially for the **network** **validators** who are willing to quickly **upgrade their nodes**, deploy the **most recent version** of the VM and **preserve** the **availability**/**consistency** of the network.

<figure><img src="https://miro.medium.com/v2/resize:fit:1400/0*l-8B7O09XAe_sjl-" alt="" height="331" width="700"><figcaption></figcaption></figure>

This is possible thanks to modern “container” technologies like _Docker_ which provide the capability to **create, share and run a common public image of the **_**FHVM**_ on different supported systems and environments (Kubernetes clusters, VPS clouds, on-premise servers, student laptops, etc).

The **docker images** are **automatically built** from the **public repositories** every time a change is made and detected on the source code using a set of pre-defined compiling and testing instructions (_CI/CD pipeline_).

They are also versioned and protected in the **public image library **_**Docker Hub**_.

Finally, in order to automatically deploy the most recent versions of the _FHVM_, continuous delivery will be performed at fairhive-labs.
