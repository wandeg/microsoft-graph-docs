---
title: "callRecord resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# callRecord resource type


Namespace: microsoft.graph.callRecords




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get callRecord](../api/callrecords-callrecord-get.md)|[callRecord](../resources/callrecords-callrecord.md)|Read properties and relationships of the [callRecord](../resources/callrecords-callrecord.md) object.|
|[Update callRecord](../api/callrecords-callrecord-update.md)|[callRecord](../resources/callrecords-callrecord.md)|Update the properties of a [callRecord](../resources/callrecords-callrecord.md) object.|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callrecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Add sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callrecords-session.md)|Add sessions by posting to the sessions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|joinWebUrl|String||
|lastModifiedDateTime|DateTimeOffset||
|modalities|Enumeration collection||
|organizer|[identitySet](../resources/callrecords-identityset.md)||
|participants|[identitySet](../resources/callrecords-identityset.md) collection||
|startDateTime|DateTimeOffset||
|type|Enumeration| Possible values are: `unknown`, `groupCall`, `peerToPeer`, `unknownFutureValue`.|
|version|Int64||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sessions|[session](../resources/callrecords-session.md) collection||

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

