---
title: "updateRecordingStatusOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# updateRecordingStatusOperation resource type




Inherits from [commsOperation](../resources/commsOperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List updateRecordingStatusOperations](../api/updaterecordingstatusoperation-list.md)|[updateRecordingStatusOperation](../resources/updateRecordingStatusOperation.md) collection|List properties and relationships of the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) objects.|
|[Get updateRecordingStatusOperation](../api/updaterecordingstatusoperation-get.md)|[updateRecordingStatusOperation](../resources/updateRecordingStatusOperation.md)|Read properties and relationships of the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object.|
|[Create updateRecordingStatusOperation](../api/updaterecordingstatusoperation-create.md)|[updateRecordingStatusOperation](../resources/updateRecordingStatusOperation.md)|Create a new [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object.|
|[Delete updateRecordingStatusOperation](../api/updaterecordingstatusoperation-delete.md)|None|Deletes a [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md).|
|[Update updateRecordingStatusOperation](../api/updaterecordingstatusoperation-update.md)|[updateRecordingStatusOperation](../resources/updateRecordingStatusOperation.md)|Update the properties of a [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsOperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[ResultInfo](../resources/ResultInfo.md)| Inherited from [commsOperation](../resources/commsOperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsOperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  }
}
```

