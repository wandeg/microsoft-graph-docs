---
title: "externalConnection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# externalConnection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List externalConnections](../api/externalconnection-list.md)|[externalConnection](../resources/externalconnection.md) collection|Get a list of the [externalConnection](../resources/externalconnection.md) objects and their properties.|
|[Get externalConnection](../api/externalconnection-get.md)|[externalConnection](../resources/externalconnection.md)|Read the properties and relationships of an [externalConnection](../resources/externalconnection.md) object.|
|[Create externalConnection](../api/externalconnection-post-connections.md)|[externalConnection](../resources/externalconnection.md)|Create a new [externalConnection](../resources/externalconnection.md) object.|
|[Delete externalConnection](../api/externalconnection-delete.md)|None|Deletes an [externalConnection](../resources/externalconnection.md) object.|
|[Update externalConnection](../api/externalconnection-update.md)|[externalConnection](../resources/externalconnection.md)|Update the properties of an [externalConnection](../resources/externalconnection.md) object.|
|[List schema](../api/externalconnection-list-schema.md)|[schema](../resources/schema.md) collection|Get the schemata from the schema navigation property.|
|[Create schema](../api/externalconnection-post-schema.md)|[schema](../resources/schema.md)|Create a new schema object.|
|[Delete schema](../api/externalconnection-delete-schema.md)|None|Delete a [schema](../resources/schema.md) object.|
|[Update schema](../api/externalconnection-update-schema.md)|[schema](../resources/schema.md)|Update the properties of a schema object.|
|[Get schema](../api/schema-get.md)|[schema](../resources/schema.md)|Read the properties and relationships of a [schema](../resources/schema.md) object.|
|[List items](../api/externalconnection-list-items.md)|[externalItem](../resources/externalitem.md) collection|Get the externalItems from the items navigation property.|
|[Create items](../api/externalconnection-post-items.md)|[externalItem](../resources/externalitem.md)|Create a new items object.|
|[Delete items](../api/externalconnection-delete-items.md)|None|Delete an [externalItem](../resources/externalitem.md) object.|
|[Update items](../api/externalconnection-update-items.md)|[externalItem](../resources/externalitem.md)|Update the properties of an items object.|
|[Get externalItem](../api/externalitem-get.md)|[externalItem](../resources/externalitem.md)|Read the properties and relationships of an [externalItem](../resources/externalitem.md) object.|
|[List operations](../api/externalconnection-list-operations.md)|[connectionOperation](../resources/connectionoperation.md) collection|Get the connectionOperations from the operations navigation property.|
|[Create operations](../api/externalconnection-post-operations.md)|[connectionOperation](../resources/connectionoperation.md)|Create a new operations object.|
|[Delete operations](../api/externalconnection-delete-operations.md)|None|Delete an [connectionOperation](../resources/connectionoperation.md) object.|
|[Update operations](../api/externalconnection-update-operations.md)|[connectionOperation](../resources/connectionoperation.md)|Update the properties of an operations object.|
|[Get connectionOperation](../api/connectionoperation-get.md)|[connectionOperation](../resources/connectionoperation.md)|Read the properties and relationships of a [connectionOperation](../resources/connectionoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|[configuration](../resources/configuration.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|items|[externalItem](../resources/externalitem.md) collection|**TODO: Add Description**|
|operations|[connectionOperation](../resources/connectionoperation.md) collection|**TODO: Add Description**|
|schema|[schema](../resources/schema.md)|**TODO: Add Description**|

## JSON representation
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

