---
title: "commsOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# commsOperation resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get commsOperation](../api/commsoperation-get.md)|[commsOperation](../resources/commsOperation.md)|Read properties and relationships of the [commsOperation](../resources/commsoperation.md) object.|
|[Delete commsOperation](../api/commsoperation-delete.md)|None|Deletes a [commsOperation](../resources/commsoperation.md).|
|[Update commsOperation](../api/commsoperation-update.md)|[commsOperation](../resources/commsOperation.md)|Update the properties of a [commsOperation](../resources/commsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[ResultInfo](../resources/ResultInfo.md)||
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

