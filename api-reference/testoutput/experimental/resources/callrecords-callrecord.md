---
title: "callRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# callRecord resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get callRecord](../api/callrecords-callrecord-get.md)|[callRecord](../resources/callRecords-callRecord.md)|Read properties and relationships of the [callRecord](../resources/callrecord.md) object.|
|[Delete callRecord](../api/callrecords-callrecord-delete.md)|None|Deletes a [callRecord](../resources/callrecord.md).|
|[Update callRecord](../api/callrecords-callrecord-update.md)|[callRecord](../resources/callRecords-callRecord.md)|Update the properties of a [callRecord](../resources/callrecord.md) object.|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callRecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Add sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callRecords-session.md)|Add sessions by posting to the sessions collection.|
|[List callRecords](../api/cloudcommunications-list-callrecords.md)|[callRecord](../resources/callRecords-callRecord.md) collection|Get the callRecords from the callRecords navigation property.|
|[Add callRecords](../api/cloudcommunications-post-callrecords.md)|[callRecord](../resources/callRecords-callRecord.md)|Add callRecords by posting to the callRecords collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/callRecords-entity.md)|
|joinWebUrl|String||
|lastModifiedDateTime|DateTimeOffset||
|modalities|Enumeration collection||
|organizer|[identitySet](../resources/callRecords-identitySet.md)||
|participants|[identitySet](../resources/callRecords-identitySet.md) collection||
|startDateTime|DateTimeOffset||
|type|Enumeration|. Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[session](../resources/callRecords-session.md) collection||

## JSON Representation
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

