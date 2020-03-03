---
title: "operation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# operation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List operations](../api/operation-list.md)|[operation](../resources/operation.md) collection|List properties and relationships of the [operation](../resources/operation.md) objects.|
|[Get operation](../api/operation-get.md)|[operation](../resources/operation.md)|Read properties and relationships of the [operation](../resources/operation.md) object.|
|[Create operation](../api/operation-create.md)|[operation](../resources/operation.md)|Create a new [operation](../resources/operation.md) object.|
|[Delete operation](../api/operation-delete.md)|None|Deletes a [operation](../resources/operation.md).|
|[Update operation](../api/operation-update.md)|[operation](../resources/operation.md)|Update the properties of a [operation](../resources/operation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.operation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operation",
  "id": "String (identifier)",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)"
}
```

