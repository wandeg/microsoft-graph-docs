---
title: "homeRealmDiscoveryPolicy resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# homeRealmDiscoveryPolicy resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [stsPolicy](../resources/stspolicy.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List homeRealmDiscoveryPolicies](../api/policyroot-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Create homeRealmDiscoveryPolicies](../api/policyroot-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Create a new homeRealmDiscoveryPolicies object.|
|[Delete homeRealmDiscoveryPolicies](../api/policyroot-delete-homerealmdiscoverypolicies.md)|None|Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[Update homeRealmDiscoveryPolicies](../api/policyroot-update-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Update the properties of a homeRealmDiscoveryPolicies object.|
|[Get homeRealmDiscoveryPolicies](../api/policyroot-get-homerealmdiscoverypolicy.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Read the properties and relationships of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[List appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Add appliesTo](../api/homerealmdiscoverypolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Add appliesTo by posting to the appliesTo collection.|
|[Remove appliesTo](../api/homerealmdiscoverypolicy-delete-appliesto.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.homeRealmDiscoveryPolicy",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": "Boolean"
}
```

