---
title: "servicePrincipal resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# servicePrincipal resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|addIns|[addIn](../resources/addin.md) collection|**TODO: Add Description**|
|alternativeNames|String collection|**TODO: Add Description**|
|api|[apiServicePrincipal](../resources/apiserviceprincipal.md)|**TODO: Add Description**|
|appDescription|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|applicationTemplateId|String|**TODO: Add Description**|
|appOwnerOrganizationId|Guid|**TODO: Add Description**|
|appRoleAssignmentRequired|Boolean|**TODO: Add Description**|
|appRoles|[appRole](../resources/approle.md) collection|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|errorUrl|String|**TODO: Add Description**|
|hasPermissionClassifications|Boolean|**TODO: Add Description**|
|homepage|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|info|[informationalUrl](../resources/informationalurl.md)|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|loginUrl|String|**TODO: Add Description**|
|logoutUrl|String|**TODO: Add Description**|
|notes|String|**TODO: Add Description**|
|notificationEmailAddresses|String collection|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description**|
|preferredSingleSignOnMode|String|**TODO: Add Description**|
|preferredTokenSigningKeyEndDateTime|DateTimeOffset|**TODO: Add Description**|
|preferredTokenSigningKeyThumbprint|String|**TODO: Add Description**|
|publishedPermissionScopes|[permissionScope](../resources/permissionscope.md) collection|**TODO: Add Description**|
|publisherName|String|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|
|samlMetadataUrl|String|**TODO: Add Description**|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|**TODO: Add Description**|
|servicePrincipalNames|String collection|**TODO: Add Description**|
|servicePrincipalType|String|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appRoleAssignedTo|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|**TODO: Add Description**|
|createdObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|delegatedPermissionClassifications|[delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) collection|**TODO: Add Description**|
|endpoints|[endpoint](../resources/endpoint.md) collection|**TODO: Add Description**|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|**TODO: Add Description**|
|licenseDetails|[licenseDetails](../resources/licensedetails.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|oauth2PermissionGrants|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|**TODO: Add Description**|
|ownedObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|policies|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|**TODO: Add Description**|
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
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
  "api": {
    "@odata.type": "microsoft.graph.apiServicePrincipal"
  },
  "appDescription": "String",
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
  "description": "String",
  "displayName": "String",
  "errorUrl": "String",
  "hasPermissionClassifications": "Boolean",
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
  "notes": "String",
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
```

