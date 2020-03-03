---
title: "yammerDeviceUsageUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# yammerDeviceUsageUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerDeviceUsageUserDetails](../api/yammerdeviceusageuserdetail-list.md)|[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) collection|List properties and relationships of the [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) objects.|
|[Get yammerDeviceUsageUserDetail](../api/yammerdeviceusageuserdetail-get.md)|[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)|Read properties and relationships of the [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) object.|
|[Create yammerDeviceUsageUserDetail](../api/yammerdeviceusageuserdetail-create.md)|[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)|Create a new [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) object.|
|[Delete yammerDeviceUsageUserDetail](../api/yammerdeviceusageuserdetail-delete.md)|None|Deletes a [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md).|
|[Update yammerDeviceUsageUserDetail](../api/yammerdeviceusageuserdetail-update.md)|[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)|Update the properties of a [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastActivityDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|stateChangeDate|Date||
|usedAndroidPhone|Boolean||
|usediPad|Boolean||
|usediPhone|Boolean||
|usedOthers|Boolean||
|usedWeb|Boolean||
|usedWindowsPhone|Boolean||
|userPrincipalName|String||
|userState|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerDeviceUsageUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "userState": "String",
  "stateChangeDate": "Date",
  "lastActivityDate": "Date",
  "usedWeb": true,
  "usedWindowsPhone": true,
  "usedAndroidPhone": true,
  "usediPhone": true,
  "usediPad": true,
  "usedOthers": true,
  "reportPeriod": "String"
}
```

