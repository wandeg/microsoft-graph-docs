---
title: "teamsDeviceUsageUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teamsDeviceUsageUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsDeviceUsageUserDetails](../api/teamsdeviceusageuserdetail-list.md)|[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) collection|List properties and relationships of the [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) objects.|
|[Get teamsDeviceUsageUserDetail](../api/teamsdeviceusageuserdetail-get.md)|[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)|Read properties and relationships of the [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.|
|[Create teamsDeviceUsageUserDetail](../api/teamsdeviceusageuserdetail-create.md)|[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)|Create a new [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.|
|[Delete teamsDeviceUsageUserDetail](../api/teamsdeviceusageuserdetail-delete.md)|None|Deletes a [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md).|
|[Update teamsDeviceUsageUserDetail](../api/teamsdeviceusageuserdetail-update.md)|[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)|Update the properties of a [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|usedAndroidPhone|Boolean||
|usediOS|Boolean||
|usedMac|Boolean||
|usedWeb|Boolean||
|usedWindows|Boolean||
|usedWindowsPhone|Boolean||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsDeviceUsageUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "lastActivityDate": "Date",
  "isDeleted": true,
  "deletedDate": "Date",
  "usedWeb": true,
  "usedWindowsPhone": true,
  "usediOS": true,
  "usedMac": true,
  "usedAndroidPhone": true,
  "usedWindows": true,
  "reportPeriod": "String"
}
```

