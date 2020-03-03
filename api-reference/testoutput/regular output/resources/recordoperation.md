---
title: "recordOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# recordOperation resource type


Namespace: microsoft.graph




Inherits from [commsOperation](../resources/commsoperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List recordOperations](../api/recordoperation-list.md)|[recordOperation](../resources/recordoperation.md) collection|List properties and relationships of the [recordOperation](../resources/recordoperation.md) objects.|
|[Get recordOperation](../api/recordoperation-get.md)|[recordOperation](../resources/recordoperation.md)|Read properties and relationships of the [recordOperation](../resources/recordoperation.md) object.|
|[Create recordOperation](../api/recordoperation-create.md)|[recordOperation](../resources/recordoperation.md)|Create a new [recordOperation](../resources/recordoperation.md) object.|
|[Delete recordOperation](../api/recordoperation-delete.md)|None|Deletes a [recordOperation](../resources/recordoperation.md).|
|[Update recordOperation](../api/recordoperation-update.md)|[recordOperation](../resources/recordoperation.md)|Update the properties of a [recordOperation](../resources/recordoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|recordingAccessToken|String||
|recordingLocation|String||
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.recordOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recordOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "recordingLocation": "String",
  "recordingAccessToken": "String"
}
```

