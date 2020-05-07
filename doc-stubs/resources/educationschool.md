---
title: "educationSchool resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationSchool resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [educationOrganization](../resources/educationorganization.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[delta](../api/educationschool-delta.md)|[educationSchool](../resources/educationschool.md) collection|**TODO: Add Description**|
|[List classes](../api/educationschool-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Add classes](../api/educationschool-post-classes.md)|[educationClass](../resources/educationclass.md)|Add classes by posting to the classes collection.|
|[Remove classes](../api/educationschool-delete-classes.md)|None|Remove a [educationClass](../resources/educationclass.md) object.|
|[List users](../api/educationschool-list-users.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUsers from the users navigation property.|
|[Add users](../api/educationschool-post-users.md)|[educationUser](../resources/educationuser.md)|Add users by posting to the users collection.|
|[Remove users](../api/educationschool-delete-users.md)|None|Remove a [educationUser](../resources/educationuser.md) object.|
|[List administrativeUnit](../api/educationschool-list-administrativeunit.md)|[administrativeUnit](../resources/administrativeunit.md) collection|Get the administrativeUnits from the administrativeUnit navigation property.|
|[Add administrativeUnit](../api/educationschool-post-administrativeunit.md)|[administrativeUnit](../resources/administrativeunit.md)|Add administrativeUnit by posting to the administrativeUnit collection.|
|[Remove administrativeUnit](../api/educationschool-delete-administrativeunit.md)|None|Remove an [administrativeUnit](../resources/administrativeunit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|displayName|String|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md)|
|externalId|String|**TODO: Add Description**|
|externalPrincipalId|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description** Inherited from [educationOrganization](../resources/educationorganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|fax|String|**TODO: Add Description**|
|highestGrade|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lowestGrade|String|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|principalEmail|String|**TODO: Add Description**|
|principalName|String|**TODO: Add Description**|
|schoolNumber|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|administrativeUnit|[administrativeUnit](../resources/administrativeunit.md)|**TODO: Add Description**|
|classes|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|users|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationSchool",
  "baseType": "microsoft.graph.educationOrganization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSchool",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "lowestGrade": "String",
  "highestGrade": "String",
  "schoolNumber": "String",
  "externalId": "String",
  "phone": "String",
  "fax": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  }
}
```

