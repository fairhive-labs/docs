---
description: >-
  In this stage, fellowships stake tokens, ensuring commitment, while initiators lock fees and contractor payments. These secure methods in smart contracts safeguard interests and foster trust in the PoLN ecosystem.
---

# **Staking & Payment Locks**

<figure><img src="../../.gitbook/assets/_whyvrafvr_cubes_843b0dd3-bafb-4dff-8d3b-ae5788721c60.png" alt="" width="563"><figcaption></figcaption></figure>

In the realm of PoLN's operational dynamics, this phase serves as a foundational checkpoint, ensuring both initiator and fellowship commitment.

By mandating staked assets and locking payments, it infuses the ecosystem with accountability, while safeguarding the interests of all participants.

## **Purpose of Staking**

Staking is not just a formality within the PoLN protocol. It serves a multi-fold purpose:

### **Skin in the Game**

The staking mechanism is designed to ensure that fellowships are genuinely committed to the success of a project. By staking $POLN tokens, they are essentially putting their resources on the line, signaling their confidence in the successful execution of the project.

### **Potential Rewards**

Upon the successful completion of the project, fellowships retrieve their staked amount and earn the protocol fees as their reward. If the project fails, they risk losing their entire staked amount.

### **Deterrence against Malfeasance**

Staking serves as a deterrent against any potential malicious intentions or lackluster commitment from the fellowship. Their direct financial stake in the project's outcome ensures that they remain incentivized for the project's success.

## **Dynamic Staking Amounts**

While there is a minimum staking requirement of 10% of the total project fees set by the initiator, fellowships can choose to stake any amount above this threshold.

By staking higher amounts, fellowships might portray a heightened level of confidence and commitment to the project, potentially influencing the initiator's bid selection process.

## **Initiator's Fee Payment & Contractor Provisioning**

Once a fellowship's bid is accepted and they've staked the requisite $POLN tokens, the onus shifts to the initiator. 

The initiator must promptly address two vital financial commitments: 
* covering the protocol's fees,
* setting aside the contractor's payment.

To ensure transparency, trust, and security within PoLN's ecosystem, both these sums are locked into a smart contract-based escrow system. This escrow acts as a trust-establishing mechanism, confirming to fellowships and contractors that the initiator has genuinely committed the funds. 

Furthermore, the escrow operates based on set project milestones, allowing for incremental releases of funds as progress markers are achieved. 

In cases of disputes or disagreements, this neutral financial holding ground ensures neither party can unilaterally access the funds without due resolution.

By locking in both the fees and the contractor's prospective payment, PoLN not only guarantees the availability of funds for fee distribution at the project's culmination but also solidifies the contractor's trust, knowing their due remuneration is secure.

## **Protection Mechanism & Assurance**

Both the fellowship's staked tokens and the initiator's locked fees, alongside the provisioned contractor payment, are securely stored in smart contracts on the blockchain.

This structure serves multiple purposes:

* The contractor is assured of payment upon successful delivery, fostering trust and motivation.
* The fellowship can retrieve their staked tokens upon the project's success, ensuring their financial security.
* The initiator's commitment to the project is visibly represented by the locked-in funds, emphasizing the seriousness and genuine intent behind the project.

## **Release of Payments & Stakes**

### **Distribution of Locked Fees**

Upon successful completion of the project and validation from the initiator, the locked protocol fees are distributed amongst all members of the fellowship based on previously agreed-upon ratios.

### **Return of Fellowship's Stake**

Alongside the release of the protocol fees, the fellowship's staked $POLN tokens are unlocked and returned to them, signifying the successful execution and delivery of the project.

### **Payment to the Contractor**

The agreed payment for the contractor's services is released as per the predefined invoicing schedule or milestones.

This ensures that all parties are fairly compensated for their roles and contributions upon project completion.

## **Project Failure Scenarios**

When a project does not achieve its desired objectives or fails, the following mechanisms will come into play:

### **Distribution of Protocol Fees**

If the project is deemed a failure, the entire protocol fees paid by the initiator will be distributed among the broader community rather than the fellowship.

### **Loss of Fellowship's Stake**

In the event of a project's failure, the fellowship's staked $POLN tokens are burnt, representing a direct financial loss to the fellowship.

### **Initiator’s Reward**

The initiator does not receive their reward in the case of project failure.

These measures aim to maintain the integrity of the system, hold fellowships accountable, and ensure they remain genuinely committed to the projects they decide to undertake.

## **Dispute Resolution**

In the initial stages of the PoLN protocol, disputes between the initiator and the fellowship will be handled based on a predefined set of guidelines and criteria.

These criteria will serve as a framework to determine the release or forfeiture of locked funds. They could include, but are not limited to:

* [ ] **Project Delivery Assessment:** This will focus on whether the project was delivered as per the outlined specifications and requirements.
* [ ] **Timelines:** If the project was delivered within the agreed-upon time or if there were delays, and the reason for such delays.
* [ ] **Quality of Work:** An evaluation of the work's quality compared to industry standards or previous work from the contractor.
* [ ] **Communication:** Regularity, clarity, and promptness of communication between parties during the project's duration.
* [ ] **Feedback Loops:** The efficiency in addressing feedback or changes requested by the initiator during the course of the project.

In the future, as the PoLN ecosystem matures, there is an aspiration to integrate a decentralized arbitration system.

This would involve community members or designated arbitrators who, in case of disagreements, would weigh in based on evidence presented by both parties. This system would not only bolster the trust within the community but also ensure more fairness and decentralization in the resolution process.

## **Timely Provisions by Initiator**

Post bid acceptance, the initiator has a grace period (e.g., 1 week) to provision the contractor's payment and pay the required PoLN fees.

Should the initiator fail to meet these obligations within the set timeframe:

* The project is marked as "Aborted".
* Fellowships are notified that the project has not commenced due to payment failures.
* The stipulations surrounding such scenarios should be explicitly outlined in the contract between the fellowship and the initiator.
* Upon the project's status being marked as "Aborted," the fellowship can retrieve its staked amount without any penalties. The project then reverts to its original state, and if no action is taken, it will eventually be discarded after the specified deadline.

## **Fellowship's Staking Commitment**

If a fellowship, after winning the bid, fails to stake the agreed-upon amount within the specified period:

* The initiator is alerted and has the discretion to choose an alternative fellowship or await the initial fellowship's compliance.
* The initial project bid by the fellowship is considered void or cancelled.
* Here too, the conditions and repercussions of not meeting the staking commitments should be mentioned in the contract between the fellowship and the initiator.

## **Handling Project Duration Exceedance**

### **Completion & Success Acknowledgment**

If a project is approaching or has exceeded its original duration but all parties are in agreement with the work's quality and direction, the current project should be marked as successfully completed.

This allows for the distribution of the locked funds: fellowship members receive their fees, the staked $POLN is returned, and the initiator obtains its reward.

### **Initiating a Continuation Project**

In cases where more time is required to achieve the final goal or to continue with new phases, a new project should be initiated.

The initiator can create a follow-up project that can be seen as a continuation of the previous one.

This "sequel" project can be templated from the previous one for efficiency, with adjustments made to reflect the new scope, duration, and conditions.

### **Transparency & Transition**

The transition from the original to the continuation project should be seamless and transparent. Notifications should be sent to all involved parties to ensure clarity.

It's advantageous as this process reduces the risks associated with longer projects and ensures regular assessment and rewards distribution.

### **Benefits**

By treating the need for extra time as a new project, both the initiator and the fellowship can regularly reassess conditions, preventing any potential drift in objectives.

This structure also ensures timely payouts, rewards, and a consistent sense of accomplishment and progression for all parties involved.

## **Termination Option**

If both parties can't agree on the terms of the extension, there should be an option for the initiator to terminate the project.

In such cases, the payout to the fellowship would be proportional to the work completed, and the staked $POLN would be returned to the fellowship after deducting any penalties if applicable.

{% hint style="success" %}
This phase primarily focuses on ensuring financial security and fostering trust among all participants, thus ensuring smooth project execution. In essence, the goal is to provide flexibility while ensuring fairness and transparency. This safeguards the interests of both the initiator and the fellowship in cases of project duration extensions.
{% endhint %}