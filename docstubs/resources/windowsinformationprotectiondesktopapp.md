---
title: "windowsInformationProtectionDesktopApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# windowsInformationProtectionDesktopApp resource type


Namespace: microsoft.graph




Inherits from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|binaryName|String||
|binaryVersionHigh|String||
|binaryVersionLow|String||
|denied|Boolean| Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|description|String| Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|displayName|String| Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|productName|String| Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|publisherName|String| Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```

