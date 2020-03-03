---
title: "activityHistoryItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# activityHistoryItem resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get activityHistoryItem](../api/activityhistoryitem-get.md)|[activityHistoryItem](../resources/activityHistoryItem.md)|Read properties and relationships of the [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[Delete activityHistoryItem](../api/activityhistoryitem-delete.md)|None|Deletes a [activityHistoryItem](../resources/activityhistoryitem.md).|
|[Update activityHistoryItem](../api/activityhistoryitem-update.md)|[activityHistoryItem](../resources/activityHistoryItem.md)|Update the properties of a [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[Get userActivity](../api/useractivity-get.md)|[userActivity](../resources/userActivity.md)|Read properties and relationships of the [userActivity](../resources/useractivity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDurationSeconds|Int32||
|createdDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActiveDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|startedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|userTimezone|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activity|[userActivity](../resources/userActivity.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activityHistoryItem",
  "id": "String (identifier)",
  "status": "String",
  "activeDurationSeconds": 1024,
  "createdDateTime": "String (timestamp)",
  "lastActiveDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "userTimezone": "String"
}
```

