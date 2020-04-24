---
title: "win32LobAppPowerShellScriptRequirement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppPowerShellScriptRequirement resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionType|win32LobAppPowerShellScriptDetectionType|The detection type for script output. Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|detectionValue|String|The detection value Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md)|
|displayName|String|The unique display name for this rule|
|enforceSignatureCheck|Boolean|A value indicating whether signature check is enforced|
|operator|win32LobAppDetectionOperator|The operator for detection Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|runAs32Bit|Boolean|A value indicating whether this script should run as 32-bit|
|runAsAccount|runAsAccountType|Indicates the type of execution context the script runs in. Possible values are: `system`, `user`.|
|scriptContent|String|The base64 encoded script content to detect Win32 Line of Business (LoB) app|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppPowerShellScriptRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppPowerShellScriptRequirement",
  "operator": "String",
  "detectionValue": "String",
  "displayName": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```

