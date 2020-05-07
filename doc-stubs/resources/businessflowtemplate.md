---
title: "businessFlowTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# businessFlowTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List businessFlowTemplates](../api/businessflowtemplate-list.md)|[businessFlowTemplate](../resources/businessflowtemplate.md) collection|Get a list of the [businessFlowTemplate](../resources/businessflowtemplate.md) objects and their properties.|
|[Get businessFlowTemplate](../api/businessflowtemplate-get.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Read the properties and relationships of a [businessFlowTemplate](../resources/businessflowtemplate.md) object.|
|[Create businessFlowTemplate](../api/businessflowtemplate-post-businessflowtemplates.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Create a new [businessFlowTemplate](../resources/businessflowtemplate.md) object.|
|[Delete businessFlowTemplate](../api/businessflowtemplate-delete.md)|None|Deletes a [businessFlowTemplate](../resources/businessflowtemplate.md) object.|
|[Update businessFlowTemplate](../api/businessflowtemplate-update.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Update the properties of a [businessFlowTemplate](../resources/businessflowtemplate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.businessFlowTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.businessFlowTemplate",
  "id": "String (identifier)",
  "displayName": "String"
}
```

