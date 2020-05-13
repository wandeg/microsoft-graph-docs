---
title: "activityHistoryItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# activityHistoryItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List historyItems](../api/projectrome-useractivity-list-historyitems.md)|[activityHistoryItem](../resources/projectrome-activityhistoryitem.md) collection|Get the activityHistoryItems from the historyItems navigation property.|
|[Create historyItems](../api/projectrome-useractivity-post-historyitems.md)|[activityHistoryItem](../resources/projectrome-activityhistoryitem.md)|Create a new historyItems object.|
|[Delete historyItems](../api/projectrome-useractivity-delete-historyitems.md)|None|Delete an [activityHistoryItem](../resources/projectrome-activityhistoryitem.md) object.|
|[Update historyItems](../api/projectrome-useractivity-update-historyitems.md)|[activityHistoryItem](../resources/projectrome-activityhistoryitem.md)|Update the properties of a historyItems object.|
|[Get historyItems](../api/projectrome-useractivity-get-activityhistoryitem.md)|[activityHistoryItem](../resources/projectrome-activityhistoryitem.md)|Read the properties and relationships of an [activityHistoryItem](../resources/projectrome-activityhistoryitem.md) object.|
|[List activity](../api/projectrome-activityhistoryitem-list-activity.md)|[userActivity](../resources/projectrome-useractivity.md) collection|Get the userActivities from the activity navigation property.|
|[Add activity](../api/projectrome-activityhistoryitem-post-activity.md)|[userActivity](../resources/projectrome-useractivity.md)|Add activity by posting to the activity collection.|
|[Remove activity](../api/projectrome-activityhistoryitem-delete-activity.md)|None|Remove a [userActivity](../resources/projectrome-useractivity.md) object.|

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
|activity|[userActivity](../resources/projectrome-useractivity.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "activeDurationSeconds": "Integer",
  "createdDateTime": "String (timestamp)",
  "lastActiveDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "startedDateTime": "String (timestamp)",
  "userTimezone": "String"
}
```

