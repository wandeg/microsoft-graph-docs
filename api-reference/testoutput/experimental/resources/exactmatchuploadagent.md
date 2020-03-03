---
title: "exactMatchUploadAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# exactMatchUploadAgent resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get exactMatchUploadAgent](../api/exactmatchuploadagent-get.md)|[exactMatchUploadAgent](../resources/exactMatchUploadAgent.md)|Read properties and relationships of the [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|
|[Delete exactMatchUploadAgent](../api/exactmatchuploadagent-delete.md)|None|Deletes a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md).|
|[Update exactMatchUploadAgent](../api/exactmatchuploadagent-update.md)|[exactMatchUploadAgent](../resources/exactMatchUploadAgent.md)|Update the properties of a [exactMatchUploadAgent](../resources/exactmatchuploadagent.md) object.|
|[List exactMatchUploadAgents](../api/dataclassificationservice-list-exactmatchuploadagents.md)|[exactMatchUploadAgent](../resources/exactMatchUploadAgent.md) collection|Get the exactMatchUploadAgents from the exactMatchUploadAgents navigation property.|
|[Add exactMatchUploadAgents](../api/dataclassificationservice-post-exactmatchuploadagents.md)|[exactMatchUploadAgent](../resources/exactMatchUploadAgent.md)|Add exactMatchUploadAgents by posting to the exactMatchUploadAgents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|creationDateTime|DateTimeOffset||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
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

