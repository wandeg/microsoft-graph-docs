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

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List servicePrincipals](../api/serviceprincipal-list.md)|[servicePrincipal](../resources/serviceprincipal.md) collection|Get a list of the [servicePrincipal](../resources/serviceprincipal.md) objects and their properties.|
|[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md)|[servicePrincipal](../resources/serviceprincipal.md)|Create a new [servicePrincipal](../resources/serviceprincipal.md) object.|
|[Get servicePrincipal](../api/serviceprincipal-get.md)|[servicePrincipal](../resources/serviceprincipal.md)|Read the properties and relationships of a [servicePrincipal](../resources/serviceprincipal.md) object.|
|[Update servicePrincipal](../api/serviceprincipal-update.md)|[servicePrincipal](../resources/serviceprincipal.md)|Update the properties of a [servicePrincipal](../resources/serviceprincipal.md) object.|
|[Delete servicePrincipal](../api/serviceprincipal-delete.md)|None|Deletes a [servicePrincipal](../resources/serviceprincipal.md) object.|
|[List activityBasedTimeoutPolicies](../api/serviceprincipal-list-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection|Get the activityBasedTimeoutPolicies from the activityBasedTimeoutPolicies navigation property.|
|[Add activityBasedTimeoutPolicies](../api/serviceprincipal-post-activitybasedtimeoutpolicies.md)|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)|Add activityBasedTimeoutPolicies by posting to the activityBasedTimeoutPolicies collection.|
|[Remove activityBasedTimeoutPolicies](../api/serviceprincipal-delete-activitybasedtimeoutpolicies.md)|None|Remove an [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.|
|[List claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Add claimsMappingPolicies](../api/serviceprincipal-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[Remove claimsMappingPolicies](../api/serviceprincipal-delete-claimsmappingpolicies.md)|None|Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List tokenIssuancePolicies](../api/serviceprincipal-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Add tokenIssuancePolicies](../api/serviceprincipal-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[Remove tokenIssuancePolicies](../api/serviceprincipal-delete-tokenissuancepolicies.md)|None|Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[List tokenLifetimePolicies](../api/serviceprincipal-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/serviceprincipal-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|
|[Remove tokenLifetimePolicies](../api/serviceprincipal-delete-tokenlifetimepolicies.md)|None|Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|addIns|[addIn](../resources/addin.md) collection|**TODO: Add Description**|
|alternativeNames|String collection|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|applicationTemplateId|String|**TODO: Add Description**|
|appOwnerOrganizationId|Guid|**TODO: Add Description**|
|appRoleAssignmentRequired|Boolean|**TODO: Add Description**|
|appRoles|[appRole](../resources/approle.md) collection|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|homepage|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|info|[informationalUrl](../resources/informationalurl.md)|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|loginUrl|String|**TODO: Add Description**|
|logoutUrl|String|**TODO: Add Description**|
|notificationEmailAddresses|String collection|**TODO: Add Description**|
|oauth2PermissionScopes|[permissionScope](../resources/permissionscope.md) collection|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description**|
|preferredSingleSignOnMode|String|**TODO: Add Description**|
|replyUrls|String collection|**TODO: Add Description**|
|samlSingleSignOnSettings|[samlSingleSignOnSettings](../resources/samlsinglesignonsettings.md)|**TODO: Add Description**|
|servicePrincipalNames|String collection|**TODO: Add Description**|
|servicePrincipalType|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activityBasedTimeoutPolicies|[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) collection|**TODO: Add Description**|
|appRoleAssignedTo|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|appRoleAssignments|[appRoleAssignment](../resources/approleassignment.md) collection|**TODO: Add Description**|
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|**TODO: Add Description**|
|createdObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|endpoints|[endpoint](../resources/endpoint.md) collection|**TODO: Add Description**|
|memberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|oauth2PermissionGrants|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|**TODO: Add Description**|
|ownedObjects|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|**TODO: Add Description**|
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|**TODO: Add Description**|
|transitiveMemberOf|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.servicePrincipal",
  "baseType": "microsoft.graph.directoryObject",
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
  "oauth2PermissionScopes": [
    {
      "@odata.type": "microsoft.graph.permissionScope"
    }
  ],
  "passwordCredentials": [
    {
      "@odata.type": "microsoft.graph.passwordCredential"
    }
  ],
  "preferredSingleSignOnMode": "String",
  "replyUrls": [
    "String"
  ],
  "servicePrincipalNames": [
    "String"
  ],
  "samlSingleSignOnSettings": {
    "@odata.type": "microsoft.graph.samlSingleSignOnSettings"
  },
  "servicePrincipalType": "String",
  "tags": [
    "String"
  ],
  "tokenEncryptionKeyId": "Guid"
}
```

