---
title: "muteParticipantOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# muteParticipantOperation resource type


Namespace: microsoft.graph




Inherits from [commsOperation](../resources/commsoperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List muteParticipantOperations](../api/muteparticipantoperation-list.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md) collection|List properties and relationships of the [muteParticipantOperation](../resources/muteparticipantoperation.md) objects.|
|[Get muteParticipantOperation](../api/muteparticipantoperation-get.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|Read properties and relationships of the [muteParticipantOperation](../resources/muteparticipantoperation.md) object.|
|[Create muteParticipantOperation](../api/muteparticipantoperation-create.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|Create a new [muteParticipantOperation](../resources/muteparticipantoperation.md) object.|
|[Delete muteParticipantOperation](../api/muteparticipantoperation-delete.md)|None|Deletes a [muteParticipantOperation](../resources/muteparticipantoperation.md).|
|[Update muteParticipantOperation](../api/muteparticipantoperation-update.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|Update the properties of a [muteParticipantOperation](../resources/muteparticipantoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.muteParticipantOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.muteParticipantOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  }
}
```

