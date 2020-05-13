---
title: "educationRoot resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationRoot resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List classes](../api/educationroot-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationroot-post-classes.md)|[educationClass](../resources/educationclass.md)|Create a new classes object.|
|[Delete classes](../api/educationroot-delete-classes.md)|None|Delete an [educationClass](../resources/educationclass.md) object.|
|[Update classes](../api/educationroot-update-classes.md)|[educationClass](../resources/educationclass.md)|Update the properties of a classes object.|
|[Get classes](../api/educationroot-get-educationclass.md)|[educationClass](../resources/educationclass.md)|Read the properties and relationships of an [educationClass](../resources/educationclass.md) object.|
|[List schools](../api/educationroot-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationroot-post-schools.md)|[educationSchool](../resources/educationschool.md)|Create a new schools object.|
|[Delete schools](../api/educationroot-delete-schools.md)|None|Delete an [educationSchool](../resources/educationschool.md) object.|
|[Update schools](../api/educationroot-update-schools.md)|[educationSchool](../resources/educationschool.md)|Update the properties of a schools object.|
|[Get schools](../api/educationroot-get-educationschool.md)|[educationSchool](../resources/educationschool.md)|Read the properties and relationships of an [educationSchool](../resources/educationschool.md) object.|
|[List users](../api/educationroot-list-users.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the users navigation property.|
|[Create users](../api/educationroot-post-users.md)|[educationUser](../resources/educationuser.md)|Create a new users object.|
|[Delete users](../api/educationroot-delete-users.md)|None|Delete an [educationUser](../resources/educationuser.md) object.|
|[Update users](../api/educationroot-update-users.md)|[educationUser](../resources/educationuser.md)|Update the properties of a users object.|
|[Get users](../api/educationroot-get-educationuser.md)|[educationUser](../resources/educationuser.md)|Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.|
|[List me](../api/educationroot-list-me.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the me navigation property.|
|[Create me](../api/educationroot-post-me.md)|[educationUser](../resources/educationuser.md)|Create a new me object.|
|[Delete me](../api/educationroot-delete-me.md)|None|Delete an [educationUser](../resources/educationuser.md) object.|
|[Update me](../api/educationroot-update-me.md)|[educationUser](../resources/educationuser.md)|Update the properties of a me object.|
|[Get me](../api/educationroot-get-educationuser.md)|[educationUser](../resources/educationuser.md)|Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|me|[educationUser](../resources/educationuser.md)|**TODO: Add Description**|
|schools|[educationSchool](../resources/educationschool.md) collection|**TODO: Add Description**|
|users|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationRoot",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationRoot",
  "id": "String (identifier)"
}
```

