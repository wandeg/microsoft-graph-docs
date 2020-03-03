---
title: "educationSubmissionResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationSubmissionResource resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md)|[educationSubmissionResource](../resources/educationSubmissionResource.md)|Read properties and relationships of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Delete educationSubmissionResource](../api/educationsubmissionresource-delete.md)|None|Deletes a [educationSubmissionResource](../resources/educationsubmissionresource.md).|
|[Update educationSubmissionResource](../api/educationsubmissionresource-update.md)|[educationSubmissionResource](../resources/educationSubmissionResource.md)|Update the properties of a [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentResourceUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationResource.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSubmissionResource",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "id": "String (identifier)",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  },
  "assignmentResourceUrl": "String"
}
```

