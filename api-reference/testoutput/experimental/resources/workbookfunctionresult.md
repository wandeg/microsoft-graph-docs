---
title: "workbookFunctionResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookFunctionResult resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookFunctionResults](../api/workbookfunctionresult-list.md)|[workbookFunctionResult](../resources/workbookfunctionresult.md) collection|List properties and relationships of the [workbookFunctionResult](../resources/workbookfunctionresult.md) objects.|
|[Get workbookFunctionResult](../api/workbookfunctionresult-get.md)|[workbookFunctionResult](../resources/workbookfunctionresult.md)|Read properties and relationships of the [workbookFunctionResult](../resources/workbookfunctionresult.md) object.|
|[Create workbookFunctionResult](../api/workbookfunctionresult-create.md)|[workbookFunctionResult](../resources/workbookfunctionresult.md)|Create a new [workbookFunctionResult](../resources/workbookfunctionresult.md) object.|
|[Delete workbookFunctionResult](../api/workbookfunctionresult-delete.md)|None|Deletes a [workbookFunctionResult](../resources/workbookfunctionresult.md).|
|[Update workbookFunctionResult](../api/workbookfunctionresult-update.md)|[workbookFunctionResult](../resources/workbookfunctionresult.md)|Update the properties of a [workbookFunctionResult](../resources/workbookfunctionresult.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|value|[Json](../resources/json.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookFunctionResult",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFunctionResult",
  "id": "String (identifier)",
  "error": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

