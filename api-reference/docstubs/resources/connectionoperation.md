---
title: "connectionOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# connectionOperation resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get connectionOperation](../api/connectionoperation-get.md)|[connectionOperation](../resources/connectionoperation.md)|Read the properties and relationships of a [connectionOperation](../resources/connectionoperation.md) object.|
|[Update connectionOperation](../api/connectionoperation-update.md)|[connectionOperation](../resources/connectionoperation.md)|Update the properties of a [connectionOperation](../resources/connectionoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[errorDetail](../resources/errordetail.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|connectionOperationStatus|**TODO: Add Description**. Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|

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

