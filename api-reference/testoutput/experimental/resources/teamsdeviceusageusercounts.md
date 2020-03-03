---
title: "teamsDeviceUsageUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsDeviceUsageUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsDeviceUsageUserCountses](../api/teamsdeviceusageusercounts-list.md)|[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) collection|List properties and relationships of the [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) objects.|
|[Get teamsDeviceUsageUserCounts](../api/teamsdeviceusageusercounts-get.md)|[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)|Read properties and relationships of the [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object.|
|[Create teamsDeviceUsageUserCounts](../api/teamsdeviceusageusercounts-create.md)|[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)|Create a new [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object.|
|[Delete teamsDeviceUsageUserCounts](../api/teamsdeviceusageusercounts-delete.md)|None|Deletes a [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md).|
|[Update teamsDeviceUsageUserCounts](../api/teamsdeviceusageusercounts-update.md)|[teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md)|Update the properties of a [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidPhone|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|ios|Int64||
|mac|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int64||
|windows|Int64||
|windowsPhone|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "web": 1024,
  "windowsPhone": 1024,
  "androidPhone": 1024,
  "ios": 1024,
  "mac": 1024,
  "windows": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

