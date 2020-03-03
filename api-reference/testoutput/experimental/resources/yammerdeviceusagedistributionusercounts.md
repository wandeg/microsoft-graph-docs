---
title: "yammerDeviceUsageDistributionUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# yammerDeviceUsageDistributionUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerDeviceUsageDistributionUserCountses](../api/yammerdeviceusagedistributionusercounts-list.md)|[yammerDeviceUsageDistributionUserCounts](../resources/yammerDeviceUsageDistributionUserCounts.md) collection|List properties and relationships of the [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) objects.|
|[Get yammerDeviceUsageDistributionUserCounts](../api/yammerdeviceusagedistributionusercounts-get.md)|[yammerDeviceUsageDistributionUserCounts](../resources/yammerDeviceUsageDistributionUserCounts.md)|Read properties and relationships of the [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) object.|
|[Create yammerDeviceUsageDistributionUserCounts](../api/yammerdeviceusagedistributionusercounts-create.md)|[yammerDeviceUsageDistributionUserCounts](../resources/yammerDeviceUsageDistributionUserCounts.md)|Create a new [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) object.|
|[Delete yammerDeviceUsageDistributionUserCounts](../api/yammerdeviceusagedistributionusercounts-delete.md)|None|Deletes a [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md).|
|[Update yammerDeviceUsageDistributionUserCounts](../api/yammerdeviceusagedistributionusercounts-update.md)|[yammerDeviceUsageDistributionUserCounts](../resources/yammerDeviceUsageDistributionUserCounts.md)|Update the properties of a [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|iPad|Int32||
|iPhone|Int32||
|other|Int32||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int32||
|windowsPhone|Int32||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerDeviceUsageDistributionUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageDistributionUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "web": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "iPhone": 1024,
  "iPad": 1024,
  "other": 1024,
  "reportPeriod": "String"
}
```

