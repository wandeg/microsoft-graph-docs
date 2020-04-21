---
title: "activityHistoryItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# activityHistoryItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get activityHistoryItem](../api/activityhistoryitem-get.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Read properties and relationships of an [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[Update activityHistoryItem](../api/activityhistoryitem-update.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Update the properties of a [activityHistoryItem](../resources/activityhistoryitem.md) object.|
|[List activity](../api/activityhistoryitem-list-activity.md)|[userActivity](../resources/useractivity.md) collection|Get the userActivities from the activity navigation property.|
|[Add activity](../api/activityhistoryitem-post-activity.md)|[userActivity](../resources/useractivity.md)|Add activity by posting to the activity collection.|
|[Remove activity](../api/activityhistoryitem-delete-activity.md)|None|Remove an activity object.|
|[List historyItems](../api/useractivity-list-historyitems.md)|[activityHistoryItem](../resources/activityhistoryitem.md) collection|Get the activityHistoryItems from the historyItems navigation property.|
|[Create historyItems](../api/useractivity-post-historyitems.md)|[activityHistoryItem](../resources/activityhistoryitem.md)|Create a new historyItems object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeDurationSeconds|Int32|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastActiveDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|startedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|status|**TODO: Add Description**. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|userTimezone|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activity|[userActivity](../resources/useractivity.md)|**TODO: Add Description**|

## JSON representation
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

