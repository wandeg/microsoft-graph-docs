---
title: "reportRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# reportRoot resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get reportRoot](../api/reportroot-get.md)|[reportRoot](../resources/reportroot.md)|Read the properties and relationships of a [reportRoot](../resources/reportroot.md) object.|
|[Update reportRoot](../api/reportroot-update.md)|[reportRoot](../resources/reportroot.md)|Update the properties of a [reportRoot](../resources/reportroot.md) object.|
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add Description**|
|[getRelyingPartyDetailedSummary](../api/reportroot-getrelyingpartydetailedsummary.md)|[relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) collection|**TODO: Add Description**|
|[List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|Get the applicationSignInDetailedSummaries from the applicationSignInDetailedSummary navigation property.|
|[Create applicationSignInDetailedSummary](../api/reportroot-post-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Create a new applicationSignInDetailedSummary object.|
|[Delete applicationSignInDetailedSummary](../api/reportroot-delete-applicationsignindetailedsummary.md)|None|Delete an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[Update applicationSignInDetailedSummary](../api/reportroot-update-applicationsignindetailedsummary.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Update the properties of an applicationSignInDetailedSummary object.|
|[Get applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md)|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Read the properties and relationships of an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object.|
|[List credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) collection|Get the credentialUserRegistrationDetails from the credentialUserRegistrationDetails navigation property.|
|[Create credentialUserRegistrationDetails](../api/reportroot-post-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Create a new credentialUserRegistrationDetails object.|
|[Delete credentialUserRegistrationDetails](../api/reportroot-delete-credentialuserregistrationdetails.md)|None|Delete a [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.|
|[Update credentialUserRegistrationDetails](../api/reportroot-update-credentialuserregistrationdetails.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Update the properties of a credentialUserRegistrationDetails object.|
|[Get credentialUserRegistrationDetails](../api/credentialuserregistrationdetails-get.md)|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Read the properties and relationships of a [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.|
|[List userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) collection|Get the userCredentialUsageDetails from the userCredentialUsageDetails navigation property.|
|[Create userCredentialUsageDetails](../api/reportroot-post-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Create a new userCredentialUsageDetails object.|
|[Delete userCredentialUsageDetails](../api/reportroot-delete-usercredentialusagedetails.md)|None|Delete a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|
|[Update userCredentialUsageDetails](../api/reportroot-update-usercredentialusagedetails.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Update the properties of a userCredentialUsageDetails object.|
|[Get userCredentialUsageDetails](../api/usercredentialusagedetails-get.md)|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Read the properties and relationships of a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|applicationSignInDetailedSummary|[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) collection|**TODO: Add Description**|
|credentialUserRegistrationDetails|[credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) collection|**TODO: Add Description**|
|userCredentialUsageDetails|[userCredentialUsageDetails](../resources/usercredentialusagedetails.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```

