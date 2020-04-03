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
|check32BitOn64System|Boolean||
|detectionType|Enumeration| Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|detectionValue|String| Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md)|
|keyPath|String||
|operator|Enumeration| Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|valueName|String||

## Relationships
None

## JSON representation
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

