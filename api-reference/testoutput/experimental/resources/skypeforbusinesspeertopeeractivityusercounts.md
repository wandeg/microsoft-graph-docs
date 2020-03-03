---
title: "skypeForBusinessPeerToPeerActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessPeerToPeerActivityUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessPeerToPeerActivityUserCountses](../api/skypeforbusinesspeertopeeractivityusercounts-list.md)|[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) collection|List properties and relationships of the [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) objects.|
|[Get skypeForBusinessPeerToPeerActivityUserCounts](../api/skypeforbusinesspeertopeeractivityusercounts-get.md)|[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)|Read properties and relationships of the [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) object.|
|[Create skypeForBusinessPeerToPeerActivityUserCounts](../api/skypeforbusinesspeertopeeractivityusercounts-create.md)|[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)|Create a new [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) object.|
|[Delete skypeForBusinessPeerToPeerActivityUserCounts](../api/skypeforbusinesspeertopeeractivityusercounts-delete.md)|None|Deletes a [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md).|
|[Update skypeForBusinessPeerToPeerActivityUserCounts](../api/skypeforbusinesspeertopeeractivityusercounts-update.md)|[skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md)|Update the properties of a [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSharing|Int64||
|audio|Int64||
|fileTransfer|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
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
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts",
  "id": "String (identifier)",
  "im": 1024,
  "audio": 1024,
  "video": 1024,
  "appSharing": 1024,
  "fileTransfer": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

