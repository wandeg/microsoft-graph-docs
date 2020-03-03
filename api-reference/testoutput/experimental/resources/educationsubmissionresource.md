---
title: "educationSubmissionResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationSubmissionResource resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationSubmissionResources](../api/educationsubmissionresource-list.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md) collection|List properties and relationships of the [educationSubmissionResource](../resources/educationsubmissionresource.md) objects.|
|[Get educationSubmissionResource](../api/educationsubmissionresource-get.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Read properties and relationships of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Create educationSubmissionResource](../api/educationsubmissionresource-create.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Create a new [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|
|[Delete educationSubmissionResource](../api/educationsubmissionresource-delete.md)|None|Deletes a [educationSubmissionResource](../resources/educationsubmissionresource.md).|
|[Update educationSubmissionResource](../api/educationsubmissionresource-update.md)|[educationSubmissionResource](../resources/educationsubmissionresource.md)|Update the properties of a [educationSubmissionResource](../resources/educationsubmissionresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentResourceUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationresource.md)||

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

