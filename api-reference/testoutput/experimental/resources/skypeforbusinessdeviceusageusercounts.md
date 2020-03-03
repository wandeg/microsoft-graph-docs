---
title: "skypeForBusinessDeviceUsageUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessDeviceUsageUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessDeviceUsageUserCountses](../api/skypeforbusinessdeviceusageusercounts-list.md)|[skypeForBusinessDeviceUsageUserCounts](../resources/skypeForBusinessDeviceUsageUserCounts.md) collection|List properties and relationships of the [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) objects.|
|[Get skypeForBusinessDeviceUsageUserCounts](../api/skypeforbusinessdeviceusageusercounts-get.md)|[skypeForBusinessDeviceUsageUserCounts](../resources/skypeForBusinessDeviceUsageUserCounts.md)|Read properties and relationships of the [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) object.|
|[Create skypeForBusinessDeviceUsageUserCounts](../api/skypeforbusinessdeviceusageusercounts-create.md)|[skypeForBusinessDeviceUsageUserCounts](../resources/skypeForBusinessDeviceUsageUserCounts.md)|Create a new [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) object.|
|[Delete skypeForBusinessDeviceUsageUserCounts](../api/skypeforbusinessdeviceusageusercounts-delete.md)|None|Deletes a [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md).|
|[Update skypeForBusinessDeviceUsageUserCounts](../api/skypeforbusinessdeviceusageusercounts-update.md)|[skypeForBusinessDeviceUsageUserCounts](../resources/skypeForBusinessDeviceUsageUserCounts.md)|Update the properties of a [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|iPad|Int32||
|iPhone|Int32||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|windows|Int32||
|windowsPhone|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

