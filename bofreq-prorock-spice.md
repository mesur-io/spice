# Name: Secure Patterns for Internet CrEdentials (SPICE)

## Description

There is a need to more clearly document verifiable credentials - that is credentials that utilize the issuer, holder, and verifier (three party) model across various work IETF, ISO, W3C, and other SDOs.  This need particularly arises in use cases for verifiable credentials that do not involve human-in-the-loop interactions, need strong and long lived identifiers for business entities, and for those that require CBOR encoding, and those that leverage the cryptographic agility properties of COSE. Based on these use cases, there is a need to clearly define message formats and supporting mechanisms.  Additionally, multiple groups at the IETF need a clear definition for what architectures might exist and should be leveraged for certain use cases related to credentials following this three party model, and to identify where there are gaps or new architectural concepts that need to be defined.

By ensuring that we cover those topics and directly point to appropriate standards developed in other groups at IETF and elsewhere, we can also help avoid the re-creation of existing items and re-introduction of security concerns that have already been dealt with in broadly deployed and well-understood standards. 

This work will answer the need for a common set of language for use in describing broader concepts related to the use of verifiable credentials with the three-party model (issuer, holder, verifier) with optional selective disclosure, external status representation, and other privacy-focused capabilities within a variety of credential presentation scenarios, while ensuring that adequate review from across the IETF / IRTF occurs for this work.

## Required Details

- Status: WG Forming
- Responsible AD: Roman Danyliw
- BOF proponents: Mike Prorock <mprorock@mesur.io>, Heather Flanagan <hlf@sphericalcowconsulting.com>, Leif Johansson <leifj@sunet.se>, Brent Zundel <brent.zundel@gendigital.com>, Henk Birkholz <henk.birkholz@sit.fraunhofer.de>
- BOF chairs: TBD
- Number of people expected to attend: 60
- Length of session (1 or 2 hours): 2 hours
- Conflicts (whole Areas and/or WGs)
  - Chair Conflicts: TBD
  - Technology Overlap: OAUTH, SCITT, RATS, COSE, CBOR, JOSE, WIMSE, MLS, MIMI
  - Key Participant Conflict: COSE, JOSE, CFRG, OAUTH, RATS, OPSAWG, IOTOPS, SCITT

## Information for IAB/IESG

To allow evaluation of your proposal, please include the following items:

- Any protocols or practices that already exist in this space:
  - https://openid.net/specs/openid-4-verifiable-credential-issuance-1_0.html
  - https://openid.net/specs/openid-4-verifiable-presentations-1_0.html
  - https://openid.net/specs/openid-connect-self-issued-v2-1_0.html
  - https://developer.apple.com/documentation/passkit/wallet/verifying_wallet_identity_requests?language=objc
  - https://chapi.io/ 
  - https://identity.foundation/presentation-exchange/ 
  - https://w3id.org/traceability/interoperability
  - https://datatracker.ietf.org/doc/draft-barnes-mls-userinfo-vc/  
  - Verifiable Credentials Data Model v1.1 (w3.org)
  - Decentralized Identifiers v1.0 (w3.org)

- Which (if any) modifications to existing protocols or practices are required:
  - The group will try to avoid modification to existing protocols and practices
- Which (if any) entirely new protocols or practices are required:
  - TBD based on scope of group - there is some chance that there is a practice shift towards enforced data-minimization through selective disclosure as a preferred mode of operations when working with credentials
- Open source projects (if any) implementing this work:
  - TBD based on scope of group

## Agenda

### Problem Statement (30 min)

- Problem Area and introduction to verifiable credentials
- Known Use Cases
- How is SPICE related to other IETF Work

### Scope and Proposed Work Items (45 min)

- SPICE Use Cases Documentation
- Selective Disclosure with CWTs
- Architecture
- Other Items that might be considered for inclusion in this group

### Discussion (45 min)

- Is the IETF the right place to do this work?
- Which organizations and SDOs need to be involved/collaborated with?
- What are the expected technical challenges?
- Is there interest in implementing such specifications?
- Is the technology likely to get deployed?
- Is there enough interest in helping with the work (spec editing, reviewing, implementing, deploying)?

## Links to the mailing list, draft charter if any, relevant Internet-Drafts, etc.

- Mailing List: TBD (requested: https://www.ietf.org/mailman/listinfo/spice)
- Draft charter: https://docs.google.com/document/d/1-5N8Wc-0RmXUDWhUbxCL2UMbn7X9UVnH_NCcBh6DZWY/edit 
- Relevant Internet-Drafts:
  - Use Cases:
    - https://datatracker.ietf.org/doc/draft-prorock-spice-use-cases/
  - Solutions:
    - https://datatracker.ietf.org/doc/draft-prorock-cose-sd-cwt/
