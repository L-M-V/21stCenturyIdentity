
# Video Plan

Slide: Introduction

Safeguarding citizens privacy and ownership of their personal data 
How might we build telemetry and data insights without compromising citizen privacy? 

Building Citizen’s Trust in this Digital World
In order to access online services, citizens need to give their consent for their data to be used. How do you gain their trust that their data will be used appropriately? 

Narration:
Hello this is Luke from Team "Secure Identity" and my project is 21st Century Identity, Privacy and Data Management. 

My presentation revolves around these two questions. How can we bring our identities and associated private data into the 21st Century? 

The answer - Self Sovereign Identity or SSI. SSI is a blockchain powered privacy ledger that provides identity and credential verification. My project is a research document establishing what is Self-Sovereign Identity, how does it work and how can it be mapped to existing government services.

Slide: Traditional Identity Examples

Self Sovereign Identity is different from traditional identity management because it is decentralised and the private data is owned by the user.
Traditional Identity is heavily controlled by individual identity providers which lead them open to attacks and have a distinct lack of transparency in how user data is managed. 

Slide: How does Self Sovereign Identity WOrk 

How does a blockchain SSI work? More comprehensive examples are included in the research document, but for the sake of brevity I'll cover the basics here.
There are three main roles: Issuers, Users and Provers. 

Issuers create digital credentials and add anonymous information to the block chain so that these credentials can be later verified. 

Users - These have a digital wallet which can store requested credentials and respond to proof requests.

Provers - Provers ask users for credential proof when the user attempts to use a service. The user supplies the credential and the prover then consults the block chain to verify that the credential is valid and issued by a trusted authority. 

Credentials do not have to stay as a single immutable block, they can be broken down into smaller parts and the internal data can be mixed and matched across multiple credentials without effecting verification.Credentials can be time-limited and automatically revoked. 

Slide: Enhancing User Privacy

How can SSI be used by governments and to enhance User Privacy and enforce appropriate use of their data? Because all credentials must be explicitly requested from the user, the user can track, log and accept or reject each request. This consent is registered anonymously on the blockchain itself, allowing the parties to independently verify that consent was achieved before data was transferred. Personal data can be transformed (reducing data birth to an over 18 flag for instance) or reduced to only provide necessary information. Governments have a verification chain of where data originated, and citizens have complete ownership of their personal data. No identifiable personal data is stored on the ledger.

In my research document I cover a few example government use cases such as employment and covid-19 check-ins. So where to next? SSI is being actively developed and has seen a huge uptake in the last few years due to the explosion of blockchain technologies and pressure for verifiable vaccine passports. The European Union has invested 5.6 million Euros in the European Self Sovereign Identity Framework over the last couple of years as it looks to provide a government back identity framework for all Europeans. One question remains: How will the Australian And New Zealand Governments take advantage of the next step in digital identity?

Slide: Thank you

Thank you to GovHack and all of the data providers and mentors for the great weekend. Cheers. 








---
# Slides which were too long

Slide: 
Traditional Identity is the backbone of our current internet, you have an account with each organisation and an associated secret to verify yourself and setup trust that you are who you say you are.

Federated Identity was the next identity step, whereby one account could be used across a variety of services (A "Federation"). An identity provider sits as an intermediary between you and these services.

User-Centric Identity: Putting the user in the middle of the process. Credentials are not directly stored on a service, but the service allows you access by trusting the identity provider's certification document or token. 

Self-Sovereign Identity (referred to as SSI from here forth) is a massive expansion on the concept of User-Centric - Evernym defines SSI  as "Lifetime portable identity for any person, organisation, or thing that does not depend on any centralised authority and can never be taken away". 

How does a blockchain SSI like Hyperledger Indy work? Let us consider an employment situation. First, I create a digital identity wallet with a secret key in a phone application. The key is used to prove that any acquired credentials are uniquely mine. I now request my academic transcript from "Programming University". The University known as the issuer adds necessary anonymous registration information onto the ledger before transferring the credential to us so that it can be independently verified. The transcript contains our name, average grade and graduation status. Each piece of data on this credential can be individually used or mathmatically transformed without without effecting it's verifiability. We can now use these pieces of information to fill in the Job Application proof request from GovHack. The requests asks for our name, graduation status and a minimum grade level. Our phone application automatically pre-fills the graduation status, and transforms our average grade value to conditional meeting the minimum grade level. GovHack will not see our average grade, just that we meet it's requirement. We now send our job application to GovHack which will go through each piece of requested data and verify that it was indeed Programming University that provided the credentional by querying the blockchain ledger. 

Let us consider the example of entering a business which requires us to be over the age of 18. Normally we show our government provided ID (which is trusted by both parties). This contains our name, date of birth and address. The business then performs a calculation on the date of birth and then either admits or rejects our request to enter. I'm sure you would agree that there is a lot of un-necessary private information transferred in this process. 

Blockchain SSI works similarly, we first receive a credential from a trusted source, in this case a digital version of our driver's licence. The issuer (the government) adds necessary registration anonymous information onto the ledger before transferring the credential to us. We can then break down this credential without effecting it's verifiability. 



I believe one of the greatest improvements in the flexibility and security that the SSI provides to users. Your driver's licence credential (its number alone) can instantly be used as verification across any number of government services, your vaccine status can provide access to events and businesses without revealing any other medical information. And this is just the credential layer - applications can be built on top once you have established secure communication. 