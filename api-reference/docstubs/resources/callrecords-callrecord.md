---
title: "callRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# callRecord resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get callRecord](../api/callrecords-callrecord-get.md)|[callRecord](../resources/callrecords-callrecord.md)|Read properties and relationships of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[Update callRecord](../api/callrecords-callrecord-update.md)|[callRecord](../resources/callrecords-callrecord.md)|Update the properties of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callrecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Create sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callrecords-session.md)|Create a new sessions object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md)|
|joinWebUrl|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|modalities|modality collection|**TODO: Add Description**|
|organizer|[identitySet](../resources/callrecords-identityset.md)|**TODO: Add Description**|
|participants|[identitySet](../resources/callrecords-identityset.md) collection|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|type|callType|**TODO: Add Description**. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[session](../resources/callrecords-session.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callRecords.callRecord",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.callRecord",
  "id": "String (identifier)",
  "version": 1024,
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "joinWebUrl": "String"
}
```

