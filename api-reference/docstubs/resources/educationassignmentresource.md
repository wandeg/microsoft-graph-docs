---
title: "educationAssignmentResource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationAssignmentResource resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationAssignmentResource](../api/educationassignmentresource-get.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Read the properties and relationships of an [educationAssignmentResource](../resources/educationassignmentresource.md) object.|
|[Update educationAssignmentResource](../api/educationassignmentresource-update.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Update the properties of an [educationAssignmentResource](../resources/educationassignmentresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|distributeForStudentWork|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationresource.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "id": "String (identifier)",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  }
}
```

