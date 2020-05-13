---
title: "user resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# user resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[delta](../api/user-delta.md)|[user](../resources/user.md) collection|**TODO: Add Description**|
|[assignLicense](../api/user-assignlicense.md)|[user](../resources/user.md)|**TODO: Add Description**|
|[changePassword](../api/user-changepassword.md)|None|**TODO: Add Description**|
|[revokeSignInSessions](../api/user-revokesigninsessions.md)|Boolean|**TODO: Add Description**|
|[reprocessLicenseAssignment](../api/user-reprocesslicenseassignment.md)|[user](../resources/user.md)|**TODO: Add Description**|
|[List appRoleAssignments](../api/user-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/user-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignments object.|
|[Delete appRoleAssignments](../api/user-delete-approleassignments.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignments](../api/user-update-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Get appRoleAssignments](../api/user-get-approleassignment.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List oauth2PermissionGrants](../api/user-list-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|Get the oAuth2PermissionGrant from the oauth2PermissionGrants navigation property.|
|[Add oauth2PermissionGrants](../api/user-post-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Add oauth2PermissionGrants by posting to the oauth2PermissionGrants collection.|
|[Remove oauth2PermissionGrants](../api/user-delete-oauth2permissiongrants.md)|None|Remove an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|ageGroup|String|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|consentProvidedForMinor|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|creationType|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|employeeId|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|identities|[objectIdentity](../resources/objectidentity.md) collection|**TODO: Add Description**|
|imAddresses|String collection|**TODO: Add Description**|
|isResourceAccount|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|lastPasswordChangeDateTime|DateTimeOffset|**TODO: Add Description**|
|legalAgeGroupClassification|String|**TODO: Add Description**|
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseassignmentstate.md) collection|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|onPremisesDistinguishedName|String|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description**|
|onPremisesImmutableId|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSamAccountName|String|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesUserPrincipalName|String|**TODO: Add Description**|
|otherMails|String collection|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|signInSessionsValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|streetAddress|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|createdObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|directReports|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|licenseDetails|[licenseDetails](../resources/licensedetails.md) collection|**TODO: Add Description**|
|manager|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|oauth2PermissionGrants|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|**TODO: Add Description**|
|ownedDevices|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|ownedObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|registeredDevices|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "creationType": "String",
  "department": "String",
  "displayName": "String",
  "employeeId": "String",
  "faxNumber": "String",
  "givenName": "String",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesDomainName": "String",
  "onPremisesSamAccountName": "String",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "postalCode": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "showInAddressList": "Boolean",
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

