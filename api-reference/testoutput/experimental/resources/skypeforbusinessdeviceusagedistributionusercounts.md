---
title: "skypeForBusinessDeviceUsageDistributionUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessDeviceUsageDistributionUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessDeviceUsageDistributionUserCountses](../api/skypeforbusinessdeviceusagedistributionusercounts-list.md)|[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeForBusinessDeviceUsageDistributionUserCounts.md) collection|List properties and relationships of the [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) objects.|
|[Get skypeForBusinessDeviceUsageDistributionUserCounts](../api/skypeforbusinessdeviceusagedistributionusercounts-get.md)|[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeForBusinessDeviceUsageDistributionUserCounts.md)|Read properties and relationships of the [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) object.|
|[Create skypeForBusinessDeviceUsageDistributionUserCounts](../api/skypeforbusinessdeviceusagedistributionusercounts-create.md)|[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeForBusinessDeviceUsageDistributionUserCounts.md)|Create a new [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) object.|
|[Delete skypeForBusinessDeviceUsageDistributionUserCounts](../api/skypeforbusinessdeviceusagedistributionusercounts-delete.md)|None|Deletes a [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md).|
|[Update skypeForBusinessDeviceUsageDistributionUserCounts](../api/skypeforbusinessdeviceusagedistributionusercounts-update.md)|[skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeForBusinessDeviceUsageDistributionUserCounts.md)|Update the properties of a [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|iPad|Int32||
|iPhone|Int32||
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
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageDistributionUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "windows": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "reportPeriod": "String"
}
```

