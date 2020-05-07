---
title: "win32LobAppRegistryRequirement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppRegistryRequirement resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|check32BitOn64System|Boolean|**TODO: Add Description**|
|detectionType|win32LobAppRegistryDetectionType|**TODO: Add Description**. Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.|
|detectionValue|String|**TODO: Add Description** Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md)|
|keyPath|String|**TODO: Add Description**|
|operator|win32LobAppDetectionOperator|**TODO: Add Description** Inherited from [win32LobAppRequirement](../resources/win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|valueName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "check32BitOn64System": "Boolean",
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```

