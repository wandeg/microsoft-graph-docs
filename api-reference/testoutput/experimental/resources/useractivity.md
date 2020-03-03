---
title: "userActivity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userActivity resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userActivity](../api/useractivity-get.md)|[userActivity](../resources/userActivity.md)|Read properties and relationships of the [userActivity](../resources/useractivity.md) object.|
|[Delete userActivity](../api/useractivity-delete.md)|None|Deletes a [userActivity](../resources/useractivity.md).|
|[Update userActivity](../api/useractivity-update.md)|[userActivity](../resources/userActivity.md)|Update the properties of a [userActivity](../resources/useractivity.md) object.|
|[List historyItems](../api/useractivity-list-historyitems.md)|[activityHistoryItem](../resources/activityHistoryItem.md) collection|Get the activityHistoryItems from the historyItems navigation property.|
|[Add historyItems](../api/useractivity-post-historyitems.md)|[activityHistoryItem](../resources/activityHistoryItem.md)|Add historyItems by posting to the historyItems collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activationUrl|String||
|activitySourceHost|String||
|appActivityId|String||
|appDisplayName|String||
|contentInfo|[Json](../resources/Json.md)||
|contentUrl|String||
|createdDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|fallbackUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `active`, `updated`, `deleted`, `ignored`, `unknownFutureValue`.|
|userTimezone|String||
|visualElements|[visualInfo](../resources/visualInfo.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|historyItems|[activityHistoryItem](../resources/activityHistoryItem.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userActivity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userActivity",
  "id": "String (identifier)",
  "visualElements": {
    "@odata.type": "microsoft.graph.visualInfo",
    "attribution": {
      "@odata.type": "microsoft.graph.imageInfo",
      "iconUrl": "String",
      "alternativeText": "String",
      "alternateText": "String",
      "addImageQuery": true
    },
    "backgroundColor": "String",
    "description": "String",
    "displayText": "String",
    "content": {
      "@odata.type": "microsoft.graph.Json"
    }
  },
  "activitySourceHost": "String",
  "activationUrl": "String",
  "appActivityId": "String",
  "appDisplayName": "String",
  "contentUrl": "String",
  "createdDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "fallbackUrl": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "userTimezone": "String",
  "contentInfo": {
    "@odata.type": "microsoft.graph.Json"
  },
  "status": "String"
}
```

