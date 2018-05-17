# Client Removal Template

#### This pull request should add the documentation of data destruction. Merges should only be performed by a Principal.

## Tasks to be completed when opening

 - [ ] Pull request title is "Data Destruction - Client Name" (e.g. `Data Destruction - ABC Health System (0273ABC)`)

## Summary Information

**Client Name:** `ABC Health System`

**Client Code:** `0273ABC`

## Task list to work through during life of pull request

 - [ ] Document the scope of data to be destroyed and the reason for destruction
 - [ ] Link this pull request to any relevant client removal pull request
 - [ ] Gather all the required documentation below
 - [ ] If published reports are included in the scope of data to destroy, Open an issue in the [hosting repository](https://indy-github.milliman.com/PRM/qlikview-hosting) using [this template](https://indy-github.milliman.com/raw/PRM/qlikview-hosting/master/templates/Client%20Removal%20Request.md) to request removal of any in-scope reports from the hosting infrastructure.
 - [ ] Remove any in-scope data from network drives
 - [ ] Engage the DBA to remove any in-scope data from databases:
    - [ ] Live databases
    - [ ] Development/test databases
    - [ ] Database backups (if no out of scope data exists in the database)
 - [ ] Complete the [Certification of Data Destruction](https://indy-github.milliman.com/PRM/client-and-project-documentation/blob/master/templates/Data_Destruction_Certification_Template.doc) and add to the client's folder in this repository
    - [ ] Ask Indy IT to determine whether tape backups might reasonably exist for the client's data. If so, include the disclaimer language.
    - [ ] If database backups include data not in-scope for the request, include the disclaimer language.
 - [ ] @mention/assign a principal for final review, signature, and merging

## Required Documentation

The documents below should be included as files in this pull request (i.e. after merging they will exist in the "code" section of this repository).

 - [ ] The client's original request for data Destruction
 - [ ] A signed copy of the Certification of Data Destruction
