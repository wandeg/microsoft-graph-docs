---
title: "homeRealmDiscoveryPolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# homeRealmDiscoveryPolicy resource type


Namespace: microsoft.graph




Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-get.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Read properties and relationships of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[Update homeRealmDiscoveryPolicy](../api/homerealmdiscoverypolicy-update.md)|[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)|Update the properties of a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.|
|[List appliesTo](../api/homerealmdiscoverypolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/homerealmdiscoverypolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definition|String collection| Inherited from [stsPolicy](../resources/stspolicy.md)|
|description|String| Inherited from [policyBase](../resources/policybase.md)|
|displayName|String| Inherited from [policyBase](../resources/policybase.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOrganizationDefault|Boolean| Inherited from [stsPolicy](../resources/stspolicy.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection| Inherited from [stsPolicy](../resources/stspolicy.md)|

## JSON representation
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

