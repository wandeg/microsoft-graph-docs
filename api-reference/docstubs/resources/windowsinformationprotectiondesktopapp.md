---
title: "windowsInformationProtectionDesktopApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionDesktopApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|binaryName|String|The binary name.|
|binaryVersionHigh|String|The high binary version.|
|binaryVersionLow|String|The lower binary version.|
|denied|Boolean|If true, app is denied protection or exemption. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|description|String|The app's description. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|displayName|String|App display name. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|productName|String|The product name. Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|
|publisherName|String|The publisher name Inherited from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md)|

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

