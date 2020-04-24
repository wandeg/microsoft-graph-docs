---
title: "educationClass resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationClass resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationClass](../api/educationclass-get.md)|[educationClass](../resources/educationclass.md)|Read the properties and relationships of an [educationClass](../resources/educationclass.md) object.|
|[Update educationClass](../api/educationclass-update.md)|[educationClass](../resources/educationclass.md)|Update the properties of an [educationClass](../resources/educationclass.md) object.|
|[delta](../api/educationclass-delta.md)|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|[List assignments](../api/educationclass-list-assignments.md)|[educationAssignment](../resources/educationassignment.md) collection|Get the educationAssignments from the assignments navigation property.|
|[Create assignments](../api/educationclass-post-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/educationclass-delete-assignments.md)|None|Delete an [educationAssignment](../resources/educationassignment.md) object.|
|[Update assignments](../api/educationclass-update-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Update the properties of an assignments object.|
|[Get educationAssignment](../api/educationassignment-get.md)|[educationAssignment](../resources/educationassignment.md)|Read the properties and relationships of an [educationAssignment](../resources/educationassignment.md) object.|
|[List assignmentCategories](../api/educationclass-list-assignmentcategories.md)|[educationCategory](../resources/educationcategory.md) collection|Get the educationCategories from the assignmentCategories navigation property.|
|[Create assignmentCategories](../api/educationclass-post-assignmentcategories.md)|[educationCategory](../resources/educationcategory.md)|Create a new assignmentCategories object.|
|[Delete assignmentCategories](../api/educationclass-delete-assignmentcategories.md)|None|Delete an [educationCategory](../resources/educationcategory.md) object.|
|[Update assignmentCategories](../api/educationclass-update-assignmentcategories.md)|[educationCategory](../resources/educationcategory.md)|Update the properties of an assignmentCategories object.|
|[Get educationCategory](../api/educationcategory-get.md)|[educationCategory](../resources/educationcategory.md)|Read the properties and relationships of an [educationCategory](../resources/educationcategory.md) object.|
|[List members](../api/educationclass-list-members.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the members navigation property.|
|[Add members](../api/educationclass-post-members.md)|[educationUser](../resources/educationuser.md)|Add members by posting to the members collection.|
|[Remove members](../api/educationclass-delete-members.md)|None|Remove a [educationUser](../resources/educationuser.md) object.|
|[List teachers](../api/educationclass-list-teachers.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the teachers navigation property.|
|[Add teachers](../api/educationclass-post-teachers.md)|[educationUser](../resources/educationuser.md)|Add teachers by posting to the teachers collection.|
|[Remove teachers](../api/educationclass-delete-teachers.md)|None|Remove a [educationUser](../resources/educationuser.md) object.|
|[List schools](../api/educationclass-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Add schools](../api/educationclass-post-schools.md)|[educationSchool](../resources/educationschool.md)|Add schools by posting to the schools collection.|
|[Remove schools](../api/educationclass-delete-schools.md)|None|Remove a [educationSchool](../resources/educationschool.md) object.|
|[List group](../api/educationclass-list-group.md)|[group](../resources/group.md) collection|Get the groups from the group navigation property.|
|[Add group](../api/educationclass-post-group.md)|[group](../resources/group.md)|Add group by posting to the group collection.|
|[Remove group](../api/educationclass-delete-group.md)|None|Remove a [group](../resources/group.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classCode|String|**TODO: Add Description**|
|course|[educationCourse](../resources/educationcourse.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|externalName|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|grade|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mailNickname|String|**TODO: Add Description**|
|term|[educationTerm](../resources/educationterm.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignmentCategories|[educationCategory](../resources/educationcategory.md) collection|**TODO: Add Description**|
|assignments|[educationAssignment](../resources/educationassignment.md) collection|**TODO: Add Description**|
|group|[group](../resources/group.md)|**TODO: Add Description**|
|members|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|
|schools|[educationSchool](../resources/educationschool.md) collection|**TODO: Add Description**|
|teachers|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "displayName": "String",
  "mailNickname": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "classCode": "String",
  "externalName": "String",
  "externalId": "String",
  "externalSource": "String",
  "grade": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  },
  "course": {
    "@odata.type": "microsoft.graph.educationCourse",
    "subject": "String",
    "courseNumber": "String"
  }
}
```

