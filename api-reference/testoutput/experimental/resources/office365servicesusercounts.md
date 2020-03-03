---
title: "office365ServicesUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365ServicesUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ServicesUserCountses](../api/office365servicesusercounts-list.md)|[office365ServicesUserCounts](../resources/office365ServicesUserCounts.md) collection|List properties and relationships of the [office365ServicesUserCounts](../resources/office365servicesusercounts.md) objects.|
|[Get office365ServicesUserCounts](../api/office365servicesusercounts-get.md)|[office365ServicesUserCounts](../resources/office365ServicesUserCounts.md)|Read properties and relationships of the [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.|
|[Create office365ServicesUserCounts](../api/office365servicesusercounts-create.md)|[office365ServicesUserCounts](../resources/office365ServicesUserCounts.md)|Create a new [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.|
|[Delete office365ServicesUserCounts](../api/office365servicesusercounts-delete.md)|None|Deletes a [office365ServicesUserCounts](../resources/office365servicesusercounts.md).|
|[Update office365ServicesUserCounts](../api/office365servicesusercounts-update.md)|[office365ServicesUserCounts](../resources/office365ServicesUserCounts.md)|Update the properties of a [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exchangeActive|Int64||
|exchangeInactive|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|office365Active|Int64||
|office365Inactive|Int64||
|oneDriveActive|Int64||
|oneDriveInactive|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharePointActive|Int64||
|sharePointInactive|Int64||
|skypeForBusinessActive|Int64||
|skypeForBusinessInactive|Int64||
|teamsActive|Int64||
|teamsInactive|Int64||
|yammerActive|Int64||
|yammerInactive|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "exchangeActive": 1024,
  "exchangeInactive": 1024,
  "oneDriveActive": 1024,
  "oneDriveInactive": 1024,
  "sharePointActive": 1024,
  "sharePointInactive": 1024,
  "skypeForBusinessActive": 1024,
  "skypeForBusinessInactive": 1024,
  "yammerActive": 1024,
  "yammerInactive": 1024,
  "teamsActive": 1024,
  "teamsInactive": 1024,
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```

