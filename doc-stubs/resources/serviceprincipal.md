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
|[delta](../api/serviceprincipal-delta.md)|[servicePrincipal](../resources/serviceprincipal.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/serviceprincipal-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/serviceprincipal-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/serviceprincipal-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/serviceprincipal-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/serviceprincipal-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[List appRoleAssignedTo](../api/serviceprincipal-list-approleassignedto.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignedTo navigation property.|
|[Create appRoleAssignedTo](../api/serviceprincipal-post-approleassignedto.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignedTo object.|
|[Get appRoleAssignedTo](../api/serviceprincipal-get-approleassignment.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignedTo](../api/serviceprincipal-update-approleassignedto.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignedTo object.|
|[Delete appRoleAssignedTo](../api/serviceprincipal-delete-approleassignedto.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List appRoleAssignments](../api/serviceprincipal-list-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md) collection|Get the appRoleAssignments from the appRoleAssignments navigation property.|
|[Create appRoleAssignments](../api/serviceprincipal-post-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Create a new appRoleAssignments object.|
|[Get appRoleAssignments](../api/serviceprincipal-get-approleassignment.md)|[appRoleAssignment](../resources/approleassignment.md)|Read the properties and relationships of an [appRoleAssignment](../resources/approleassignment.md) object.|
|[Update appRoleAssignments](../api/serviceprincipal-update-approleassignments.md)|[appRoleAssignment](../resources/approleassignment.md)|Update the properties of an appRoleAssignments object.|
|[Delete appRoleAssignments](../api/serviceprincipal-delete-approleassignments.md)|None|Delete an [appRoleAssignment](../resources/approleassignment.md) object.|
|[List claimsMappingPolicies](../api/serviceprincipal-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Add claimsMappingPolicies](../api/serviceprincipal-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[Remove claimsMappingPolicies](../api/serviceprincipal-delete-claimsmappingpolicies.md)|None|Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List createdObjects](../api/serviceprincipal-list-createdobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdObjects navigation property.|
|[Add createdObjects](../api/serviceprincipal-post-createdobjects.md)|[directoryObject](../resources/directoryobject.md)|Add createdObjects by posting to the createdObjects collection.|
|[Remove createdObjects](../api/serviceprincipal-delete-createdobjects.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List endpoints](../api/serviceprincipal-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Create endpoints](../api/serviceprincipal-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Create a new endpoints object.|
|[Get endpoints](../api/serviceprincipal-get-endpoint.md)|[endpoint](../resources/endpoint.md)|Read the properties and relationships of an [endpoint](../resources/endpoint.md) object.|
|[Update endpoints](../api/serviceprincipal-update-endpoints.md)|[endpoint](../resources/endpoint.md)|Update the properties of an endpoints object.|
|[Delete endpoints](../api/serviceprincipal-delete-endpoints.md)|None|Delete an [endpoint](../resources/endpoint.md) object.|
|[List homeRealmDiscoveryPolicies](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Add homeRealmDiscoveryPolicies](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[Remove homeRealmDiscoveryPolicies](../api/serviceprincipal-delete-homerealmdiscoverypolicies.md)|None|Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[List licenseDetails](../api/serviceprincipal-list-licensedetails.md)|[licenseDetails](../resources/licensedetails.md) collection|Get the licenseDetails from the licenseDetails navigation property.|
|[Create licenseDetails](../api/serviceprincipal-post-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Create a new licenseDetails object.|
|[Get licenseDetails](../api/serviceprincipal-get-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Read the properties and relationships of a [licenseDetails](../resources/licensedetails.md) object.|
|[Update licenseDetails](../api/serviceprincipal-update-licensedetails.md)|[licenseDetails](../resources/licensedetails.md)|Update the properties of a licenseDetails object.|
|[Delete licenseDetails](../api/serviceprincipal-delete-licensedetails.md)|None|Delete a [licenseDetails](../resources/licensedetails.md) object.|
|[List memberOf](../api/serviceprincipal-list-memberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the memberOf navigation property.|
|[Add memberOf](../api/serviceprincipal-post-memberof.md)|[directoryObject](../resources/directoryobject.md)|Add memberOf by posting to the memberOf collection.|
|[Remove memberOf](../api/serviceprincipal-delete-memberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List oauth2PermissionGrants](../api/serviceprincipal-list-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|Get the oAuth2PermissionGrant from the oauth2PermissionGrants navigation property.|
|[Add oauth2PermissionGrants](../api/serviceprincipal-post-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Add oauth2PermissionGrants by posting to the oauth2PermissionGrants collection.|
|[Remove oauth2PermissionGrants](../api/serviceprincipal-delete-oauth2permissiongrants.md)|None|Remove an [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|
|[List ownedObjects](../api/serviceprincipal-list-ownedobjects.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the ownedObjects navigation property.|
|[Add ownedObjects](../api/serviceprincipal-post-ownedobjects.md)|[directoryObject](../resources/directoryobject.md)|Add ownedObjects by posting to the ownedObjects collection.|
|[Remove ownedObjects](../api/serviceprincipal-delete-ownedobjects.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/serviceprincipal-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/serviceprincipal-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/serviceprincipal-delete-owners.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List tokenIssuancePolicies](../api/serviceprincipal-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Add tokenIssuancePolicies](../api/serviceprincipal-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[Remove tokenIssuancePolicies](../api/serviceprincipal-delete-tokenissuancepolicies.md)|None|Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[List tokenLifetimePolicies](../api/serviceprincipal-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/serviceprincipal-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|
|[Remove tokenLifetimePolicies](../api/serviceprincipal-delete-tokenlifetimepolicies.md)|None|Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.|
|[List transitiveMemberOf](../api/serviceprincipal-list-transitivememberof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the transitiveMemberOf navigation property.|
|[Add transitiveMemberOf](../api/serviceprincipal-post-transitivememberof.md)|[directoryObject](../resources/directoryobject.md)|Add transitiveMemberOf by posting to the transitiveMemberOf collection.|
|[Remove transitiveMemberOf](../api/serviceprincipal-delete-transitivememberof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|addIns|[addIn](../resources/addin.md) collection|**TODO: Add Description**|
|alternativeNames|String collection|**TODO: Add Description**|
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
|homepage|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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
|endpoints|[endpoint](../resources/endpoint.md) collection|**TODO: Add Description**|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|**TODO: Add Description**|
|licenseDetails|[licenseDetails](../resources/licensedetails.md) collection|**TODO: Add Description**|
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

