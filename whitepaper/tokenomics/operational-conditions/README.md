---
description: >-
  Operational conditions within PoLN's tokenomics underpin the token's
  real-world utility, fostering engagement and enhancing ecosystem value,
  balancing functionality with economic incentives.
cover: ../.gitbook/assets/conditions.png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# ⛏ (preview) Operational Conditions

The PoLN protocol operates within a set of phases, each carefully designed to ensure transparency, efficiency, and commitment from all parties involved. These operational phases lay the foundation for the protocol's functioning and streamline the project lifecycle. 

Here's a brief overview:

1. **Initiator's Project Description and Posting:** This phase is the starting point, focusing on how an initiator outlines a project. It emphasizes setting clear parameters and handling confidentiality concerns, ensuring the project's requirements are well-understood by potential bidders.
2. **Fellowship Formation and Bidding:** A core phase where fellowships are formed, harnessing diverse skillsets and expertise. The bidding process is also elucidated, detailing how fellowships showcase their capabilities and propose their strategies for project execution.
3. **Staking & Payment Locks:** This segment underscores the commitment aspect of the protocol. Through staking mechanisms, both the fellowship and initiator guarantee their dedication to the project, ensuring that they have skin in the game.
4. **Project Execution & Evaluation:** At the heart of the protocol lies the actual execution of the project. This phase delves into the nuts and bolts of project management, with an emphasis on continuous monitoring and evaluation from both the initiator's and the fellowship's vantage points.
5. **Reward & Fee Distribution:** The culmination of the project lifecycle, this phase breaks down the distribution of rewards and fees. It provides clarity on how dues are settled, whether in the case of successful project completion or potential failures.

## **Staking & Payment Locks**

<figure><img src="../.gitbook/assets/_whyvrafvr_cubes_843b0dd3-bafb-4dff-8d3b-ae5788721c60.png" alt="" width="563"><figcaption></figcaption></figure>

In the realm of PoLN's operational dynamics, this phase serves as a foundational checkpoint, ensuring both initiator and fellowship commitment.&#x20;

By mandating staked assets and locking payments, it infuses the ecosystem with accountability, while safeguarding the interests of all participants.

### **Purpose of Staking**

Staking is not just a formality within the PoLN protocol. It serves a multi-fold purpose:

#### **Skin in the Game**

The staking mechanism is designed to ensure that fellowships are genuinely committed to the success of a project. By staking $POLN tokens, they are essentially putting their resources on the line, signaling their confidence in the successful execution of the project.

#### **Potential Rewards**

Upon the successful completion of the project, fellowships retrieve their staked amount and earn the protocol fees as their reward. If the project fails, they risk losing their entire staked amount.

#### **Deterrence against Malfeasance**

Staking serves as a deterrent against any potential malicious intentions or lackluster commitment from the fellowship. Their direct financial stake in the project's outcome ensures that they remain incentivized for the project's success.

### **Dynamic Staking Amounts**

While there is a minimum staking requirement of 10% of the total project fees set by the initiator, fellowships can choose to stake any amount above this threshold.&#x20;

By staking higher amounts, fellowships might portray a heightened level of confidence and commitment to the project, potentially influencing the initiator's bid selection process.

### **Initiator's Fee Payment & Contractor Provisioning**

Upon the acceptance of the fellowship's bid and their subsequent staking of the committed $POLN tokens, the initiator is responsible for two key financial elements:

* Paying the agreed-upon fees for the protocol.
* Provisioning the payment intended for the contractor's work/delivery.

Both these amounts are securely locked in an escrow smart contract.&#x20;

This ensures not only the availability of funds for fee distribution upon project completion but also guarantees the contractor's payment for the services rendered.

### **Protection Mechanism & Assurance**

Both the fellowship's staked tokens and the initiator's locked fees, alongside the provisioned contractor payment, are securely stored in smart contracts on the blockchain.&#x20;

This structure serves multiple purposes:

* The contractor is assured of payment upon successful delivery, fostering trust and motivation.
* The fellowship can retrieve their staked tokens upon the project's success, ensuring their financial security.
* The initiator's commitment to the project is visibly represented by the locked-in funds, emphasizing the seriousness and genuine intent behind the project.

### **Release of Payments & Stakes**

#### **Distribution of Locked Fees**

Upon successful completion of the project and validation from the initiator, the locked protocol fees are distributed amongst all members of the fellowship based on previously agreed-upon ratios.

#### **Return of Fellowship's Stake**

Alongside the release of the protocol fees, the fellowship's staked $POLN tokens are unlocked and returned to them, signifying the successful execution and delivery of the project.

#### **Payment to the Contractor**

The agreed payment for the contractor's services is released as per the predefined invoicing schedule or milestones.

This ensures that all parties are fairly compensated for their roles and contributions upon project completion.

### **Project Failure Scenarios**

When a project does not achieve its desired objectives or fails, the following mechanisms will come into play:

#### **Distribution of Protocol Fees**

If the project is deemed a failure, the entire protocol fees paid by the initiator will be distributed among the broader community rather than the fellowship.

#### **Loss of Fellowship's Stake**

In the event of a project's failure, the fellowship's staked $POLN tokens are burnt, representing a direct financial loss to the fellowship.

#### **Initiator’s Reward**

The initiator does not receive their reward in the case of project failure.

These measures aim to maintain the integrity of the system, hold fellowships accountable, and ensure they remain genuinely committed to the projects they decide to undertake.

### **Dispute Resolution**

In the initial stages of the PoLN protocol, disputes between the initiator and the fellowship will be handled based on a predefined set of guidelines and criteria.&#x20;

These criteria will serve as a framework to determine the release or forfeiture of locked funds. They could include, but are not limited to:

* [ ] **Project Delivery Assessment:** This will focus on whether the project was delivered as per the outlined specifications and requirements.
* [ ] **Timelines:** If the project was delivered within the agreed-upon time or if there were delays, and the reason for such delays.
* [ ] **Quality of Work:** An evaluation of the work's quality compared to industry standards or previous work from the contractor.
* [ ] **Communication:** Regularity, clarity, and promptness of communication between parties during the project's duration.
* [ ] **Feedback Loops:** The efficiency in addressing feedback or changes requested by the initiator during the course of the project.

In the future, as the PoLN ecosystem matures, there is an aspiration to integrate a decentralized arbitration system.&#x20;

This would involve community members or designated arbitrators who, in case of disagreements, would weigh in based on evidence presented by both parties. This system would not only bolster the trust within the community but also ensure more fairness and decentralization in the resolution process.

### **Timely Provisions by Initiator**

Post bid acceptance, the initiator has a grace period (e.g., 1 week) to provision the contractor's payment and pay the required PoLN fees.&#x20;

Should the initiator fail to meet these obligations within the set timeframe:

* The project is marked as "Aborted".
* Fellowships are notified that the project has not commenced due to payment failures.
* The stipulations surrounding such scenarios should be explicitly outlined in the contract between the fellowship and the initiator.
* Upon the project's status being marked as "Aborted," the fellowship can retrieve its staked amount without any penalties. The project then reverts to its original state, and if no action is taken, it will eventually be discarded after the specified deadline.

### **Fellowship's Staking Commitment**

If a fellowship, after winning the bid, fails to stake the agreed-upon amount within the specified period:

* The initiator is alerted and has the discretion to choose an alternative fellowship or await the initial fellowship's compliance.
* The initial project bid by the fellowship is considered void or cancelled.
* Here too, the conditions and repercussions of not meeting the staking commitments should be mentioned in the contract between the fellowship and the initiator.

### **Handling Project Duration Exceedance**

#### **Completion & Success Acknowledgment**

If a project is approaching or has exceeded its original duration but all parties are in agreement with the work's quality and direction, the current project should be marked as successfully completed.&#x20;

This allows for the distribution of the locked funds: fellowship members receive their fees, the staked $POLN is returned, and the initiator obtains its reward.

#### **Initiating a Continuation Project**

In cases where more time is required to achieve the final goal or to continue with new phases, a new project should be initiated.&#x20;

The initiator can create a follow-up project that can be seen as a continuation of the previous one.

This "sequel" project can be templated from the previous one for efficiency, with adjustments made to reflect the new scope, duration, and conditions.

#### **Transparency & Transition**

The transition from the original to the continuation project should be seamless and transparent. Notifications should be sent to all involved parties to ensure clarity.&#x20;

It's advantageous as this process reduces the risks associated with longer projects and ensures regular assessment and rewards distribution.

#### **Benefits**

By treating the need for extra time as a new project, both the initiator and the fellowship can regularly reassess conditions, preventing any potential drift in objectives.&#x20;

This structure also ensures timely payouts, rewards, and a consistent sense of accomplishment and progression for all parties involved.

### **Termination Option**

If both parties can't agree on the terms of the extension, there should be an option for the initiator to terminate the project.&#x20;

In such cases, the payout to the fellowship would be proportional to the work completed, and the staked $POLN would be returned to the fellowship after deducting any penalties if applicable.

{% hint style="success" %}
This phase primarily focuses on ensuring financial security and fostering trust among all participants, thus ensuring smooth project execution. In essence, the goal is to provide flexibility while ensuring fairness and transparency. This safeguards the interests of both the initiator and the fellowship in cases of project duration extensions.
{% endhint %}

## **Project Execution & Evaluation**

In the decentralized ecosystem facilitated by the PoLN protocol, the protocol serves primarily as a trust layer, ensuring staking, fee management, and reward distribution. However, project execution largely follows the agreed terms between the initiator and the fellowship, outside of the protocol's direct oversight.

### **Project Execution**

While the PoLN protocol isn't a comprehensive project management solution, it does establish the foundational elements of trust and commitment. Once a project commences:

* The initiator and fellowship operate based on their agreement, likely leveraging external project management tools or communication platforms such as Discord, Telegram, or WhatsApp.
* Progress markers or milestones might be established in the agreement, serving as checkpoints. These checkpoints can be tied to payment releases or updates within the PoLN protocol, allowing for transparent tracking of project progression.

### **Project Evaluation**

Evaluation is critical to ensure both the initiator's satisfaction and the fellowship's proper compensation. A few potential evaluation criteria could be:

* [ ] **Completion Accuracy:** How closely does the finished product align with the original project description and requirements?
* [ ] **Timeliness:** Did the fellowship complete the project within the stipulated timeframe? Were milestones achieved as scheduled?
* [ ] **Quality of Work:** Beyond mere completion, is the work of a high standard, meeting or surpassing industry benchmarks?
* [ ] **Quality of Communication:** Were updates, issues, and changes communicated effectively and promptly by the fellowship? Did the fellowship maintain transparency throughout the process?
* [ ] **Resource Management:** Were resources, both in terms of budget and manpower, utilized efficiently? Did the fellowship stick to the budgetary confines, if any were set?
* [ ] **Stakeholder Feedback:** This incorporates feedback not just from the initiator but also from any other affected parties, ensuring a holistic review of the project's impact.
* [ ] **Adaptability:** How did the fellowship handle unforeseen challenges or obstacles? Was there agility in problem-solving and finding alternative solutions?
* [ ] **Team Collaboration:** If the project involved multiple members from the fellowship, how well did they collaborate? Was there cohesion in the team's efforts?
* [ ] **Technology and Innovation:** Did the fellowship employ the latest technologies, methodologies, or innovative solutions suitable for the project?
* [ ] **Ethical Considerations:** Were all stages of the project executed ethically, respecting all involved parties, data protection standards, and industry best practices?
* [ ] **Client Satisfaction:** Beyond the tangible outcomes, was the initiator or client content with the working relationship, the fellowship's responsiveness, and overall experience?
* [ ] **Value for Money:** Considering the fees involved, did the fellowship provide a result that signifies good value for the money invested by the initiator?
* [ ] **Knowledge Transfer:** If applicable, did the fellowship provide adequate training, documentation, or support for the initiator to understand and utilize the delivered product or service?
* [ ] **Environmental and Social Impact:** Especially relevant for larger projects, was there consideration of environmental sustainability and positive social impact?
* [ ] **Post-Completion Support:** Was there a mechanism for addressing post-completion queries, concerns, or required tweaks? How committed was the fellowship in ensuring smooth transition post-project?

{% hint style="info" %}
These criteria can serve as a detailed checklist for initiators to assess the performance of a fellowship upon project completion, ensuring a holistic review and understanding of the engagement's success.
{% endhint %}

### **Fellowship's Retrospective Evaluation on Initiator Interaction**&#x20;

In the dynamic landscape of project collaboration, mutual feedback is crucial. While initiators play an instrumental role in defining and driving projects, the fellowship's experiences and interactions with them often dictate the smoothness of the collaboration. This evaluation offers fellowships an opportunity to reflect upon and articulate their experiences with the initiator. The insights gathered here are not just invaluable for continuous improvement but also set the stage for more fruitful collaborations in the future. Through this lens, every actor in the fellowship—be it an agent, mentor, or contractor—brings a unique perspective, ensuring a comprehensive understanding of the collaborative dynamics.

#### Evaluation by Agents:

1. **Clarity & Communication**:
   * [ ] Were the project's goals and requirements clearly defined by the initiator?
   * [ ] Was the initiator receptive to clarifications and modifications?
   * [ ] How responsive and communicative was the initiator throughout the project?
2. **Resource Provision**:
   * [ ] Did the initiator provide all necessary resources and accesses in a timely manner?
   * [ ] Were there any unnecessary delays due to unavailability of critical information or resources from the initiator?
3. **Feedback & Flexibility**:
   * [ ] Was the initiator open to modifications or changes based on unforeseen challenges?
   * [ ] How often did the initiator provide constructive feedback?
4. **Payment & Compensation**:
   * [ ] Were all financial transactions, including compensation, timely and as per the agreement?
5. **Overall Experience**:
   * [ ] Would the agent consider working with this initiator again in the future?
   * [ ] Any particular areas of improvement for smoother collaborations in the future?

#### Evaluation by Mentors:

1. **Knowledge Transfer & Receptivity**:
   * [ ] Was the initiator open to suggestions and guidance provided?
   * [ ] How effectively could mentorship be imparted to the project teams or the initiator?
2. **Scope & Challenges**:
   * [ ] Did the project's scope remain consistent, or were there frequent changes?
   * [ ] Were challenges and roadblocks addressed proactively?
3. **Collaboration**:
   * [ ] How collaborative was the initiator in terms of problem-solving and brainstorming?
   * [ ] Were the insights and expertise of the mentor respected and valued?
4. **Feedback & Recognition**:
   * [ ] Was the mentor's role acknowledged and contributions recognized?
   * [ ] Was there any feedback loop established for the mentor’s own improvement?
5. **Overall Mentorship Experience**:
   * [ ] Was the mentorship role fulfilling in this particular project?
   * [ ] Any areas where the mentorship process can be enhanced for future projects?

#### Evaluation by Contractors:

1. **Task Definition & Clarity**:
   * [ ] Were the tasks and deliverables clearly defined?
   * [ ] How frequently did the contractor have to seek clarifications on assigned tasks?
2. **Support & Resources**:
   * [ ] Was there ample support from the initiator in terms of resources, information, and tools?
   * [ ] Were there any hindrances in execution due to lack of support?
3. **Feedback & Revision**:
   * [ ] How timely and constructive was the feedback on the submitted work?
   * [ ] Were there excessive revisions or changes asked for post-submission?
4. **Work Environment & Relationship**:
   * [ ] If the contractor had to work on-premises or in collaboration with the initiator's team, how was the work environment?
   * [ ] Was there respect for the contractor’s time and expertise?
5. **Compensation & Timeliness**:
   * [ ] Were the payments made as per the agreed schedule?
   * [ ] Were there any disputes regarding compensation, and if so, how were they handled?
6. **Overall Contracting Experience**:
   * [ ] Based on the project experience, would the contractor be open to future projects with this initiator?
   * [ ] What improvements can be made for a smoother contractor-initiator relationship?

{% hint style="info" %}
These evaluations allow the fellowship to reflect on their collaboration with the initiator and assess areas of strength and potential improvement. The aim is to foster a culture of continuous learning and improvement within the PoLN ecosystem.
{% endhint %}

{% hint style="success" %}
Post-evaluation, based on the initiator's assessment, the PoLN protocol can then facilitate the release of locked fees to the fellowship and return the staked tokens.
{% endhint %}

{% hint style="warning" %}
It's essential to note that while the PoLN protocol offers a structure for these interactions, the detailed dynamics of project execution and evaluation are largely dictated by the agreement between the initiator and the fellowship.
{% endhint %}

## Reward & Fee Distribution

In the decentralized world of PoLN, the act of compensating contributors for their efforts is paramount. This reward and fee distribution phase seeks to ensure that all stakeholders, be it initiators, fellowships, or the broader community, are fairly remunerated for their roles. Here, we delve into the intricacies of how value is allocated and distributed across the protocol, ensuring that there's skin in the game, commitment is sustained, and quality is continuously delivered. The system is meticulously designed, integrating a robust reward matrix for initiators based on project duration and a well-structured distribution plan for protocol fees. By doing so, PoLN creates a harmonious ecosystem where contributors are incentivized to align with the platform's objectives, leading to better outcomes for all. Dive in to understand the precision with which PoLN has crafted its reward and fee distribution mechanism.

### **Success Scenario**

Upon the successful completion of a project, the distribution system activates:

* **Fellowship:** The fellowship retrieves its staked tokens, and in addition, they are awarded the protocol fees as their primary remuneration.
* **Initiator:** The initiator gets rewarded from a predefined token pool based on the project's duration and the associated unit. The reward calculation is based on a matrix/grid system that considers both the project's duration and its time unit. As an example, for an 8 months long project, the initiator would receive 65536 $POLN.

### **Unsuccessful Scenario**

In the event a project is deemed unsuccessful:

* **Fellowship:** The fellowship loses its staked tokens as they are burnt, which incurs a financial loss for them. They also miss out on the protocol fees.
* **Initiator:** The initiator does not receive any reward.
* **Community:** The protocol fees, which would have otherwise gone to the fellowship, are redirected to the broader community. These funds are used for operations like training, helpdesk and support, mediation, KYC, development, maintenance, and refilling the initiator rewards pool.

### **Aborted Projects**

If a project is terminated before its set deadline:

* **Fellowship:** The fellowship's staked tokens are burnt.
* **Initiator:** The initiator can claim back the remaining payment that was locked for the contractor since they will no longer be getting paid. However, the initiator does not receive any rewards, and any protocol fees already paid are not refunded.
* **Community:** The community receives the protocol fees for their continued operational support.

### **Halving Mechanism for Initiator Rewards**

To ensure the sustainability of the reward system, there's a halving mechanism in place. As the token pool for initiator rewards depletes and reaches a reduction of 50%, the reward rates for initiators will be halved. This ensures that even as the available tokens in the pool reduce, the system can continue rewarding initiators for a longer period, thereby maintaining the attractiveness and viability of the PoLN platform.

{% hint style="success" %}
This mechanism ensures that all the stakeholders in a project, be it the initiator, the fellowship, or the community, have a clear understanding of the potential gains or losses. It emphasizes both the rewards for successful completion and the penalties for failures, thereby motivating all parties to maintain high standards of work and commitment.
{% endhint %}

***

{% hint style="info" %}
While the operational conditions outlined above establish the foundational framework of PoLN's operations, there are additional dimensions which, though not yet detailed extensively, are pivotal for the protocol's long-term evolution and optimization.



These include:

* **Dispute Resolution:** A vital aspect that could be further expanded upon, focusing on structured mechanisms to handle disagreements or unmet expectations.
* **Continuous Learning & Platform Improvement:** Embracing feedback from past projects can offer invaluable insights. This phase would emphasize refining the platform and fostering a culture of continuous learning among fellowships.
* **Community Engagement & Governance:** Democracy and decentralization are at the heart of blockchain protocols. This phase would foster a sense of ownership among the PoLN community, enabling members to have a say in decision-making and protocol evolution.
* **Onboarding & Training:** As PoLN grows, welcoming new members and ensuring they are well-acquainted with the platform's ethos will be crucial. This phase would ensure smooth assimilation and adherence to best practices.
{% endhint %}

{% hint style="success" %}
In the dynamic world of blockchain protocols, adaptability and a forward-looking approach are paramount. These potential phases, if integrated, can further bolster PoLN's stature as a premier platform, driving innovation while ensuring robust operational standards.
{% endhint %}
