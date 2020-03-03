---
title: "skypeForBusinessDeviceUsageUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessDeviceUsageUserDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessDeviceUsageUserDetails](../api/skypeforbusinessdeviceusageuserdetail-list.md)|[skypeForBusinessDeviceUsageUserDetail](../resources/skypeForBusinessDeviceUsageUserDetail.md) collection|List properties and relationships of the [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) objects.|
|[Get skypeForBusinessDeviceUsageUserDetail](../api/skypeforbusinessdeviceusageuserdetail-get.md)|[skypeForBusinessDeviceUsageUserDetail](../resources/skypeForBusinessDeviceUsageUserDetail.md)|Read properties and relationships of the [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) object.|
|[Create skypeForBusinessDeviceUsageUserDetail](../api/skypeforbusinessdeviceusageuserdetail-create.md)|[skypeForBusinessDeviceUsageUserDetail](../resources/skypeForBusinessDeviceUsageUserDetail.md)|Create a new [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) object.|
|[Delete skypeForBusinessDeviceUsageUserDetail](../api/skypeforbusinessdeviceusageuserdetail-delete.md)|None|Deletes a [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md).|
|[Update skypeForBusinessDeviceUsageUserDetail](../api/skypeforbusinessdeviceusageuserdetail-update.md)|[skypeForBusinessDeviceUsageUserDetail](../resources/skypeForBusinessDeviceUsageUserDetail.md)|Update the properties of a [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActivityDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|usedAndroidPhone|Boolean||
|usediPad|Boolean||
|usediPhone|Boolean||
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
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessDeviceUsageUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "lastActivityDate": "Date",
  "usedWindows": true,
  "usedWindowsPhone": true,
  "usedAndroidPhone": true,
  "usediPhone": true,
  "usediPad": true,
  "reportPeriod": "String"
}
```

