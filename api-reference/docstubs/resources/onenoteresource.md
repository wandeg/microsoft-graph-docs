---
title: "onenoteResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenoteResource resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteResource](../api/onenoteresource-get.md)|[onenoteResource](../resources/onenoteresource.md)|Read the properties and relationships of an [onenoteResource](../resources/onenoteresource.md) object.|
|[Update onenoteResource](../api/onenoteresource-update.md)|[onenoteResource](../resources/onenoteresource.md)|Update the properties of an [onenoteResource](../resources/onenoteresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteResource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "String (identifier)",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```

