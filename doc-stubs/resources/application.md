---
title: "application resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# application resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List applications](../api/application-list.md)|[application](../resources/application.md) collection|Get a list of the [application](../resources/application.md) objects and their properties.|
|[Get application](../api/application-get.md)|[application](../resources/application.md)|Read the properties and relationships of an [application](../resources/application.md) object.|
|[Create application](../api/application-post-applications.md)|[application](../resources/application.md)|Create a new [application](../resources/application.md) object.|
|[Delete application](../api/application-delete.md)|None|Deletes an [application](../resources/application.md) object.|
|[Update application](../api/application-update.md)|[application](../resources/application.md)|Update the properties of an [application](../resources/application.md) object.|
|[addKey](../api/application-addkey.md)|[keyCredential](../resources/keycredential.md)|**TODO: Add Description**|
|[addPassword](../api/application-addpassword.md)|[passwordCredential](../resources/passwordcredential.md)|**TODO: Add Description**|
|[removeKey](../api/application-removekey.md)|None|**TODO: Add Description**|
|[removePassword](../api/application-removepassword.md)|None|**TODO: Add Description**|
|[delta](../api/application-delta.md)|[application](../resources/application.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/application-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/application-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/application-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/application-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/application-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[List extensionProperties](../api/application-list-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md) collection|Get the extensionProperties from the extensionProperties navigation property.|
|[Create extensionProperties](../api/application-post-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md)|Create a new extensionProperties object.|
|[Delete extensionProperties](../api/application-delete-extensionproperties.md)|None|Delete an [extensionProperty](../resources/extensionproperty.md) object.|
|[Update extensionProperties](../api/application-update-extensionproperties.md)|[extensionProperty](../resources/extensionproperty.md)|Update the properties of an extensionProperties object.|
|[Get extensionProperty](../api/extensionproperty-get.md)|[extensionProperty](../resources/extensionproperty.md)|Read the properties and relationships of an [extensionProperty](../resources/extensionproperty.md) object.|
|[List claimsMappingPolicies](../api/application-list-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|Get the claimsMappingPolicies from the claimsMappingPolicies navigation property.|
|[Add claimsMappingPolicies](../api/application-post-claimsmappingpolicies.md)|[claimsMappingPolicy](../resources/claimsmappingpolicy.md)|Add claimsMappingPolicies by posting to the claimsMappingPolicies collection.|
|[Remove claimsMappingPolicies](../api/application-delete-claimsmappingpolicies.md)|None|Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.|
|[List createdOnBehalfOf](../api/application-list-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the createdOnBehalfOf navigation property.|
|[Add createdOnBehalfOf](../api/application-post-createdonbehalfof.md)|[directoryObject](../resources/directoryobject.md)|Add createdOnBehalfOf by posting to the createdOnBehalfOf collection.|
|[Remove createdOnBehalfOf](../api/application-delete-createdonbehalfof.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List owners](../api/application-list-owners.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the owners navigation property.|
|[Add owners](../api/application-post-owners.md)|[directoryObject](../resources/directoryobject.md)|Add owners by posting to the owners collection.|
|[Remove owners](../api/application-delete-owners.md)|None|Remove an [directoryObject](../resources/directoryobject.md) object.|
|[List homeRealmDiscoveryPolicies](../api/application-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Add homeRealmDiscoveryPolicies](../api/application-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Add homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|
|[Remove homeRealmDiscoveryPolicies](../api/application-delete-homerealmdiscoverypolicies.md)|None|Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[List tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|Get the tokenIssuancePolicies from the tokenIssuancePolicies navigation property.|
|[Add tokenIssuancePolicies](../api/application-post-tokenissuancepolicies.md)|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)|Add tokenIssuancePolicies by posting to the tokenIssuancePolicies collection.|
|[Remove tokenIssuancePolicies](../api/application-delete-tokenissuancepolicies.md)|None|Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.|
|[List tokenLifetimePolicies](../api/application-list-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|Get the tokenLifetimePolicies from the tokenLifetimePolicies navigation property.|
|[Add tokenLifetimePolicies](../api/application-post-tokenlifetimepolicies.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Add tokenLifetimePolicies by posting to the tokenLifetimePolicies collection.|
|[Remove tokenLifetimePolicies](../api/application-delete-tokenlifetimepolicies.md)|None|Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.|
|[List connectorGroup](../api/application-list-connectorgroup.md)|[connectorGroup](../resources/connectorgroup.md) collection|Get the connectorGroups from the connectorGroup navigation property.|
|[Add connectorGroup](../api/application-post-connectorgroup.md)|[connectorGroup](../resources/connectorgroup.md)|Add connectorGroup by posting to the connectorGroup collection.|
|[Remove connectorGroup](../api/application-delete-connectorgroup.md)|None|Remove a [connectorGroup](../resources/connectorgroup.md) object.|
|[List synchronization](../api/application-list-synchronization.md)|[synchronization](../resources/synchronization.md) collection|Get the synchronizations from the synchronization navigation property.|
|[Create synchronization](../api/application-post-synchronization.md)|[synchronization](../resources/synchronization.md)|Create a new synchronization object.|
|[Delete synchronization](../api/application-delete-synchronization.md)|None|Delete a [synchronization](../resources/synchronization.md) object.|
|[Update synchronization](../api/application-update-synchronization.md)|[synchronization](../resources/synchronization.md)|Update the properties of a synchronization object.|
|[Get synchronization](../api/synchronization-get.md)|[synchronization](../resources/synchronization.md)|Read the properties and relationships of a [synchronization](../resources/synchronization.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|api|[apiApplication](../resources/apiapplication.md)|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|appRoles|[appRole](../resources/approle.md) collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|displayName|String|**TODO: Add Description**|
|groupMembershipClaims|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|identifierUris|String collection|**TODO: Add Description**|
|info|[informationalUrl](../resources/informationalurl.md)|**TODO: Add Description**|
|isDeviceOnlyAuthSupported|Boolean|**TODO: Add Description**|
|isFallbackPublicClient|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|logo|Stream|**TODO: Add Description**|
|onPremisesPublishing|[onPremisesPublishing](../resources/onpremisespublishing.md)|**TODO: Add Description**|
|optionalClaims|[optionalClaims](../resources/optionalclaims.md)|**TODO: Add Description**|
|parentalControlSettings|[parentalControlSettings](../resources/parentalcontrolsettings.md)|**TODO: Add Description**|
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md) collection|**TODO: Add Description**|
|publicClient|[publicClientApplication](../resources/publicclientapplication.md)|**TODO: Add Description**|
|publisherDomain|String|**TODO: Add Description**|
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md) collection|**TODO: Add Description**|
|signInAudience|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|tokenEncryptionKeyId|Guid|**TODO: Add Description**|
|web|[webApplication](../resources/webapplication.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|claimsMappingPolicies|[claimsMappingPolicy](../resources/claimsmappingpolicy.md) collection|**TODO: Add Description**|
|connectorGroup|[connectorGroup](../resources/connectorgroup.md)|**TODO: Add Description**|
|createdOnBehalfOf|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|extensionProperties|[extensionProperty](../resources/extensionproperty.md) collection|**TODO: Add Description**|
|homeRealmDiscoveryPolicies|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|**TODO: Add Description**|
|owners|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|synchronization|[synchronization](../resources/synchronization.md)|**TODO: Add Description**|
|tokenIssuancePolicies|[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) collection|**TODO: Add Description**|
|tokenLifetimePolicies|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.application",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
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
}
```

