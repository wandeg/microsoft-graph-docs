---
title: "session resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# session resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get session](../api/callrecords-session-get.md)|[session](../resources/callRecords-session.md)|Read properties and relationships of the [session](../resources/session.md) object.|
|[Delete session](../api/callrecords-session-delete.md)|None|Deletes a [session](../resources/session.md).|
|[Update session](../api/callrecords-session-update.md)|[session](../resources/callRecords-session.md)|Update the properties of a [session](../resources/session.md) object.|
|[List segments](../api/callrecords-session-list-segments.md)|[segment](../resources/callRecords-segment.md) collection|Get the segments from the segments navigation property.|
|[Add segments](../api/callrecords-session-post-segments.md)|[segment](../resources/callRecords-segment.md)|Add segments by posting to the segments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callRecords-endpoint.md)||
|caller|[endpoint](../resources/callRecords-endpoint.md)||
|endDateTime|DateTimeOffset||
|failureInfo|[failureInfo](../resources/callRecords-failureInfo.md)||
|id|String| Inherited from [entity](../resources/callRecords-entity.md)|
|modalities|Enumeration collection||
|startDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|segments|[segment](../resources/callRecords-segment.md) collection||

## JSON Representation
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

