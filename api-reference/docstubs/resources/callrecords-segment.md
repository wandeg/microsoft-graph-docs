---
title: "segment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# segment resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get segment](../api/callrecords-segment-get.md)|[segment](../resources/callrecords-segment.md)|Read the properties and relationships of a [segment](../resources/callrecords-segment.md) object.|
|[Update segment](../api/callrecords-segment-update.md)|[segment](../resources/callrecords-segment.md)|Update the properties of a [segment](../resources/callrecords-segment.md) object.|
|[List segments](../api/callrecords-session-list-segments.md)|[segment](../resources/callrecords-segment.md) collection|Get the segments from the segments navigation property.|
|[Create segments](../api/callrecords-session-post-segments.md)|[segment](../resources/callrecords-segment.md)|Create a new segments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md)|
|media|[media](../resources/callrecords-media.md) collection|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|

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

