---
title: "workbookApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# workbookApplication resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get workbookApplication](../api/workbookapplication-get.md)|[workbookApplication](../resources/workbookapplication.md)|Read properties and relationships of a [workbookApplication](../resources/workbookapplication.md) object.|
|[Update workbookApplication](../api/workbookapplication-update.md)|[workbookApplication](../resources/workbookapplication.md)|Update the properties of a [workbookApplication](../resources/workbookapplication.md) object.|
|[calculate](../api/workbookapplication-calculate.md)|None|**TODO: Add Description**|
|[List application](../api/workbook-list-application.md)|[workbookApplication](../resources/workbookapplication.md) collection|Get the workbookApplications from the application navigation property.|
|[Create application](../api/workbook-post-application.md)|[workbookApplication](../resources/workbookapplication.md)|Create a new application object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calculationMode|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookApplication",
  "id": "String (identifier)",
  "calculationMode": "String"
}
```

