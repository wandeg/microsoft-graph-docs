---
title: "printService resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printService resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List endpoints](../api/printservice-list-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md) collection|Get the printServiceEndpoints from the endpoints navigation property.|
|[Create endpoints](../api/printservice-post-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Create a new endpoints object.|
|[Delete endpoints](../api/printservice-delete-endpoints.md)|None|Delete an [printServiceEndpoint](../resources/printserviceendpoint.md) object.|
|[Update endpoints](../api/printservice-update-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Update the properties of an endpoints object.|
|[Get printServiceEndpoint](../api/printserviceendpoint-get.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Read the properties and relationships of a [printServiceEndpoint](../resources/printserviceendpoint.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|endpoints|[printServiceEndpoint](../resources/printserviceendpoint.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

