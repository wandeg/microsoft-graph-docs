---
title: "applicationServicePrincipal resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applicationServicePrincipal resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|application|[application](../resources/application.md)|**TODO: Add Description**|
|servicePrincipal|[servicePrincipal](../resources/serviceprincipal.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationServicePrincipal",
  "application": {
    "@odata.type": "#microsoft.graph.application",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)",
    "api": {
      "@odata.type": "microsoft.graph.apiApplication"
    },
    "appId": "String",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole"
      }
    ],
    "createdDateTime": "String (timestamp)",
    "isFallbackPublicClient": "Boolean",
    "identifierUris": [
      "String"
    ],
    "displayName": "String",
    "groupMembershipClaims": "String",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl"
    },
    "isDeviceOnlyAuthSupported": "Boolean",
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential"
      }
    ],
    "logo": "Stream",
    "optionalClaims": {
      "@odata.type": "microsoft.graph.optionalClaims"
    },
    "parentalControlSettings": {
      "@odata.type": "microsoft.graph.parentalControlSettings"
    },
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential"
      }
    ],
    "publicClient": {
      "@odata.type": "microsoft.graph.publicClientApplication"
    },
    "publisherDomain": "String",
    "requiredResourceAccess": [
      {
        "@odata.type": "microsoft.graph.requiredResourceAccess"
      }
    ],
    "signInAudience": "String",
    "tags": [
      "String"
    ],
    "tokenEncryptionKeyId": "Guid",
    "web": {
      "@odata.type": "microsoft.graph.webApplication"
    },
    "onPremisesPublishing": {
      "@odata.type": "microsoft.graph.onPremisesPublishing"
    }
  },
  "servicePrincipal": {
    "@odata.type": "#microsoft.graph.servicePrincipal",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)",
    "accountEnabled": "Boolean",
    "addIns": [
      {
        "@odata.type": "microsoft.graph.addIn"
      }
    ],
    "alternativeNames": [
      "String"
    ],
    "appDisplayName": "String",
    "appId": "String",
    "applicationTemplateId": "String",
    "appOwnerOrganizationId": "Guid",
    "appRoleAssignmentRequired": "Boolean",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole"
      }
    ],
    "displayName": "String",
    "errorUrl": "String",
    "homepage": "String",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl"
    },
    "keyCredentials": [
      {
        "@odata.type": "microsoft.graph.keyCredential"
      }
    ],
    "loginUrl": "String",
    "logoutUrl": "String",
    "notificationEmailAddresses": [
      "String"
    ],
    "publishedPermissionScopes": [
      {
        "@odata.type": "microsoft.graph.permissionScope"
      }
    ],
    "passwordCredentials": [
      {
        "@odata.type": "microsoft.graph.passwordCredential"
      }
    ],
    "preferredTokenSigningKeyEndDateTime": "String (timestamp)",
    "preferredTokenSigningKeyThumbprint": "String",
    "preferredSingleSignOnMode": "String",
    "publisherName": "String",
    "replyUrls": [
      "String"
    ],
    "samlMetadataUrl": "String",
    "samlSingleSignOnSettings": {
      "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
    },
    "servicePrincipalNames": [
      "String"
    ],
    "servicePrincipalType": "String",
    "signInAudience": "String",
    "tags": [
      "String"
    ],
    "tokenEncryptionKeyId": "Guid"
  }
}
```

