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


Inherits from [windowsInformationProtectionApp](../resources/windowsinformationprotectionapp.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|binaryName|String|**TODO: Add Description**|
|binaryVersionHigh|String|**TODO: Add Description**|
|binaryVersionLow|String|**TODO: Add Description**|
|denied|Boolean|**TODO: Add Description** Inherited from [windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md)|
|description|String|**TODO: Add Description** Inherited from [windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md)|
|displayName|String|**TODO: Add Description** Inherited from [windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md)|
|productName|String|**TODO: Add Description** Inherited from [windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md)|
|publisherName|String|**TODO: Add Description** Inherited from [windowsInformationProtectionApp](../resources/intune-windowsinformationprotectionapp.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "denied": "Boolean",
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```

