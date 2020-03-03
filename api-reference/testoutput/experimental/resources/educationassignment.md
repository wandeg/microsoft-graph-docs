---
title: "educationAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationAssignment resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationAssignment](../api/educationassignment-get.md)|[educationAssignment](../resources/educationAssignment.md)|Read properties and relationships of the [educationAssignment](../resources/educationassignment.md) object.|
|[Delete educationAssignment](../api/educationassignment-delete.md)|None|Deletes a [educationAssignment](../resources/educationassignment.md).|
|[Update educationAssignment](../api/educationassignment-update.md)|[educationAssignment](../resources/educationAssignment.md)|Update the properties of a [educationAssignment](../resources/educationassignment.md) object.|
|[publish](../api/educationassignment-publish.md)|[educationAssignment](../resources/educationAssignment.md)||
|[getResourcesFolderUrl](../api/educationassignment-getresourcesfolderurl.md)|String||
|[List resources](../api/educationassignment-list-resources.md)|[educationAssignmentResource](../resources/educationAssignmentResource.md) collection|Get the educationAssignmentResources from the resources navigation property.|
|[Add resources](../api/educationassignment-post-resources.md)|[educationAssignmentResource](../resources/educationAssignmentResource.md)|Add resources by posting to the resources collection.|
|[List submissions](../api/educationassignment-list-submissions.md)|[educationSubmission](../resources/educationSubmission.md) collection|Get the educationSubmissions from the submissions navigation property.|
|[Add submissions](../api/educationassignment-post-submissions.md)|[educationSubmission](../resources/educationSubmission.md)|Add submissions by posting to the submissions collection.|
|[List categories](../api/educationassignment-list-categories.md)|[educationCategory](../resources/educationCategory.md) collection|Get the educationCategories from the categories navigation property.|
|[Add categories](../api/educationassignment-post-categories.md)|[educationCategory](../resources/educationCategory.md)|Add categories by posting to the categories collection.|
|[Get educationRubric](../api/educationrubric-get.md)|[educationRubric](../resources/educationRubric.md)|Read properties and relationships of the [educationRubric](../resources/educationrubric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowLateSubmissions|Boolean||
|allowStudentsToAddResourcesToSubmission|Boolean||
|assignDateTime|DateTimeOffset||
|assignedDateTime|DateTimeOffset||
|assignTo|[educationAssignmentRecipient](../resources/educationAssignmentRecipient.md)||
|classId|String||
|closeDateTime|DateTimeOffset||
|createdBy|[identitySet](../resources/identitySet.md)||
|createdDateTime|DateTimeOffset||
|displayName|String||
|dueDateTime|DateTimeOffset||
|grading|[educationAssignmentGradeType](../resources/educationAssignmentGradeType.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|instructions|[educationItemBody](../resources/educationItemBody.md)||
|lastModifiedBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `draft`, `published`, `assigned`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[educationCategory](../resources/educationCategory.md) collection||
|resources|[educationAssignmentResource](../resources/educationAssignmentResource.md) collection||
|rubric|[educationRubric](../resources/educationRubric.md)||
|submissions|[educationSubmission](../resources/educationSubmission.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationAssignment",
  "id": "String (identifier)",
  "classId": "String",
  "displayName": "String",
  "instructions": {
    "@odata.type": "microsoft.graph.educationItemBody"
  },
  "closeDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "assignDateTime": "String (timestamp)",
  "assignedDateTime": "String (timestamp)",
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "assignTo": {
    "@odata.type": "microsoft.graph.educationAssignmentRecipient"
  },
  "allowLateSubmissions": true,
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "allowStudentsToAddResourcesToSubmission": true,
  "status": "String"
}
```

