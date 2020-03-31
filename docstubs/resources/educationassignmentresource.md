---
title: "educationAssignmentResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationAssignmentResource resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationAssignmentResource](../api/educationassignmentresource-get.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Read properties and relationships of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.|
|[Update educationAssignmentResource](../api/educationassignmentresource-update.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Update the properties of a [educationAssignmentResource](../resources/educationassignmentresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|distributeForStudentWork|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationresource.md)||

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

