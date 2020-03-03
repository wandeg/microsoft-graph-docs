---
title: "playPromptOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# playPromptOperation resource type




Inherits from [commsOperation](../resources/commsOperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List playPromptOperations](../api/playpromptoperation-list.md)|[playPromptOperation](../resources/playPromptOperation.md) collection|List properties and relationships of the [playPromptOperation](../resources/playpromptoperation.md) objects.|
|[Get playPromptOperation](../api/playpromptoperation-get.md)|[playPromptOperation](../resources/playPromptOperation.md)|Read properties and relationships of the [playPromptOperation](../resources/playpromptoperation.md) object.|
|[Create playPromptOperation](../api/playpromptoperation-create.md)|[playPromptOperation](../resources/playPromptOperation.md)|Create a new [playPromptOperation](../resources/playpromptoperation.md) object.|
|[Delete playPromptOperation](../api/playpromptoperation-delete.md)|None|Deletes a [playPromptOperation](../resources/playpromptoperation.md).|
|[Update playPromptOperation](../api/playpromptoperation-update.md)|[playPromptOperation](../resources/playPromptOperation.md)|Update the properties of a [playPromptOperation](../resources/playpromptoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsOperation.md)|
|completionReason|Enumeration|. Possible values are: `unknown`, `completedSuccessfully`, `mediaOperationCanceled`, `unknownFutureValue`.|
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
  "@odata.type": "microsoft.graph.playPromptOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.playPromptOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  },
  "completionReason": "String"
}
```

