---
title: "session resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# session resource type


Namespace: microsoft.graph.callRecords




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get session](../api/callrecords-session-get.md)|[session](../resources/callrecords-session.md)|Read properties and relationships of the [session](../resources/callrecords-session.md) object.|
|[Update session](../api/callrecords-session-update.md)|[session](../resources/callrecords-session.md)|Update the properties of a [session](../resources/callrecords-session.md) object.|
|[List segments](../api/callrecords-session-list-segments.md)|[segment](../resources/callrecords-segment.md) collection|Get the segments from the segments navigation property.|
|[Add segments](../api/callrecords-session-post-segments.md)|[segment](../resources/callrecords-segment.md)|Add segments by posting to the segments collection.|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callrecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Add sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callrecords-session.md)|Add sessions by posting to the sessions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callrecords-endpoint.md)||
|caller|[endpoint](../resources/callrecords-endpoint.md)||
|endDateTime|DateTimeOffset||
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)||
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|modalities|Enumeration collection||
|startDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|segments|[segment](../resources/callrecords-segment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.session",
  "id": "String (identifier)",
  "modalities": [
    "String"
  ],
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
  }
}
```

