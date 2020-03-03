---
title: "skypeForBusinessOrganizerActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessOrganizerActivityUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessOrganizerActivityUserCountses](../api/skypeforbusinessorganizeractivityusercounts-list.md)|[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) collection|List properties and relationships of the [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) objects.|
|[Get skypeForBusinessOrganizerActivityUserCounts](../api/skypeforbusinessorganizeractivityusercounts-get.md)|[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)|Read properties and relationships of the [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object.|
|[Create skypeForBusinessOrganizerActivityUserCounts](../api/skypeforbusinessorganizeractivityusercounts-create.md)|[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)|Create a new [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object.|
|[Delete skypeForBusinessOrganizerActivityUserCounts](../api/skypeforbusinessorganizeractivityusercounts-delete.md)|None|Deletes a [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md).|
|[Update skypeForBusinessOrganizerActivityUserCounts](../api/skypeforbusinessorganizeractivityusercounts-update.md)|[skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md)|Update the properties of a [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSharing|Int64||
|audioVideo|Int64||
|dialInOut3rdParty|Int64||
|dialInOutMicrosoft|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityUserCounts",
  "id": "String (identifier)",
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

