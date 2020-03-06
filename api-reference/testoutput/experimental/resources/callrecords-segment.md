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
|[Get segment](../api/callrecords-segment-get.md)|[segment](../resources/callrecords-segment.md)|Read properties and relationships of the [segment](../resources/callrecords-segment.md) object.|
|[Update segment](../api/callrecords-segment-update.md)|[segment](../resources/callrecords-segment.md)|Update the properties of a [segment](../resources/callrecords-segment.md) object.|
|[List segments](../api/callrecords-session-list-segments.md)|[segment](../resources/callrecords-segment.md) collection|Get the segments from the segments navigation property.|
|[Add segments](../api/callrecords-session-post-segments.md)|[segment](../resources/callrecords-segment.md)|Add segments by posting to the segments collection.|

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

## JSON representation
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

