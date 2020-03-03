---
title: "educationClass resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationClass resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationClass](../api/educationclass-get.md)|[educationClass](../resources/educationClass.md)|Read properties and relationships of the [educationClass](../resources/educationclass.md) object.|
|[Delete educationClass](../api/educationclass-delete.md)|None|Deletes a [educationClass](../resources/educationclass.md).|
|[Update educationClass](../api/educationclass-update.md)|[educationClass](../resources/educationClass.md)|Update the properties of a [educationClass](../resources/educationclass.md) object.|
|[delta](../api/educationclass-delta.md)|[educationClass](../resources/educationClass.md) collection||
|[List assignments](../api/educationclass-list-assignments.md)|[educationAssignment](../resources/educationAssignment.md) collection|Get the educationAssignments from the assignments navigation property.|
|[Add assignments](../api/educationclass-post-assignments.md)|[educationAssignment](../resources/educationAssignment.md)|Add assignments by posting to the assignments collection.|
|[List assignmentCategories](../api/educationclass-list-assignmentcategories.md)|[educationCategory](../resources/educationCategory.md) collection|Get the educationCategories from the assignmentCategories navigation property.|
|[Add assignmentCategories](../api/educationclass-post-assignmentcategories.md)|[educationCategory](../resources/educationCategory.md)|Add assignmentCategories by posting to the assignmentCategories collection.|
|[List members](../api/educationclass-list-members.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the members navigation property.|
|[Create members](../api/educationclass-post-members.md)|[educationUser](../resources/educationUser.md)|Create members by posting to the members collection.|
|[List teachers](../api/educationclass-list-teachers.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the teachers navigation property.|
|[Create teachers](../api/educationclass-post-teachers.md)|[educationUser](../resources/educationUser.md)|Create teachers by posting to the teachers collection.|
|[List schools](../api/educationclass-list-schools.md)|[educationSchool](../resources/educationSchool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationclass-post-schools.md)|[educationSchool](../resources/educationSchool.md)|Create schools by posting to the schools collection.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of the [group](../resources/group.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classCode|String||
|course|[educationCourse](../resources/educationCourse.md)||
|createdBy|[identitySet](../resources/identitySet.md)||
|description|String||
|displayName|String||
|externalId|String||
|externalName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|grade|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|mailNickname|String||
|term|[educationTerm](../resources/educationTerm.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignmentCategories|[educationCategory](../resources/educationCategory.md) collection||
|assignments|[educationAssignment](../resources/educationAssignment.md) collection||
|group|[group](../resources/group.md)||
|members|[educationUser](../resources/educationUser.md) collection||
|schools|[educationSchool](../resources/educationSchool.md) collection||
|teachers|[educationUser](../resources/educationUser.md) collection||

## JSON Representation
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
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
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

