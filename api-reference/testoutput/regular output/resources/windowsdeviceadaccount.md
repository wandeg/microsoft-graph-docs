---
title: "windowsDeviceADAccount resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# windowsDeviceADAccount resource type




Inherits from [windowsDeviceAccount](../resources/windowsDeviceAccount.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|domainName|String||
|password|String| Inherited from [windowsDeviceAccount](../resources/windowsDeviceAccount.md)|
|userName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```

