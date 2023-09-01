# Secure Patterns for Internet CrEdentials (SPICE) at IETF - Proposed Charter

## Introduction

There is a need to more clearly document verifiable credentials - that is credentials that utilize the issuer, holder, and verifier (three party) model across various work IETF, ISO, W3C, and other SDOs.  This need particularly arises in use cases for verifiable credentials that do not involve human-in-the-loop interactions, need strong and long lived identifiers for business entities, and for those that require CBOR encoding. Based on these use cases, there is a need to clearly define message formats and supporting mechanisms.  Additionally, multiple groups at the IETF need a clear definition for what architectures might exist and should be leveraged for certain use cases related to credentials following this three party model, and to identify where there are gaps or new architectural concepts that need to be defined.

By ensuring that we cover those topics and directly point to appropriate standards developed in other groups at IETF and elsewhere, we can also help avoid the re-creation of existing items and re-introduction of security concerns that have already been dealt with in broadly deployed and well-understood standards. 

This work will answer the need for a common set of language for use in describing broader concepts related to the use of verifiable credentials with the three-party model (issuer, holder, verifier) with optional selective disclosure, external status representation, and other privacy-focused capabilities within a variety of credential presentation scenarios, while ensuring that adequate review from across the IETF / IRTF occurs for this work.

## Goals

The SPICE working group aims to achieve several important goals. It will first specify an informational document that outlines the use cases commonly encountered when working with the verifiable credentials that are used within the three party model. Second, a proposed standard reference architecture document will be created. This architecture document will at minimum provide clear guidelines for system-to-system exchange of credentials. Third, at least one mechanism to support selective disclosure with CBOR credentials will be proposed for standardization.  Additionally, identifying or providing a proposed standard for how to provide identities and key material associated with verifiable credentials in use with IETF work may prove to be highly beneficial.

To ensure comprehensive collaboration and alignment, the working group will actively engage with other international organizations relevant to the problem space, including ISO, OIDF, and the W3C. We aim for this communication and collaboration to help reduce confusion related to the overall space. This collective effort will help pave the way for a robust and interoperable ecosystem across various protocols and systems.  

## Motivating Use Cases

There are several expanding use cases and common patterns that motivate the working group and broader community, including:

- Selective disclosure needs for data in verifiable credentials, especially with CBOR
- Expanding use of topic-specific microcredentials, particularly in education
- Digitization of physical supply chain credentials in multiple jurisdictions requiring CBOR creds at volume with system to system presentations
  - Impending public tests with US CBP, USDA, FDA, and other regulatory agencies
  - product passports
- IoT, Control Systems, and Critical Infrastructure related Credentials
- Credentials related to authenticity and provenance, especially related to digital media
- Offline exchange (in person) of credentials that may have been internet issued
- Embedding of credentials in other data formats
- Digital Wallet Initiatives

Some of these use cases may be solved by the group directly, for others the group may enable a solution by providing supporting specifications.

## Motivating Factors for conducting this work at IETF

- Privacy and security expertise at IETF / IRTF specifically relevant to this work
- Anticipated successful conclusion of the VC 2.0 Working Group at W3C

## Work Items

Documents produced by the working group will include the following:

- Use case document https://datatracker.ietf.org/doc/draft-prorock-spice-use-cases/ 
- Architecture document
- Selective Disclosure with CWTs https://datatracker.ietf.org/doc/draft-prorock-cose-sd-cwt/ 
- TBD Identity Specification

## Milestones

MM YYYY - Submit a Use Case and Terminology document to the IESG for publication  
MM YYYY - Submit an Architecture document to the IESG for publication  
MM YYYY - Submit a document covering selective disclosure with COSE to the IESG for publication  

## Why IETF

Because of the security and integrity aspects directly involved in verifiable credentials that utilize a three party model, particularly their reliance on asymmetric cryptography with possible intermediaries during exchange, this topic must be worked with in cooperation with existing security expertise in the IETF and IRTF.  The broader community engaging in the verifiable credential space is converging within the IETF because of this security expertise. Multiple editors of existing work in W3C related to verifiable credentials are engaged and supportive of this work, and believe that IETF is the appropriate location for this work. By working in IETF we can ensure broader engagement with the work, security, and privacy review by the appropriate experts at IETF, and better coordinate with IETF groups that are leveraging or extending this work for use in various IETF standards.  
