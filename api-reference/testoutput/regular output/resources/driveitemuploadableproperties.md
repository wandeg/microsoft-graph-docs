---
title: "driveItemUploadableProperties resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# driveItemUploadableProperties resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|fileSystemInfo|[fileSystemInfo](../resources/fileSystemInfo.md)||
|name|String||

## Relationships
None

## JSON Representation
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

