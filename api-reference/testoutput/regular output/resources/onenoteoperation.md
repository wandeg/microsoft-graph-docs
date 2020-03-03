---
title: "onenoteOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenoteOperation resource type




Inherits from [operation](../resources/operation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteOperation](../api/onenoteoperation-get.md)|[onenoteOperation](../resources/onenoteOperation.md)|Read properties and relationships of the [onenoteOperation](../resources/onenoteoperation.md) object.|
|[Delete onenoteOperation](../api/onenoteoperation-delete.md)|None|Deletes a [onenoteOperation](../resources/onenoteoperation.md).|
|[Update onenoteOperation](../api/onenoteoperation-update.md)|[onenoteOperation](../resources/onenoteOperation.md)|Update the properties of a [onenoteOperation](../resources/onenoteoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|error|[onenoteOperationError](../resources/onenoteOperationError.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset| Inherited from [operation](../resources/operation.md)|
|percentComplete|String||
|resourceId|String||
|resourceLocation|String||
|status|Enumeration| Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteOperation",
  "baseType": "microsoft.graph.operation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "String (identifier)",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "resourceId": "String",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError"
  },
  "percentComplete": "String"
}
```

