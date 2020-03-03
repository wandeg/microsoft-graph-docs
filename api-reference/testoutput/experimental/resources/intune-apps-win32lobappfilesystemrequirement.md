---
title: "win32LobAppFileSystemRequirement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# win32LobAppFileSystemRequirement resource type


Namespace: microsoft.graph




Inherits from [win32LobAppRequirement](../resources/win32lobapprequirement.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|check32BitOn64System|Boolean|A value indicating whether this file or folder is for checking 32-bit app on 64-bit system|
|detectionType|Enumeration|The file system detection type. Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.|
|detectionValue|String|The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|
|fileOrFolderName|String|The file or folder name to detect Win32 Line of Business (LoB) app|
|operator|Enumeration|The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md). Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.|
|path|String|The file or folder path to detect Win32 Line of Business (LoB) app|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```

