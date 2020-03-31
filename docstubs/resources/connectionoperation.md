---
title: "connectionOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# connectionOperation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get connectionOperation](../api/connectionoperation-get.md)|[connectionOperation](../resources/connectionoperation.md)|Read properties and relationships of the [connectionOperation](../resources/connectionoperation.md) object.|
|[Update connectionOperation](../api/connectionoperation-update.md)|[connectionOperation](../resources/connectionoperation.md)|Update the properties of a [connectionOperation](../resources/connectionoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[errorDetail](../resources/errordetail.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration| Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|

## Relationships
None

## JSON representation
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

