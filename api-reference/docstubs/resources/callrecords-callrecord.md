---
title: "callRecord resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# callRecord resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List sessions](../api/callrecords-callrecord-list-sessions.md)|[session](../resources/callrecords-session.md) collection|Get the sessions from the sessions navigation property.|
|[Create sessions](../api/callrecords-callrecord-post-sessions.md)|[session](../resources/callrecords-session.md)|Create a new sessions object.|
|[Delete sessions](../api/callrecords-callrecord-delete-sessions.md)|None|Delete a [session](../resources/callrecords-session.md) object.|
|[Update sessions](../api/callrecords-callrecord-update-sessions.md)|[session](../resources/callrecords-session.md)|Update the properties of a sessions object.|
|[Get session](../api/callrecords-session-get.md)|[session](../resources/callrecords-session.md)|Read the properties and relationships of a [session](../resources/callrecords-session.md) object.|

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
  "version": "Integer",
  "type": "String",
  "modalities": [
    "String"
  ],
  "lastModifiedDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "organizer": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ],
  "joinWebUrl": "String"
}
```

