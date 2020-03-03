---
title: "commsOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# commsOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List commsOperations](../api/commsoperation-list.md)|[commsOperation](../resources/commsoperation.md) collection|List properties and relationships of the [commsOperation](../resources/commsoperation.md) objects.|
|[Get commsOperation](../api/commsoperation-get.md)|[commsOperation](../resources/commsoperation.md)|Read properties and relationships of the [commsOperation](../resources/commsoperation.md) object.|
|[Create commsOperation](../api/commsoperation-create.md)|[commsOperation](../resources/commsoperation.md)|Create a new [commsOperation](../resources/commsoperation.md) object.|
|[Delete commsOperation](../api/commsoperation-delete.md)|None|Deletes a [commsOperation](../resources/commsoperation.md).|
|[Update commsOperation](../api/commsoperation-update.md)|[commsOperation](../resources/commsoperation.md)|Update the properties of a [commsOperation](../resources/commsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[ResultInfo](../resources/resultinfo.md)||
|status|Enumeration|. Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.commsOperation",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.commsOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  }
}
```

