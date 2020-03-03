---
title: "cancelMediaProcessingOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cancelMediaProcessingOperation resource type


Namespace: microsoft.graph




Inherits from [commsOperation](../resources/commsoperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List cancelMediaProcessingOperations](../api/cancelmediaprocessingoperation-list.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) collection|List properties and relationships of the [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) objects.|
|[Get cancelMediaProcessingOperation](../api/cancelmediaprocessingoperation-get.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md)|Read properties and relationships of the [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) object.|
|[Create cancelMediaProcessingOperation](../api/cancelmediaprocessingoperation-create.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md)|Create a new [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) object.|
|[Delete cancelMediaProcessingOperation](../api/cancelmediaprocessingoperation-delete.md)|None|Deletes a [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md).|
|[Update cancelMediaProcessingOperation](../api/cancelmediaprocessingoperation-update.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md)|Update the properties of a [cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[ResultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cancelMediaProcessingOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cancelMediaProcessingOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  }
}
```

