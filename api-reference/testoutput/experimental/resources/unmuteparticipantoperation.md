---
title: "unmuteParticipantOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unmuteParticipantOperation resource type


Namespace: microsoft.graph




Inherits from [commsOperation](../resources/commsoperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List unmuteParticipantOperations](../api/unmuteparticipantoperation-list.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) collection|List properties and relationships of the [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) objects.|
|[Get unmuteParticipantOperation](../api/unmuteparticipantoperation-get.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)|Read properties and relationships of the [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object.|
|[Create unmuteParticipantOperation](../api/unmuteparticipantoperation-create.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)|Create a new [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object.|
|[Delete unmuteParticipantOperation](../api/unmuteparticipantoperation-delete.md)|None|Deletes a [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md).|
|[Update unmuteParticipantOperation](../api/unmuteparticipantoperation-update.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)|Update the properties of a [unmuteParticipantOperation](../resources/unmuteparticipantoperation.md) object.|

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
  "@odata.type": "microsoft.graph.unmuteParticipantOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unmuteParticipantOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  }
}
```

