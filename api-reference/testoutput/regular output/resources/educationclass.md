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
|[List schools](../api/educationclass-list-schools.md)|[educationSchool](../resources/educationSchool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationclass-post-schools.md)|[educationSchool](../resources/educationSchool.md)|Create schools by posting to the schools collection.|
|[List members](../api/educationclass-list-members.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the members navigation property.|
|[Create members](../api/educationclass-post-members.md)|[educationUser](../resources/educationUser.md)|Create members by posting to the members collection.|
|[List teachers](../api/educationclass-list-teachers.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the teachers navigation property.|
|[Create teachers](../api/educationclass-post-teachers.md)|[educationUser](../resources/educationUser.md)|Create teachers by posting to the teachers collection.|
|[Get group](../api/group-get.md)|[group](../resources/group.md)|Read properties and relationships of the [group](../resources/group.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classCode|String||
|createdBy|[identitySet](../resources/identitySet.md)||
|description|String||
|displayName|String||
|externalId|String||
|externalName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|mailNickname|String||
|term|[educationTerm](../resources/educationTerm.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
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
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  }
}
```

