---
title: "connectionOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# connectionOperation resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get connectionOperation](../api/connectionoperation-get.md)|[connectionOperation](../resources/connectionOperation.md)|Read properties and relationships of the [connectionOperation](../resources/connectionoperation.md) object.|
|[Delete connectionOperation](../api/connectionoperation-delete.md)|None|Deletes a [connectionOperation](../resources/connectionoperation.md).|
|[Update connectionOperation](../api/connectionoperation-update.md)|[connectionOperation](../resources/connectionOperation.md)|Update the properties of a [connectionOperation](../resources/connectionoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[errorDetail](../resources/errorDetail.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|. Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectionOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionOperation",
  "id": "String (identifier)",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.errorDetail"
  }
}
```

