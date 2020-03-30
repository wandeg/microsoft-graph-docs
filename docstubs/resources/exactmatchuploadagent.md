---
title: "exactMatchUploadAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# exactMatchUploadAgent resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get exactMatchUploadAgent](../api/exactmatchuploadagent-get.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Read properties and relationships of the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|
|[Update exactMatchUploadAgent](../api/exactmatchuploadagent-update.md)|[exactMatchUploadAgent](../resources/exactmatchuploadagent.md)|Update the properties of a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.exactMatchUploadAgent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exactMatchUploadAgent",
  "id": "String (identifier)",
  "description": "String",
  "creationDateTime": "String (timestamp)"
}
```

