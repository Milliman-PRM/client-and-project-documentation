# Client and Project Documentation

This repository is where client and project level documentation is captured and stored. Client level documentation will be added to a client specific folder through a pull request. Documentation for each project will be stored in a separate issue.

The "code" section of this repository contains the various documentation templates and checklists in addition to the client level documentation artifacts (e.g. Conflict Checks).

Deliverable level documentation (e.g. Pre-Release Peer Review) will be captured in the [PRM-Production/qrm-documentation repository](https://indy-github.milliman.com/PRM-Production/qrm-documentation).

## Usage

#### Client Setup
Users should open a pull request creating a folder for the client and adding the appropriate documentation using the `client_setup` checklist. Only a Principal should review/merge the client setup pull requests.

#### Project Setup
Users should create an issue for each new project using the `project_setup` template. After completing the checklist this should be reviewed/merged by a Principal with the attestation from the `project_risk_level` template.

## Changes to templates/checklists

Anyone is welcome to suggest changes to the templates/checklists via pull requests. However, only a Principal should review/merge the pull requests.

# QRM Cross-Links

To fully comply with the Milliman QRM Standards, we capture different aspects of QRM Documentation in different locations.

| QRM Item | Location |
| :------- | :------- |
| PRM QRM Policy | [This file in the PRM/PRM-HQ Repository](https://indy-github.milliman.com/PRM/PRM-HQ/blob/master/10_policies/PRM_Analytics_QRM_Policy.md) |
| PRM Procedures for Peer Review of Product Components | [This file in the PRM/PRM-HQ Repository](https://indy-github.milliman.com/PRM/PRM-HQ/blob/master/12_procedures/Peer_Review_Product_Components.md) |
| Location of Peer Reviews for all Pipeline Components | Contained in the current version of `S:\PRM\Pipeline_Components_Env\Pipeline_Components_Env.bat` |
| Client-Level QRM Documentation (e.g. Client Risk Assessment) | Files and Pull Requests in the [PRM/client-and-project-documentation repository](https://indy-github.milliman.com/PRM/client-and-project-documentation) |
| Project-level QRM Documentation (e.g. Project Risk Assessment) | Issues in the [PRM/client-and-project-documentation repository](https://indy-github.milliman.com/PRM/client-and-project-documentation) |
| Deliverable-level QRM Documentation (e.g. Pre-Release Peer Review) | Issues in the [PRM-production/qrm-documentation repository](https://indy-github.milliman.com/PRM-production/qrm-documentation) |
| Client-/Project-/Deliverable-level procedures/guidelines | In the root `readme.md`, issue and pull request templates of the corresponding repositories above. |
