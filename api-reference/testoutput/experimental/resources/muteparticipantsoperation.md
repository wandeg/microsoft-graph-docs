---
title: "muteParticipantsOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# muteParticipantsOperation resource type




Inherits from [commsOperation](../resources/commsOperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List muteParticipantsOperations](../api/muteparticipantsoperation-list.md)|[muteParticipantsOperation](../resources/muteParticipantsOperation.md) collection|List properties and relationships of the [muteParticipantsOperation](../resources/muteparticipantsoperation.md) objects.|
|[Get muteParticipantsOperation](../api/muteparticipantsoperation-get.md)|[muteParticipantsOperation](../resources/muteParticipantsOperation.md)|Read properties and relationships of the [muteParticipantsOperation](../resources/muteparticipantsoperation.md) object.|
|[Create muteParticipantsOperation](../api/muteparticipantsoperation-create.md)|[muteParticipantsOperation](../resources/muteParticipantsOperation.md)|Create a new [muteParticipantsOperation](../resources/muteparticipantsoperation.md) object.|
|[Delete muteParticipantsOperation](../api/muteparticipantsoperation-delete.md)|None|Deletes a [muteParticipantsOperation](../resources/muteparticipantsoperation.md).|
|[Update muteParticipantsOperation](../api/muteparticipantsoperation-update.md)|[muteParticipantsOperation](../resources/muteParticipantsOperation.md)|Update the properties of a [muteParticipantsOperation](../resources/muteparticipantsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsOperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|participants|String collection||
|resultInfo|[ResultInfo](../resources/ResultInfo.md)| Inherited from [commsOperation](../resources/commsOperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsOperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.muteParticipantsOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.muteParticipantsOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  },
  "participants": [
    "String"
  ]
}
```

