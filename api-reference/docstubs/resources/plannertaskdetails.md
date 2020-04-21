---
title: "plannerTaskDetails resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# plannerTaskDetails resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Read properties and relationships of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Update plannerTaskDetails](../api/plannertaskdetails-update.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Update the properties of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[List details](../api/plannertask-list-details.md)|[plannerTaskDetails](../resources/plannertaskdetails.md) collection|Get the plannerTaskDetails from the details navigation property.|
|[Create details](../api/plannertask-post-details.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Create a new details object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|checklist|[plannerChecklistItems](../resources/plannerchecklistitems.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|previewType|plannerPreviewType|**TODO: Add Description**. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|references|[plannerExternalReferences](../resources/plannerexternalreferences.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTaskDetails",
  "baseType": "microsoft.graph.entity",
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

