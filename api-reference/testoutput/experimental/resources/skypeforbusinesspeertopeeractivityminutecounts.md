---
title: "skypeForBusinessPeerToPeerActivityMinuteCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessPeerToPeerActivityMinuteCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessPeerToPeerActivityMinuteCountses](../api/skypeforbusinesspeertopeeractivityminutecounts-list.md)|[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) collection|List properties and relationships of the [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) objects.|
|[Get skypeForBusinessPeerToPeerActivityMinuteCounts](../api/skypeforbusinesspeertopeeractivityminutecounts-get.md)|[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)|Read properties and relationships of the [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) object.|
|[Create skypeForBusinessPeerToPeerActivityMinuteCounts](../api/skypeforbusinesspeertopeeractivityminutecounts-create.md)|[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)|Create a new [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) object.|
|[Delete skypeForBusinessPeerToPeerActivityMinuteCounts](../api/skypeforbusinesspeertopeeractivityminutecounts-delete.md)|None|Deletes a [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md).|
|[Update skypeForBusinessPeerToPeerActivityMinuteCounts](../api/skypeforbusinesspeertopeeractivityminutecounts-update.md)|[skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md)|Update the properties of a [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audio|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|video|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts",
  "id": "String (identifier)",
  "audio": 1024,
  "video": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

