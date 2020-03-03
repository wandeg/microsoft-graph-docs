---
title: "externalConnection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# externalConnection resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List externalConnections](../api/externalconnection-list.md)|[externalConnection](../resources/externalconnection.md) collection|List properties and relationships of the [externalConnection](../resources/externalconnection.md) objects.|
|[Get externalConnection](../api/externalconnection-get.md)|[externalConnection](../resources/externalconnection.md)|Read properties and relationships of the [externalConnection](../resources/externalconnection.md) object.|
|[Create externalConnection](../api/externalconnection-post-connections.md)|[externalConnection](../resources/externalconnection.md)|Create a new [externalConnection](../resources/externalconnection.md) object.|
|[Delete externalConnection](../api/externalconnection-delete.md)|None|Deletes a [externalConnection](../resources/externalconnection.md).|
|[Update externalConnection](../api/externalconnection-update.md)|[externalConnection](../resources/externalconnection.md)|Update the properties of a [externalConnection](../resources/externalconnection.md) object.|
|[Get schema](../api/schema-get.md)|[schema](../resources/schema.md)|Read properties and relationships of the [schema](../resources/schema.md) object.|
|[List items](../api/externalconnection-list-items.md)|[externalItem](../resources/externalitem.md) collection|Get the externalItems from the items navigation property.|
|[Add items](../api/externalconnection-post-items.md)|[externalItem](../resources/externalitem.md)|Add items by posting to the items collection.|
|[List operations](../api/externalconnection-list-operations.md)|[connectionOperation](../resources/connectionoperation.md) collection|Get the connectionOperations from the operations navigation property.|
|[Add operations](../api/externalconnection-post-operations.md)|[connectionOperation](../resources/connectionoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|[configuration](../resources/configuration.md)||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|items|[externalItem](../resources/externalitem.md) collection||
|operations|[connectionOperation](../resources/connectionoperation.md) collection||
|schema|[schema](../resources/schema.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalConnection",
  "id": "String (identifier)",
  "name": "String",
  "description": "String",
  "configuration": {
    "@odata.type": "microsoft.graph.configuration",
    "authorizedApps": [
      "String"
    ]
  }
}
```

