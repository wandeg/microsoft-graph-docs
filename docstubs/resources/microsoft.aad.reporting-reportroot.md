---
title: "reportRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# reportRoot resource type


Namespace: Microsoft.AAD.Reporting



## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get reportRoot](../api/microsoft.aad.reporting-reportroot-get.md)|[reportRoot](../resources/microsoft.aad.reporting-reportroot.md)|Read properties and relationships of the [reportRoot](../resources/microsoft.aad.reporting-reportroot.md) object.|
|[Update reportRoot](../api/microsoft.aad.reporting-reportroot-update.md)|[reportRoot](../resources/microsoft.aad.reporting-reportroot.md)|Update the properties of a [reportRoot](../resources/microsoft.aad.reporting-reportroot.md) object.|
|[getAzureADLicenseUsage](../api/microsoft.aad.reporting-reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/microsoft.aad.reporting-azureadlicenseusage.md) collection||
|[getAzureADUserFeatureUsage](../api/microsoft.aad.reporting-reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/microsoft.aad.reporting-azureaduserfeatureusage.md) collection||
|[getAzureADFeatureUsage](../api/microsoft.aad.reporting-reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/microsoft.aad.reporting-azureadfeatureusage.md) collection||
|[getAzureADApplicationSignInSummary](../api/microsoft.aad.reporting-reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/microsoft.aad.reporting-applicationsigninsummary.md) collection||
|[getCredentialUserRegistrationCount](../api/microsoft.aad.reporting-reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/microsoft.aad.reporting-credentialuserregistrationcount.md) collection||
|[getCredentialUsageSummary](../api/microsoft.aad.reporting-reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/microsoft.aad.reporting-credentialusagesummary.md) collection||
|[getRelyingPartyDetailedSummary](../api/microsoft.aad.reporting-reportroot-getrelyingpartydetailedsummary.md)|[relyingPartyDetailedSummary](../resources/microsoft.aad.reporting-relyingpartydetailedsummary.md) collection||
|[List applicationSignInDetailedSummary](../api/microsoft.aad.reporting-reportroot-list-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) collection|Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.|
|[Add applicationSignInDetailedSummary](../api/microsoft.aad.reporting-reportroot-post-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md)|Add applicationSignInDetailedSummary by posting to the applicationSignInDetailedSummary collection.|
|[List credentialUserRegistrationDetails](../api/microsoft.aad.reporting-reportroot-list-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) collection|Get the credentialUserRegistrationDetailses from the credentialUserRegistrationDetails navigation property.|
|[Add credentialUserRegistrationDetails](../api/microsoft.aad.reporting-reportroot-post-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md)|Add credentialUserRegistrationDetails by posting to the credentialUserRegistrationDetails collection.|
|[List userCredentialUsageDetails](../api/microsoft.aad.reporting-reportroot-list-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) collection|Get the userCredentialUsageDetailses from the userCredentialUsageDetails navigation property.|
|[Add userCredentialUsageDetails](../api/microsoft.aad.reporting-reportroot-post-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md)|Add userCredentialUsageDetails by posting to the userCredentialUsageDetails collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|applicationSignInDetailedSummary|[applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) collection||
|credentialUserRegistrationDetails|[credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) collection||
|userCredentialUsageDetails|[userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.AAD.Reporting.reportRoot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.AAD.Reporting.reportRoot"
}
```

