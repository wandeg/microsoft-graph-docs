---
title: "cloudCommunications resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# cloudCommunications resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get cloudCommunications](../api/cloudcommunications-get.md)|[cloudCommunications](../resources/cloudcommunications.md)|Read properties and relationships of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[Update cloudCommunications](../api/cloudcommunications-update.md)|[cloudCommunications](../resources/cloudcommunications.md)|Update the properties of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[getPresencesByUserId](../api/cloudcommunications-getpresencesbyuserid.md)|[presence](../resources/presence.md) collection|**TODO: Add Description**|
|[List calls](../api/cloudcommunications-list-calls.md)|[call](../resources/call.md) collection|Get the calls from the calls navigation property.|
|[Add calls](../api/cloudcommunications-post-calls.md)|[call](../resources/call.md)|Add calls by posting to the calls collection.|
|[List callRecords](../api/cloudcommunications-list-callrecords.md)|[callRecord](../resources/callrecord.md) collection|Get the callRecords from the callRecords navigation property.|
|[Add callRecords](../api/cloudcommunications-post-callrecords.md)|[callRecord](../resources/callrecord.md)|Add callRecords by posting to the callRecords collection.|
|[List onlineMeetings](../api/cloudcommunications-list-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Add onlineMeetings](../api/cloudcommunications-post-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Add onlineMeetings by posting to the onlineMeetings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|callRecords|[callRecord](../resources/callrecord.md) collection|**TODO: Add Description**|
|calls|[call](../resources/call.md) collection|**TODO: Add Description**|
|onlineMeetings|[onlineMeeting](../resources/onlinemeeting.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudCommunications",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudCommunications",
  "id": "String (identifier)"
}
```

