---
title: "businessFlowTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# businessFlowTemplate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List businessFlowTemplates](../api/businessflowtemplate-list.md)|[businessFlowTemplate](../resources/businessflowtemplate.md) collection|List properties and relationships of the [businessFlowTemplate](../resources/businessflowtemplate.md) objects.|
|[Get businessFlowTemplate](../api/businessflowtemplate-get.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Read properties and relationships of the [businessFlowTemplate](../resources/businessflowtemplate.md) object.|
|[Create businessFlowTemplate](../api/businessflowtemplate-post-businessflowtemplates.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Create a new [businessFlowTemplate](../resources/businessflowtemplate.md) object.|
|[Delete businessFlowTemplate](../api/businessflowtemplate-delete.md)|None|Deletes a [businessFlowTemplate](../resources/businessflowtemplate.md).|
|[Update businessFlowTemplate](../api/businessflowtemplate-update.md)|[businessFlowTemplate](../resources/businessflowtemplate.md)|Update the properties of a [businessFlowTemplate](../resources/businessflowtemplate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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

