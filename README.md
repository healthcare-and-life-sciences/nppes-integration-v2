![](/images/ahlsbanner.png)

# A-HLS NPPES Integration Documentation

## Overview

The NPPES integration accelerator delivers a pre-configured, read-only, integration with NPPES using Salesforce Flow for NPI searches. These pre-built Flows are available for download into your Salesforce org free of charge.

## **Business Objective**

The objective of the Accelerator is to provide physician liaisons, and other provider support team members, to easily verify provider data with NPPES without having to leave their Provider CRM. 

## **Business Value and Benefits**

* Eliminates the need to swivel to another application outside of your Provider CRM for NPPES searches. 
* Enables a complete Physician 360 so team members can understand all of accurate the details related to the physician
* Provides the data verification necessary for the provider credentialing process.

### Primary Industry:

* Healthcare and Life Sciences

### Intended End User:

* Multiple

## Package Includes:

*Flows (2)*

* PNM_NPI_NPPES_Check
* PNM_Retrieve_NPPES_Data (sub-flow)

*Named Credential* 

* NPPES

*External Services (2)*

* getNPIwithNPPES
* NPPESexternalcred

*Permission Set*

* External_Credentials

## Configuration Requirements

### Installation Steps:

1. Install the unmanaged packag from https://login.salesforce.com/packaging/installPackage.apexp?p0=04tHu000003eGkj

### Post-Install Configuration Steps:

1. Complete External Credential Setup:
    a. Open the External Credential Permission Set
    b. Select “External Credential Principal Access" 
    c. Click Edit
    d. Select select "NPPESexternalcred - External_Credentials_aSSVgLt1685116005782" 
    e. Hit Save
    ![](./images/nppesextcredimage.png)
    ![](./images/nppespermsetimage.png)
2. Make sure the newly installed Flows are active in the org. 
3. Assign the External Credential to any user that needs to run the Flow
4. Place the PNM_NPI_NPPES_Check Flow on your Salesforce Console and/or Experience Cloud page(s). 

## Assumptions

* A customer is assuming Salesforce Lightning Experience — not Classic.
* The Accelerator uses the Lightning Design System standards and look. Customers may want to apply their own branding which can be achieved.

## Revision History
