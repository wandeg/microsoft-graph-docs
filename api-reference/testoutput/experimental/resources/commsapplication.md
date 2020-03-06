---
title: "commsApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# commsApplication resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get commsApplication](../api/commsapplication-get.md)|[commsApplication](../resources/commsapplication.md)|Read properties and relationships of the [commsApplication](../resources/commsapplication.md) object.|
|[Update commsApplication](../api/commsapplication-update.md)|[commsApplication](../resources/commsapplication.md)|Update the properties of a [commsApplication](../resources/commsapplication.md) object.|
|[List calls](../api/commsapplication-list-calls.md)|[call](../resources/call.md) collection|Get the calls from the calls navigation property.|
|[Add calls](../api/commsapplication-post-calls.md)|[call](../resources/call.md)|Add calls by posting to the calls collection.|
|[List onlineMeetings](../api/commsapplication-list-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Add onlineMeetings](../api/commsapplication-post-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Add onlineMeetings by posting to the onlineMeetings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|calls|[call](../resources/call.md) collection||
|onlineMeetings|[onlineMeeting](../resources/onlinemeeting.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.commsApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.commsApplication",
  "id": "String (identifier)"
}
```

