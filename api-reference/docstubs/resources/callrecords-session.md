---
title: "session resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# session resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get session](../api/callrecords-session-get.md)|[session](../resources/callrecords-session.md)|Read properties and relationships of a [session](../resources/callrecords-session.md) object.|
|[Update session](../api/callrecords-session-update.md)|[session](../resources/callrecords-session.md)|Update the properties of a [session](../resources/callrecords-session.md) object.|
|[List segments](../api/callrecords-session-list-segments.md)|[segment](../resources/callrecords-segment.md) collection|Get the segments from the segments navigation property.|
|[Create segments](../api/callrecords-session-post-segments.md)|[segment](../resources/callrecords-segment.md)|Create a new segments object.|
|[Delete segments](../api/callrecords-session-delete-segments.md)|None|Delete a segments object.|
|[Update segments](../api/callrecords-session-update-segments.md)|[segment](../resources/callrecords-segment.md)|Update the properties of a segments object.|
|[Get segment](../api/callrecords-segment-get.md)|[segment](../resources/callrecords-segment.md)|Read properties and relationships of a [segment](../resources/callrecords-segment.md) object.|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callrecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Create sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callrecords-session.md)|Create a new sessions object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|modalities|modality collection|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|segments|[segment](../resources/callrecords-segment.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callRecords.session",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.session",
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
  },
  "id": "String (identifier)"
}
```

