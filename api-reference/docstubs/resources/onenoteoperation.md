---
title: "onenoteOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenoteOperation resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [operation](../resources/operation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteOperation](../api/onenoteoperation-get.md)|[onenoteOperation](../resources/onenoteoperation.md)|Read the properties and relationships of an [onenoteOperation](../resources/onenoteoperation.md) object.|
|[Update onenoteOperation](../api/onenoteoperation-update.md)|[onenoteOperation](../resources/onenoteoperation.md)|Update the properties of an [onenoteOperation](../resources/onenoteoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|error|[onenoteOperationError](../resources/onenoteoperationerror.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [operation](../resources/operation.md)|
|percentComplete|String|**TODO: Add Description**|
|resourceId|String|**TODO: Add Description**|
|resourceLocation|String|**TODO: Add Description**|
|status|operationStatus|**TODO: Add Description** Inherited from [operation](../resources/operation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteOperation",
  "baseType": "microsoft.graph.operation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteOperation",
  "id": "String (identifier)",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "resourceId": "String",
  "error": {
    "@odata.type": "microsoft.graph.onenoteOperationError"
  },
  "percentComplete": "String"
}
```

