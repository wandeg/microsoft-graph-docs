---
title: "educationRoot resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationRoot resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationRoot](../api/educationroot-get.md)|[educationRoot](../resources/educationRoot.md)|Read properties and relationships of the [educationRoot](../resources/educationroot.md) object.|
|[Update educationRoot](../api/educationroot-update.md)|[educationRoot](../resources/educationRoot.md)|Update the properties of a [educationRoot](../resources/educationroot.md) object.|
|[List classes](../api/educationroot-list-classes.md)|[educationClass](../resources/educationClass.md) collection|Get the educationClasses from the classes navigation property.|
|[Add classes](../api/educationroot-post-classes.md)|[educationClass](../resources/educationClass.md)|Add classes by posting to the classes collection.|
|[List schools](../api/educationroot-list-schools.md)|[educationSchool](../resources/educationSchool.md) collection|Get the educationSchools from the schools navigation property.|
|[Add schools](../api/educationroot-post-schools.md)|[educationSchool](../resources/educationSchool.md)|Add schools by posting to the schools collection.|
|[List users](../api/educationroot-list-users.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the users navigation property.|
|[Add users](../api/educationroot-post-users.md)|[educationUser](../resources/educationUser.md)|Add users by posting to the users collection.|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationUser.md)|Read properties and relationships of the [educationUser](../resources/educationuser.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationClass.md) collection||
|me|[educationUser](../resources/educationUser.md)||
|schools|[educationSchool](../resources/educationSchool.md) collection||
|users|[educationUser](../resources/educationUser.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

