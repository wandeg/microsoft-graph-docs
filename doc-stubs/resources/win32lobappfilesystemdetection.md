---
title: "win32LobAppFileSystemDetection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobAppFileSystemDetection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [win32LobAppDetection](../resources/win32lobappdetection.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|check32BitOn64System|Boolean|**TODO: Add Description**|
|detectionType|win32LobAppFileSystemDetectionType|**TODO: Add Description**. Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|
|detectionValue|String|**TODO: Add Description**|
|fileOrFolderName|String|**TODO: Add Description**|
|operator|win32LobAppDetectionOperator|**TODO: Add Description**. Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|path|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": "Boolean",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```

