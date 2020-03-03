---
title: "segment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# segment resource type


Namespace: microsoft.graph.callRecords




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List segments](../api/callrecords-segment-list.md)|[segment](../resources/callrecords-segment.md) collection|List properties and relationships of the [segment](../resources/segment.md) objects.|
|[Get segment](../api/callrecords-segment-get.md)|[segment](../resources/callrecords-segment.md)|Read properties and relationships of the [segment](../resources/callrecords-segment.md) object.|
|[Create segment](../api/callrecords-segment-create.md)|[segment](../resources/callrecords-segment.md)|Create a new [segment](../resources/callrecords-segment.md) object.|
|[Delete segment](../api/callrecords-segment-delete.md)|None|Deletes a [segment](../resources/callrecords-segment.md).|
|[Update segment](../api/callrecords-segment-update.md)|[segment](../resources/callrecords-segment.md)|Update the properties of a [segment](../resources/callrecords-segment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callrecords-endpoint.md)||
|caller|[endpoint](../resources/callrecords-endpoint.md)||
|endDateTime|DateTimeOffset||
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)||
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|media|[media](../resources/callrecords-media.md) collection||
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

