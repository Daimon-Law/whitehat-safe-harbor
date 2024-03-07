<p align="center">
  <img src="assets/Security-Alliance-Logo-Blue.svg" alt="SEAL"/>
</p>

# Whitehat Safe Harbor

The Whitehat Safe Harbor initiative is a framework in which protocols can offer legal protection to whitehats who aid in the recovery of assets during an active exploit.

## What's in this repo?

This is a fork and re-write of the LeXpunK version created by Daimon Legal. The files are provided in mark-up and clean form, designed with the following objectives: 
- take into account industry feedback on risk allocation and incentives;
- providing additional clarifications to re-balance risk allocation and increase certainty for Whitehats; and
- improve overall readability and future updates of the agreement by overhauling clause numbering, consolidating definitions and making numerous other structural improvements.

There are 2 key documents in this repository:
- documents/Agreement Text Only (DL Edits 2024-03).docx - the main legal agreement for adoption by a Protocol along with the support appendices and FAQs defining the framework. This version includes markups and comments provided back to the Security Alliance team here: https://github.com/security-alliance/safe-harbor/discussions/3
- documents/Agreement Text Only (DL Clean Copy 2024-03).docx - clean copy for immediate use.

## How does it work?

The Safe Harbor initiative is a preemptive security measure for protocols, similar to a bug bounty. It is a framework specifically for *active exploits*, i.e. situations where a vulnerability has begun to be exploited by a malicious actor. If a protocol has adopted Safe Harbor before such an incident occurs, whitehats will have clarity on how to act in a potential rescue, and will be more likely to help intervene.

### Protocol adoption

If a protocol has reviewed the agreement, weighed its pros and cons, and is interested in proceeding with adoption, a few steps are required.

Firstly, a decision must be made regarding the agreement's terms, including:
- Which assets are in-scope for the agreement (e.g. any ERC20 token at a specific address)?
- What reward will be given to successful whitehat rescues (e.g. 10% of rescued funds capped at $1m)?
- Where should rescued funds be returned (e.g. a specific multisig or treasury address)?

Once the specifics are determined, a governance proposal should be created for voting on the adoption of Safe Harbor. Exhibit B of the agreement provides details on how this proposal should be structured. For transparency and future on-chain referencing, all relevant documents should be uploaded to IPFS at this stage. If the protocol doesn't have an official on-chain voting procedure, alternative methods can be explored to engage the community in the decision-making process.

If the decision to adopt Safe Harbor becomes official, there are three final steps for adoption:
    
- An "Agreement Fact Page" must be created by the protocol. This provides all information about the protocol's adoption of the agreement, and must be maintained off-chain for anyone to view.
- The "User Adoption Procedures" (Exhibit D of the agreement) must be adapted and inserted into the protocol website's terms-of-service. 
- A governance address must send an on-chain transaction to the Safe Harbor registry contract. This is the legally binding action, so the address calling the registry should represent the decision-making authority of the protocol.

### Whitehat adoption

If a whitehat reads and understands the entire legal framework, they may later be eligible to participate in a whitehat rescue. These rescues should only be taken in very specific circumstances, and it is important to reiterate the following:

- The framework only applies to *active exploits*, and it is a violation of the agreement if the whitehat initiates an exploit themselves.
- The protocol is not responsible for ensuring the whitehat follows the law, and the whitehat can not be protected from criminal charges outside the agreement's scope.
- There are nuances that can affect the agreement's enforceability, and whitehats will assume many legal risks by becoming involved.

If the whitehat decides to proceed with a whitehat rescue, they must follow the process specified in the agreement. This includes transferring rescued funds to the protocol's "Asset Recovery Address" and promptly notifying the protocol of the fund recovery. The whitehat may keep (or later receive) a reward, based on the terms of the agreement.

## Diagram

![Safe Harbor Flowchart](assets/flowchart.png)


