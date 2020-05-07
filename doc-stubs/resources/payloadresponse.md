---
title: "payloadResponse resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# payloadResponse resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List payloadResponses](../api/payloadresponse-list.md)|[payloadResponse](../resources/payloadresponse.md) collection|Get a list of the [payloadResponse](../resources/payloadresponse.md) objects and their properties.|
|[Get payloadResponse](../api/payloadresponse-get.md)|[payloadResponse](../resources/payloadresponse.md)|Read the properties and relationships of a [payloadResponse](../resources/payloadresponse.md) object.|
|[Create payloadResponse](../api/payloadresponse-post-payloadresponse.md)|[payloadResponse](../resources/payloadresponse.md)|Create a new [payloadResponse](../resources/payloadresponse.md) object.|
|[Delete payloadResponse](../api/payloadresponse-delete.md)|None|Deletes a [payloadResponse](../resources/payloadresponse.md) object.|
|[Update payloadResponse](../api/payloadresponse-update.md)|[payloadResponse](../resources/payloadresponse.md)|Update the properties of a [payloadResponse](../resources/payloadresponse.md) object.|
|[List responsepayload](../api/command-list-responsepayload.md)|[payloadResponse](../resources/payloadresponse.md) collection|Get the payloadResponses from the responsepayload navigation property.|
|[Add responsepayload](../api/command-post-responsepayload.md)|[payloadResponse](../resources/payloadresponse.md)|Add responsepayload by posting to the responsepayload collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.payloadResponse",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.payloadResponse",
  "id": "String (identifier)"
}
```

