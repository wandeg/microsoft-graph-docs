---
title: "skypeForBusinessOrganizerActivityMinuteCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessOrganizerActivityMinuteCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessOrganizerActivityMinuteCountses](../api/skypeforbusinessorganizeractivityminutecounts-list.md)|[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) collection|List properties and relationships of the [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) objects.|
|[Get skypeForBusinessOrganizerActivityMinuteCounts](../api/skypeforbusinessorganizeractivityminutecounts-get.md)|[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)|Read properties and relationships of the [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) object.|
|[Create skypeForBusinessOrganizerActivityMinuteCounts](../api/skypeforbusinessorganizeractivityminutecounts-create.md)|[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)|Create a new [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) object.|
|[Delete skypeForBusinessOrganizerActivityMinuteCounts](../api/skypeforbusinessorganizeractivityminutecounts-delete.md)|None|Deletes a [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md).|
|[Update skypeForBusinessOrganizerActivityMinuteCounts](../api/skypeforbusinessorganizeractivityminutecounts-update.md)|[skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md)|Update the properties of a [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audioVideo|Int64||
|dialInMicrosoft|Int64||
|dialOutMicrosoft|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityMinuteCounts",
  "id": "String (identifier)",
  "audioVideo": 1024,
  "dialInMicrosoft": 1024,
  "dialOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

