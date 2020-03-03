---
title: "plannerTaskDetails resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# plannerTaskDetails resource type


Namespace: microsoft.graph




Inherits from [plannerDelta](../resources/plannerdelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List plannerTaskDetailses](../api/plannertaskdetails-list.md)|[plannerTaskDetails](../resources/plannertaskdetails.md) collection|List properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) objects.|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Read properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Create plannerTaskDetails](../api/plannertaskdetails-create.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Create a new [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Delete plannerTaskDetails](../api/plannertaskdetails-delete.md)|None|Deletes a [plannerTaskDetails](../resources/plannertaskdetails.md).|
|[Update plannerTaskDetails](../api/plannertaskdetails-update.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Update the properties of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)||
|description|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTaskDetails",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTaskDetails",
  "id": "String (identifier)",
  "description": "String",
  "previewType": "String",
  "references": {
    "@odata.type": "microsoft.graph.plannerExternalReferences"
  },
  "checklist": {
    "@odata.type": "microsoft.graph.plannerChecklistItems"
  }
}
```

