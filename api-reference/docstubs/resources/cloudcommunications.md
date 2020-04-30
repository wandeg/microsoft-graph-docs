---
title: "cloudCommunications resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cloudCommunications resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get cloudCommunications](../api/cloudcommunications-get.md)|[cloudCommunications](../resources/cloudcommunications.md)|Read the properties and relationships of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[Update cloudCommunications](../api/cloudcommunications-update.md)|[cloudCommunications](../resources/cloudcommunications.md)|Update the properties of a [cloudCommunications](../resources/cloudcommunications.md) object.|
|[getPresencesByUserId](../api/cloudcommunications-getpresencesbyuserid.md)|[presence](../resources/presence.md) collection|**TODO: Add Description**|
|[List calls](../api/cloudcommunications-list-calls.md)|[call](../resources/call.md) collection|Get the calls from the calls navigation property.|
|[Create calls](../api/cloudcommunications-post-calls.md)|[call](../resources/call.md)|Create a new calls object.|
|[Delete calls](../api/cloudcommunications-delete-calls.md)|None|Delete a [call](../resources/call.md) object.|
|[Update calls](../api/cloudcommunications-update-calls.md)|[call](../resources/call.md)|Update the properties of a calls object.|
|[Get call](../api/call-get.md)|[call](../resources/call.md)|Read the properties and relationships of a [call](../resources/call.md) object.|
|[List callRecords](../api/cloudcommunications-list-callrecords.md)|[callRecord](../resources/callrecord.md) collection|Get the callRecords from the callRecords navigation property.|
|[Create callRecords](../api/cloudcommunications-post-callrecords.md)|[callRecord](../resources/callrecord.md)|Create a new callRecords object.|
|[Delete callRecords](../api/cloudcommunications-delete-callrecords.md)|None|Delete a [callRecord](../resources/callrecords-callrecord.md) object.|
|[Update callRecords](../api/cloudcommunications-update-callrecords.md)|[callRecord](../resources/callrecord.md)|Update the properties of a callRecords object.|
|[Get callRecord](../api/callrecords-callrecord-get.md)|[callRecord](../resources/callrecord.md)|Read the properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[List onlineMeetings](../api/cloudcommunications-list-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Create onlineMeetings](../api/cloudcommunications-post-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Create a new onlineMeetings object.|
|[Delete onlineMeetings](../api/cloudcommunications-delete-onlinemeetings.md)|None|Delete an [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Update onlineMeetings](../api/cloudcommunications-update-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Update the properties of an onlineMeetings object.|
|[Get onlineMeeting](../api/onlinemeeting-get.md)|[onlineMeeting](../resources/onlinemeeting.md)|Read the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.|

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

