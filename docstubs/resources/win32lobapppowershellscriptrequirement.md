---
title: "win32LobAppPowerShellScriptRequirement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobAppPowerShellScriptRequirement resource type


Namespace: microsoft.graph




Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|detectionType|Enumeration| Possible values are: `notConfigured`, `string`, `dateTime`, `integer`, `float`, `version`, `boolean`.|
|detectionValue|String| Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md)|
|displayName|String||
|enforceSignatureCheck|Boolean||
|operator|Enumeration| Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|runAs32Bit|Boolean||
|runAsAccount|Enumeration| Possible values are: `system`, `user`.|
|scriptContent|String||

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

