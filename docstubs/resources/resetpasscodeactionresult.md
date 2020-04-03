---
title: "resetPasscodeActionResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# resetPasscodeActionResult resource type


Namespace: microsoft.graph




Inherits from [deviceActionResult](../resources/deviceactionresult.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|actionState|Enumeration| Inherited from [deviceActionResult](../resources/deviceactionresult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|lastUpdatedDateTime|DateTimeOffset| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|passcode|String||
|startDateTime|DateTimeOffset| Inherited from [deviceActionResult](../resources/deviceactionresult.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```

