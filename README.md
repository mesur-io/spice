# spice

Secure Patterns for Internet CrEdentials

## Description

There is a need to more clearly document verifiable credentials - that is 
credentials that utilize the issuer, holder, and verifier (three party) 
model across various work at the IETF, ISO, W3C, and other SDOs.  

This need particularly arises in use cases for credentials that do not
involve human-in-the-loop interactions, and  especially in the use and 
construction of CBOR encoded verifiable credentials for use cases outside 
of authentication and authorization.

Based on these use cases, there is a need to clearly define message
formats and supporting mechanisms.  

Additionally, multiple groups at the IETF need a clear definition for
what architectures might exist and should be leveraged for certain use
cases, and to identify where there are gaps or new architectural
concepts that need to be defined.

This repository is a collection of documents related to this proposed
working group.

## Meetings

We currently meet Thursdays:

### Time

EDT/EST, Eastern Daylight Time (US) at 12:00p


DENVER, United States, Colorado (US) at 10:00a


LONDON, United Kingdom, England at 5:00p

### Connection Info

Google Meet joining info
Video call link: [https://meet.google.com/qbz-bnsd-wrv](https://meet.google.com/qbz-bnsd-wrv)
Or dial: ‪(US) +1 651-560-5478‬ PIN: ‪427 092 357‬#
More phone numbers: [https://tel.meet/qbz-bnsd-wrv?pin=4401189395496](https://tel.meet/qbz-bnsd-wrv?pin=4401189395496)

## Contributions

Any and all contributions are expected to adhere to IETF best practices
and guidelines, especially those related to IPR as outlined
[here](https://www.ietf.org/standards/ipr/) and in the [note
well](https://www.ietf.org/about/note-well/).

## General markdown guidelines

# ietf-misc

As a rule, generate a good text version of drafts for submission by the
following:

```bash
$ mmark [DRAFT].md > [DRAFT-XX].xml
$ $EDITOR [DRAFT-XX].xml # ensure -XX is correct - or if you are brave \
# sed -i 's/-latest/-XX/g' [DRAFT-XX].xml
$ xml2rfc [DRAFT-XX].xml
```

Then check drafts for [idnits](https://author-tools.ietf.org/idnits)
