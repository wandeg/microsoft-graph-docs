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


Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionType|win32LobAppPowerShellScriptDetectionType|**TODO: Add Description**. Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|detectionValue|String|**TODO: Add Description** Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md)|
|displayName|String|**TODO: Add Description**|
|enforceSignatureCheck|Boolean|**TODO: Add Description**|
|operator|win32LobAppDetectionOperator|**TODO: Add Description** Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|runAs32Bit|Boolean|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|scriptContent|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "runAsAccount": "String",
  "scriptContent": "String",
  "detectionType": "String"
}
```

