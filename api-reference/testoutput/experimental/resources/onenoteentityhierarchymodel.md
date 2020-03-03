---
title: "onenoteEntityHierarchyModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenoteEntityHierarchyModel resource type


Namespace: microsoft.graph




Inherits from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onenoteEntityHierarchyModels](../api/onenoteentityhierarchymodel-list.md)|[onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) collection|List properties and relationships of the [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) objects.|
|[Get onenoteEntityHierarchyModel](../api/onenoteentityhierarchymodel-get.md)|[onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|Read properties and relationships of the [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

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

