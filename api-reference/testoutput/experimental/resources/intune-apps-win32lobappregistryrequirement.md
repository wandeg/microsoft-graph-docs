---
title: "win32LobAppRegistryRequirement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobAppRegistryRequirement resource type


Namespace: microsoft.graph




Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|check32BitOn64System|Boolean|A value indicating whether this registry path is for checking 32-bit app on 64-bit system|
|detectionType|Enumeration|The registry data detection type. Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|detectionValue|String|The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|keyPath|String|The registry key path to detect Win32 Line of Business (LoB) app|
|operator|Enumeration|The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|valueName|String|The registry value name|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```

