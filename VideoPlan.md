
# Video Plan

Slide: Introduction

Safeguarding citizens privacy and ownership of their personal data 
How might we build telemetry and data insights without compromising citizen privacy? 

Building Citizen’s Trust in this Digital World
In order to access online services, citizens need to give their consent for their data to be used. How do you gain their trust that their data will be used appropriately? 

Narration:
Hello this is Luke from Team "Secure Identity" and my project is 21st century Identity, Privacy and Data Management. 

My presentation revolves around these two questions. How can we bring our identities and associated private data into the digital 21st Century? 

The answer - Self Sovereign Identity. A blockchain powered privacy ledger that provides identity and credential verification. My project is a  research document establishing what is Self-Sovereign Identity, how does it work and how can it be mapped to existing government services?  

But first we must look at the status quo, how is Self Sovereign Identity different to digital identities managed in today's society?


Slide: 

How does a blockchain SSI like opensource Hyperledger Indy work? More comprehensive examples are included in the research document, but for the sake of brevity I'll cover the basics here. The system has Issuers which can provide credentials and write anonymous cryptographic registration information onto the blockchain for later verification, Users And Digital Wallets which requests and manage their own credentials. Credentials can be broken down into smaller parts and data mixed and matched across multiple credentials without effecting verification and provers, who request credential proof when accessing services / organisations. Once the user supplies a credential, the prover consults the block chain and uses the original registration information to verify that the credential was issued by a trusted authority.





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



