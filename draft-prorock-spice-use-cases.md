%%%
title = "Use Cases for SPICE"
abbrev = "sd-cwt"
ipr= "trust200902"
area = "Internet"
workgroup = "None"
submissiontype = "IETF"
keyword = ["SPICE"]

[seriesInfo]
name = "Internet-Draft"
value = "draft-prorock-spice-use-cases-latest"
stream = "IETF"
status = "informational"

[pi]
toc = "yes"

[[author]]
initials = "M."
surname = "Prorock"
fullname = "Michael Prorock"
organization = "mesur.io"
  [author.address]
  email = "mprorock@mesur.io"

[[author]]
initials = "B."
surname = "Zundel"
fullname = "Brent Zundel"
organization = "Gen Digital"
  [author.address]
  email = "Brent.Zundel@gendigital.com"

%%%

.# Abstract

This document describes various use cases related to credential exchange
in a three party model (issuer, holder, verifier). These use cases aid
in the identification of which Secure Patterns for Internet CrEdentials
(SPICE) are most in need of specification or detailed documentation.

{mainmatter}

# Notational Conventions

The key words "**MUST**", "**MUST NOT**", "**REQUIRED**", "**SHALL**", "**SHALL NOT**", "**SHOULD**",
"**SHOULD NOT**", "**RECOMMENDED**", "**MAY**", and "**OPTIONAL**" in this
document are to be interpreted as described in [@!RFC2119].

# Introduction

There is a need to more clearly document verifiable credentials - that
is credentials that utilize the issuer, holder, and verifier (three
party) model across various work IETF, ISO, W3C, and other SDOs.  This
need particularly arises in use cases for verifiable credentials that do
not involve human-in-the-loop interactions, need strong identifiers for
business entities, and for those that require CBOR encoding, and those
that leverage the cryptographic agility properties of COSE. This
document which covers multiple use cases for verifiable credentials will
help inform both the required architecture and components, as well as to
help frame needs for any clearly defined message formats and/or
supporting mechanisms.

# SPICE Common Patterns

Within SPICE there are a few common patterns that continually arise:

- A need for selective disclosure with CBOR based verifiable credentials
- Cryptographic agility support via COSE, especially for PQC, and to
  permit use of the same signature algorithms with both selective
  disclosure as well as fully disclosed credentials
- Required strong and long lived identities that are correlated with
  public key material for verifiacation and permit binding to DNS,
  existing x509 certificates, as well as providing ready access to
  public keys for verification utilizing HTTP

# SPICE Use Cases

There are several expanding use cases and common patterns that motivate
the working group and broader community, including:

- Use of microcredentials, particularly in education
- Digitization of physical supply chain credentials in multiple
  jurisdictions
  - CBOR credentials
  - High volume with system to system exchange of credentions
  - both regulatory data as well as business driven information
- IoT, Control Systems, and Critical Infrastructure related Credentials
- Credentials related to authenticity and provenance, especially of
  digital media
- Offline exchange (in person) of credentials that may have been
  internet issued
- Embedding of credentials in other data formats
- Digital Wallet Initiatives

# Use Case Discussion

## Physical Supply Chain Credentials

Physical supply chain credentials create several unique scenarios and
requirements for technical implementers. There is a strong movement
towards digitiztion of physical supply chain data which is often
exchanged in paper or scanned pdf form today using legacy approaches.
Some steps have been taken towards digitatization of supply chain data
in XML, however the steps have proved problematic over native binary
formats due to the complexity, size, and volumes of transmission often
involved.

Common use cases for physical supply chains include:

- Regulatory data capture and exchange with governmental bodies
- Requirements around capturing specific types of data including:
  - Inspection information
  - Permits
  - Compliance certification (both regulatory and private)
  - Traceability information, including change of control and geospatial
    coordinates
- Providing the ability for 3rd parties to "certify" information about
  another actor in the supply chain. e.g. Vendor A is an approved
  supplier for Company X
- Passing of data between multiple intermediaries, before being sent
  along to customs agencies or consignees.
- Moving large amounts of data asyncronously, and bi-directionally over
  a network channel
- Identifying actors in a supply chain and linking them with legal
  entity information

## Credentials related to Authenticity and Provenance

Due to a proliferation of AI generated or modified content, there has
been an increased need to provide the ability to establish the
provenance of digital material.  Questions of authenticity and the means
of creation (human created, machine assited, machine created) also
abound, and in cases where AI generated content, providing the model
information related to the generation of that content is becoming
increasingly important.

Common use cases include:

- Understanding if a received piece of media is human created, and that
  the content is authorized for certain uses.
- Providing the ability to trace training materials for LLMs and similar
  models to output
- Understanding if media was created by an authoritative or trustworthy
  source
  
## Others

TBD

# Security Considerations

TBD

# IANA Considerations

NONE

# Acknowledgements

The authors would like to thank those that have worked on similar items
and/or whom have provided input into this document, especially: Hannes
Tschofenig, Henk Birkholz, Heather Flanagan, Kaliya Young, Orie Steele,
Leif Johansson, Pamela Dingle, Tobias Looker, Kristina Yasuda, Daniel
Fett, Oliver Terbu, and Michael Jones.

{backmatter}
