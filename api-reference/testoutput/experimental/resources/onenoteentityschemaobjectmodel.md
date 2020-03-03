---
title: "onenoteEntitySchemaObjectModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenoteEntitySchemaObjectModel resource type




Inherits from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onenoteEntitySchemaObjectModels](../api/onenoteentityschemaobjectmodel-list.md)|[onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md) collection|List properties and relationships of the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) objects.|
|[Get onenoteEntitySchemaObjectModel](../api/onenoteentityschemaobjectmodel-get.md)|[onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)|Read properties and relationships of the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteEntitySchemaObjectModel",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)"
}
```

