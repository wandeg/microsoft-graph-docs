---
title: "exactMatchJobBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# exactMatchJobBase resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List exactMatchJobBases](../api/exactmatchjobbase-list.md)|[exactMatchJobBase](../resources/exactMatchJobBase.md) collection|List properties and relationships of the [exactMatchJobBase](../resources/exactmatchjobbase.md) objects.|
|[Get exactMatchJobBase](../api/exactmatchjobbase-get.md)|[exactMatchJobBase](../resources/exactMatchJobBase.md)|Read properties and relationships of the [exactMatchJobBase](../resources/exactmatchjobbase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completionDateTime|DateTimeOffset||
|creationDateTime|DateTimeOffset||
|error|[classificationError](../resources/classificationError.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchJobBase",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchJobBase",
  "id": "String (identifier)",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "completionDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  }
}
```

