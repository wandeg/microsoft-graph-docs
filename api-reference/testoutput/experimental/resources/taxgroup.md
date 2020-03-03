---
title: "taxGroup resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# taxGroup resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get taxGroup](../api/taxgroup-get.md)|[taxGroup](../resources/taxGroup.md)|Read properties and relationships of the [taxGroup](../resources/taxgroup.md) object.|
|[Delete taxGroup](../api/taxgroup-delete.md)|None|Deletes a [taxGroup](../resources/taxgroup.md).|
|[Update taxGroup](../api/taxgroup-update.md)|[taxGroup](../resources/taxGroup.md)|Update the properties of a [taxGroup](../resources/taxgroup.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|taxType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.taxGroup",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.taxGroup",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "taxType": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

