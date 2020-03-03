---
title: "segment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# segment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get segment](../api/callrecords-segment-get.md)|[segment](../resources/callRecords-segment.md)|Read properties and relationships of the [segment](../resources/segment.md) object.|
|[Delete segment](../api/callrecords-segment-delete.md)|None|Deletes a [segment](../resources/segment.md).|
|[Update segment](../api/callrecords-segment-update.md)|[segment](../resources/callRecords-segment.md)|Update the properties of a [segment](../resources/segment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callRecords-endpoint.md)||
|caller|[endpoint](../resources/callRecords-endpoint.md)||
|endDateTime|DateTimeOffset||
|failureInfo|[failureInfo](../resources/callRecords-failureInfo.md)||
|id|String| Inherited from [entity](../resources/callRecords-entity.md)|
|media|[media](../resources/callRecords-media.md) collection||
|startDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callRecords.segment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "caller": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "callee": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "failureInfo": {
    "@odata.type": "microsoft.graph.callRecords.failureInfo"
  },
  "media": [
    {
      "@odata.type": "microsoft.graph.callRecords.media"
    }
  ]
}
```

