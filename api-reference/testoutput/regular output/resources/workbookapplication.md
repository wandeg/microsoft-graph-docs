---
title: "workbookApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookApplication resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookApplications](../api/workbookapplication-list.md)|[workbookApplication](../resources/workbookApplication.md) collection|List properties and relationships of the [workbookApplication](../resources/workbookapplication.md) objects.|
|[Get workbookApplication](../api/workbookapplication-get.md)|[workbookApplication](../resources/workbookApplication.md)|Read properties and relationships of the [workbookApplication](../resources/workbookapplication.md) object.|
|[Create workbookApplication](../api/workbookapplication-create.md)|[workbookApplication](../resources/workbookApplication.md)|Create a new [workbookApplication](../resources/workbookapplication.md) object.|
|[Delete workbookApplication](../api/workbookapplication-delete.md)|None|Deletes a [workbookApplication](../resources/workbookapplication.md).|
|[Update workbookApplication](../api/workbookapplication-update.md)|[workbookApplication](../resources/workbookApplication.md)|Update the properties of a [workbookApplication](../resources/workbookapplication.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calculationMode|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
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

