---
title: "tokenLifetimePolicy resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# tokenLifetimePolicy resource type


Namespace: microsoft.graph




Inherits from [stsPolicy](../resources/stspolicy.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get tokenLifetimePolicy](../api/tokenlifetimepolicy-get.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Read properties and relationships of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.|
|[Update tokenLifetimePolicy](../api/tokenlifetimepolicy-update.md)|[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)|Update the properties of a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.|
|[List appliesTo](../api/tokenlifetimepolicy-list-appliesto.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the appliesTo navigation property.|
|[Create appliesTo](../api/tokenlifetimepolicy-post-appliesto.md)|[directoryObject](../resources/directoryobject.md)|Create appliesTo by posting to the appliesTo collection.|

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
  "@odata.type": "microsoft.graph.tokenLifetimePolicy",
  "baseType": "microsoft.graph.stsPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tokenLifetimePolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": [
    "String"
  ],
  "isOrganizationDefault": true
}
```

