---
title: "onenoteEntityHierarchyModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenoteEntityHierarchyModel resource type




Inherits from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onenoteEntityHierarchyModels](../api/onenoteentityhierarchymodel-list.md)|[onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md) collection|List properties and relationships of the [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) objects.|
|[Get onenoteEntityHierarchyModel](../api/onenoteentityhierarchymodel-get.md)|[onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|Read properties and relationships of the [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)||
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteEntityHierarchyModel",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteEntityHierarchyModel",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```

