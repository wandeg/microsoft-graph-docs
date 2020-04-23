---
title: "driveItemUploadableProperties resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# driveItemUploadableProperties resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|fileSystemInfo|[fileSystemInfo](../resources/filesysteminfo.md)|**TODO: Add Description**|
|name|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.driveItemUploadableProperties"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItemUploadableProperties",
  "description": "String",
  "fileSystemInfo": {
    "@odata.type": "microsoft.graph.fileSystemInfo",
    "createdDateTime": "String (timestamp)",
    "lastAccessedDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)"
  },
  "name": "String"
}
```

