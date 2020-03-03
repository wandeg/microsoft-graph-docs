---
title: "policyBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policyBase resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List policyBases](../api/policybase-list.md)|[policyBase](../resources/policybase.md) collection|List properties and relationships of the [policyBase](../resources/policybase.md) objects.|
|[Get policyBase](../api/policybase-get.md)|[policyBase](../resources/policybase.md)|Read properties and relationships of the [policyBase](../resources/policybase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policyBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policyBase",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

