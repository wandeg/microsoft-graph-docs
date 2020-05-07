---
title: "educationAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[publish](../api/educationassignment-publish.md)|[educationAssignment](../resources/educationassignment.md)|**TODO: Add Description**|
|[getResourcesFolderUrl](../api/educationassignment-getresourcesfolderurl.md)|String|**TODO: Add Description**|
|[List resources](../api/educationassignment-list-resources.md)|[educationAssignmentResource](../resources/educationassignmentresource.md) collection|Get the educationAssignmentResources from the resources navigation property.|
|[Create resources](../api/educationassignment-post-resources.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Create a new resources object.|
|[Delete resources](../api/educationassignment-delete-resources.md)|None|Delete a [educationAssignmentResource](../resources/educationassignmentresource.md) object.|
|[Update resources](../api/educationassignment-update-resources.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Update the properties of a resources object.|
|[Get educationAssignmentResource](../api/educationassignmentresource-get.md)|[educationAssignmentResource](../resources/educationassignmentresource.md)|Read the properties and relationships of an [educationAssignmentResource](../resources/educationassignmentresource.md) object.|
|[List submissions](../api/educationassignment-list-submissions.md)|[educationSubmission](../resources/educationsubmission.md) collection|Get the educationSubmissions from the submissions navigation property.|
|[Create submissions](../api/educationassignment-post-submissions.md)|[educationSubmission](../resources/educationsubmission.md)|Create a new submissions object.|
|[Delete submissions](../api/educationassignment-delete-submissions.md)|None|Delete a [educationSubmission](../resources/educationsubmission.md) object.|
|[Update submissions](../api/educationassignment-update-submissions.md)|[educationSubmission](../resources/educationsubmission.md)|Update the properties of a submissions object.|
|[Get educationSubmission](../api/educationsubmission-get.md)|[educationSubmission](../resources/educationsubmission.md)|Read the properties and relationships of an [educationSubmission](../resources/educationsubmission.md) object.|
|[List categories](../api/educationassignment-list-categories.md)|[educationCategory](../resources/educationcategory.md) collection|Get the educationCategories from the categories navigation property.|
|[Create categories](../api/educationassignment-post-categories.md)|[educationCategory](../resources/educationcategory.md)|Create a new categories object.|
|[Delete categories](../api/educationassignment-delete-categories.md)|None|Delete a [educationCategory](../resources/educationcategory.md) object.|
|[Update categories](../api/educationassignment-update-categories.md)|[educationCategory](../resources/educationcategory.md)|Update the properties of a categories object.|
|[Get educationCategory](../api/educationcategory-get.md)|[educationCategory](../resources/educationcategory.md)|Read the properties and relationships of an [educationCategory](../resources/educationcategory.md) object.|
|[List rubric](../api/educationassignment-list-rubric.md)|[educationRubric](../resources/educationrubric.md) collection|Get the educationRubrics from the rubric navigation property.|
|[Create rubric](../api/educationassignment-post-rubric.md)|[educationRubric](../resources/educationrubric.md)|Create a new rubric object.|
|[Delete rubric](../api/educationassignment-delete-rubric.md)|None|Delete a [educationRubric](../resources/educationrubric.md) object.|
|[Update rubric](../api/educationassignment-update-rubric.md)|[educationRubric](../resources/educationrubric.md)|Update the properties of a rubric object.|
|[Get educationRubric](../api/educationrubric-get.md)|[educationRubric](../resources/educationrubric.md)|Read the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.|
|[List assignments](../api/educationclass-list-assignments.md)|[educationAssignment](../resources/educationassignment.md) collection|Get the educationAssignments from the assignments navigation property.|
|[Create assignments](../api/educationclass-post-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Create a new assignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowLateSubmissions|Boolean|**TODO: Add Description**|
|allowStudentsToAddResourcesToSubmission|Boolean|**TODO: Add Description**|
|assignDateTime|DateTimeOffset|**TODO: Add Description**|
|assignedDateTime|DateTimeOffset|**TODO: Add Description**|
|assignTo|[educationAssignmentRecipient](../resources/educationassignmentrecipient.md)|**TODO: Add Description**|
|classId|String|**TODO: Add Description**|
|closeDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|instructions|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|educationAssignmentStatus|**TODO: Add Description**. Possible values are: `draft`, `published`, `assigned`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[educationCategory](../resources/educationcategory.md) collection|**TODO: Add Description**|
|resources|[educationAssignmentResource](../resources/educationassignmentresource.md) collection|**TODO: Add Description**|
|rubric|[educationRubric](../resources/educationrubric.md)|**TODO: Add Description**|
|submissions|[educationSubmission](../resources/educationsubmission.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "allowLateSubmissions": "Boolean",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "allowStudentsToAddResourcesToSubmission": "Boolean",
  "status": "String"
}
```

