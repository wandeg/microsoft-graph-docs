---
title: "dataPolicyOperation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# dataPolicyOperation resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List dataPolicyOperations](../api/datapolicyoperation-list.md)|[dataPolicyOperation](../resources/datapolicyoperation.md) collection|Get a list of the [dataPolicyOperation](../resources/datapolicyoperation.md) objects and their properties.|
|[Get dataPolicyOperation](../api/datapolicyoperation-get.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Read the properties and relationships of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.|
|[Create dataPolicyOperation](../api/datapolicyoperation-post-datapolicyoperations.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Create a new [dataPolicyOperation](../resources/datapolicyoperation.md) object.|
|[Delete dataPolicyOperation](../api/datapolicyoperation-delete.md)|None|Deletes a [dataPolicyOperation](../resources/datapolicyoperation.md) object.|
|[Update dataPolicyOperation](../api/datapolicyoperation-update.md)|[dataPolicyOperation](../resources/datapolicyoperation.md)|Update the properties of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|progress|Double|**TODO: Add Description**|
|status|dataPolicyOperationStatus|**TODO: Add Description**. Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String|**TODO: Add Description**|
|submittedDateTime|DateTimeOffset|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataPolicyOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "id": "String (identifier)",
  "completedDateTime": "String (timestamp)",
  "status": "String",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)",
  "progress": "Double"
}
```

