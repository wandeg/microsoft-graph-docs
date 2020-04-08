---
title: "deleteUserFromSharedAppleDeviceActionResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deleteUserFromSharedAppleDeviceActionResult resource type


Namespace: microsoft.graph




Inherits from [deviceActionResult](../resources/deviceactionresult.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|actionState|Enumeration| Inherited from [deviceActionResult](../resources/deviceactionresult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|startDateTime|DateTimeOffset| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

