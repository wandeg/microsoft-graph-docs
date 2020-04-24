---
title: "win32LobAppRegistryDetection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppRegistryDetection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [win32LobAppDetection](../resources/win32lobappdetection.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|check32BitOn64System|Boolean|A value indicating whether this registry path is for checking 32-bit app on 64-bit system|
|detectionType|win32LobAppRegistryDetectionType|The registry data detection type. Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|detectionValue|String|The registry detection value|
|keyPath|String|The registry key path to detect Win32 Line of Business (LoB) app|
|operator|win32LobAppDetectionOperator|The operator for registry data detection. Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|valueName|String|The registry value name|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```

