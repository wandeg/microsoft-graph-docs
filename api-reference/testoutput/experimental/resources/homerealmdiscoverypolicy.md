---
title: "homeRealmDiscoveryPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# homeRealmDiscoveryPolicy resource type




Inherits from [stsPolicy](../resources/stsPolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md)|[homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md)|Read properties and relationships of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[Delete homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-delete.md)|None|Deletes a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md).|
|[Update homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md)|[homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md)|Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[List appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md)|[directoryObject](../resources/directoryObject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/homerealmdiscoverypolicy-post-appliesto.md)|[directoryObject](../resources/directoryObject.md)|Create appliesTo by posting to the appliesTo collection.|
|[List homeRealmDiscoveryPolicies](../api/serviceprincipal-list-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md) collection|Get the homeRealmDiscoveryPolicies from the homeRealmDiscoveryPolicies navigation property.|
|[Create homeRealmDiscoveryPolicies](../api/serviceprincipal-post-homerealmdiscoverypolicies.md)|[homeRealmDiscoveryPolicy](../resources/homeRealmDiscoveryPolicy.md)|Create homeRealmDiscoveryPolicies by posting to the homeRealmDiscoveryPolicies collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection| Inherited from [stsPolicy](../resources/stsPolicy.md)|
|description|String| Inherited from [policyBase](../resources/policyBase.md)|
|displayName|String| Inherited from [policyBase](../resources/policyBase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stsPolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryObject.md) collection| Inherited from [stsPolicy](../resources/stsPolicy.md)|

## JSON Representation
Here is a JSON representation of the resource.
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
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

