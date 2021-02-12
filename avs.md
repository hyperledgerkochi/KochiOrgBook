## KOB Address Verification Service

## Introduction

- A user uses this service to get a digital domicile credential which proves
their domicile. It is useful in a situation when the user has to prove his/her domicile for
some needs.
- A domicile credential is a proven claim that a particular person reside in a specific area, issued by an authority.
- The domicile credential, driving license and similar documents are currently printed on paper - paper credentials stored in a user's wallets.
- By bringing the concept of digital verifiable credentials to picture, paper credntials are replaced by digital certificates.
- These digital credentials are stored in digital wallets which is an android application which act as a data store on cloud.
## How are digital credentials better ?

1. Problem 1: Centralised Identifiers(A central authority issues the paper credentials, control the credentials and have the right to revoke them). 
- Can revoke documents at any time or an attack can destroy all data.
- Solution: DID gives power back to individuals and a documents on Blockchain cannot be deleted.
2. Problem 2: Paper Credentials are easy to forge: 
- In the current situation, a digitally signed certificate is downloaded and obtained as a printout. It doesnot contain any seals or watermarks.
- Solution: Digital credentials which are protected cryptographically. 
3. Problem 3: Issue of paper credentials depend on the experience and expertise of issuer (Ration card
Address proof – passport, voter card, ration card, electricity bill, water bill, telephone bill, house tax receipt, birth Certificate or SSLC certificate, identity Proof are the documents to be cross checked) and is time consuming (Average time required is 2-3 days).
- Solution: Digital credentials are proven by using crypto calculations and saves time.
4. Problem 4: Inaccessibility issues:
- Solution: Globally accessible verifiable credentials.

## Key Terms
The four major attributes of any credential are:
1. Issuer(Local Governing Body)
2. If the person producing the credentials is the person to whom the credential was issued to.
3. If claims are tampered(If wrong address is given).
4. If credential has been revoked?

Here digital verifiable credentials are those which are cryptographically constructed and  proves the above attributes.

DID : Decentralized Identifiers are created by owners, independent of any central authority.
- Almost similar to a URL.
- DID is passed to a software called DID Resolver which in turn returns the credential, which is a JSON document which is globally unique.
