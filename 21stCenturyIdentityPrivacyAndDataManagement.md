# 21st Century Identity, Privacy and Data Management

A Digital identity revolution is coming. Self-Sovereign Identity (SSI) is a complete inversion of current identity management, giving granular control of personal data to the user. This has exciting and broad ramifications for user privacy, data collection and data transfer. How can governments and organisations  both facilitate and make use of this new model of identity and personal information transfer and management?

This document is broken down into chapters.
- Chapter one explains digital identities and how they have evolved over time.
- Chapter two explores current issues with identity and personal data management. 
- Chapter three investigates Self-Sovereign Identity software solutions, blockchains and the application layer which could sit on top. 
- Chapter four looks at government datasets and data flows and how they could be implemented through a SSI foundation.
- Chapter five summarises the findings.


Questions: What is your identity? How do you prove your identity? How do you trust another person's identity? How does the government use your identity? How does the government user your data to provide services?

# Chapter One: The Evolution of Identity

## 1.1 What is a Digital Identity? What is Trust?

Wikipedia defines Digital Identity as "A digital identity is information on an entity used by computer systems to represent an external agent. That agent may be a person, organization, application, or device." 

## 1.2 The History Of Digital Identity

Christopher Allen is co-chair of the W3C Credentials Community Group which is working on standards for decentralised identity. Christopher is a pioneer in internet cryptography and worked with Netscape to develop the SSL security protocol and co-author of the IETF TLS internet draft which was used as the heart of all secure commerce of the World World Web. Christopher breaks down identity management into four stages.

### 1.2.1 Centralised / Traditional (Siloed) Identity

![Centralised Identity](Images/CentralisedIdentity.svg)

This identity model is the traditional form of identity management and the most common. Each organisation / website provides a digital credential for you to use their service.

Trust between the user and the provider is established through the transfer of *shared secrets*, most commonly in the form of a username/password but has expanded out over time into SSH-keys, physical RFID tokens and biometrics. This is known as a siloed system as there is no sharing of data between different organisations - each organisation has a separate and unique credential. 


### 1.2.2 Federated / Third Party Identity

![Federated Identity](Images/FederatedIdentity.svg)

This expands on the centralised identity by providing an identity provider which sits between you and other organisations/services. The identity provider issues the digital credential and acts very similarly to the organisation in the centralised identity model. The identity provider than provides a *single sign-on* experience (usually via a security token) to all organisations that support this identity provider. The major advantage of this model is that it reduces the number of credentials required to be maintained by the user. 

### 1.2.3 User-Centric Identity

![User-Centric Identity](Images/UserCentricIdentity.svg)

This ground-work for this type of identity originated in the white-paper "The Augmented Social Network: Building Identity and Trust into the Next-Generation Internet". The main idea being that "Every Individual ought to have the write to control his or her own identity". A simplified idealised workflow of this identity management:
- A user attempts to use a service and the services queries for identity
- The user then authenticates with a trusted identity provider and asks a for a signed identity letter from the provider stating who the user is. The user then sends this letter to the organisation. If the user cannot authenticate, the provider will return a failure. 
- The service then reads the signed letter and decides to trust the user based on the trust that the service has in the original identity provider. If the user cannot produce a certified letter, the service will prevent use or access. 

This identity management is seen in technologies such as OpenID, OAuth and Facebook Connect. 

### 1.2.4 Self-Sovereign Identity 

![Self-Sovereign Identity](Images/SelfSovereignIdentity.svg)

Drummond Reed at Evernym defines SSI as a “lifetime portable identity for any person, organisation, or thing that does not depend on any centralised authority and can never be taken away". Self-Sovereign Identity expands upon User-Centric Identity idea - placing the user directly in control of their own credentials in a digital wallet. The specific workings of this technology will be expanded in the following sections. 

### 1.2.5 Chapter References: 


Christopher Allen, 2016. "[The Path to Self-Sovereign Identity](http://www.lifewithalacrity.com/2016/04/the-path-to-self-soverereign-identity.html)"

Timothy Ruff, 2018 "[The Three Models of Digital Identity Relationships](https://medium.com/evernym/the-three-models-of-digital-identity-relationships-ca0727cb5186)"

Marcos Allende Lopez, 2020. Inter-American Development Bank. "[Self-Sovereign Identity - The future of Identity: Self-Sovereignity, Digital Wallets, and Blockchain](https://publications.iadb.org/publications/english/document/Self-Sovereign-Identity-The-Future-of-Identity-Self-Sovereignity-Digital-Wallets-and-Blockchain.pdf)"

Wikipedia contributors. (2021, August 1). Single sign-on. Wikipedia, The Free Encyclopedia. Retrieved 11:28, August 21, 2021. "[Single Sign-on](https://en.wikipedia.org/w/index.php?title=Single_sign-on&oldid=1036527960)"

Jordon, Ken, Jan Hauser, and Steven Foster. 2003. [“The Augmented Social Network: Building Identity and Trust into the Next-Generation Internet”](http://asn.planetwork.net/asn-archive/AugmentedSocialNetwork.pdf)

John Phillips. Interview. 2018. Australian Payments Summit. "[Self Sovereign Identity](https://www.auspaynet.com.au/insights/Blog/Self-Sovereign-Identity)"

# Issues with the Current System

<ins>Risks</ins>

**Data Silos** - Large Centralised Identity providers have access to millions of digital identities which makes them a target. (For example Yahoo and Equifax Data Breaches.)

**Lack Of Transparency** - How is user data being used? (Is it marketing? Political Analysis?).  Is it being transferred to additional third parties?  (Facebook–Cambridge Analytica data scandal)

**Re-Identification of other Data Sets** - By cross-referencing information contained in their databases, centralised providers may be able to reidentify existing public datasets. 



# Current Software Solutions

## Sovrin

## ESSIF - European Self Sovereign Identity Framework


# Dataset Case Studies - A Glimpse at the Future

## Re-imaginging Employment






Chapter References:
https://github.com/hyperledger/indy-sdk/blob/master/docs/getting-started/indy-walkthrough.md

## Covid-19

## Health

## Data Collection / Surveys

## Privacy Accounting

# Concerns

# Summary

<sup id="a1">[1](#identrev)</sup>

<a id="identrev">1</a>: This is a footnote.[↩](#a1)