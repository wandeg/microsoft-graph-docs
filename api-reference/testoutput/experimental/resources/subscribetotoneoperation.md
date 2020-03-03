---
title: "subscribeToToneOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# subscribeToToneOperation resource type




Inherits from [commsOperation](../resources/commsOperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List subscribeToToneOperations](../api/subscribetotoneoperation-list.md)|[subscribeToToneOperation](../resources/subscribeToToneOperation.md) collection|List properties and relationships of the [subscribeToToneOperation](../resources/subscribetotoneoperation.md) objects.|
|[Get subscribeToToneOperation](../api/subscribetotoneoperation-get.md)|[subscribeToToneOperation](../resources/subscribeToToneOperation.md)|Read properties and relationships of the [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object.|
|[Create subscribeToToneOperation](../api/subscribetotoneoperation-create.md)|[subscribeToToneOperation](../resources/subscribeToToneOperation.md)|Create a new [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object.|
|[Delete subscribeToToneOperation](../api/subscribetotoneoperation-delete.md)|None|Deletes a [subscribeToToneOperation](../resources/subscribetotoneoperation.md).|
|[Update subscribeToToneOperation](../api/subscribetotoneoperation-update.md)|[subscribeToToneOperation](../resources/subscribeToToneOperation.md)|Update the properties of a [subscribeToToneOperation](../resources/subscribetotoneoperation.md) object.|

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
  "@odata.type": "microsoft.graph.subscribeToToneOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subscribeToToneOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.ResultInfo"
  }
}
```

