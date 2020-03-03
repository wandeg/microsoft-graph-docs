---
title: "educationSchool resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationSchool resource type




Inherits from [educationOrganization](../resources/educationOrganization.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationSchool](../api/educationschool-get.md)|[educationSchool](../resources/educationSchool.md)|Read properties and relationships of the [educationSchool](../resources/educationschool.md) object.|
|[Delete educationSchool](../api/educationschool-delete.md)|None|Deletes a [educationSchool](../resources/educationschool.md).|
|[Update educationSchool](../api/educationschool-update.md)|[educationSchool](../resources/educationSchool.md)|Update the properties of a [educationSchool](../resources/educationschool.md) object.|
|[delta](../api/educationschool-delta.md)|[educationSchool](../resources/educationSchool.md) collection||
|[List classes](../api/educationschool-list-classes.md)|[educationClass](../resources/educationClass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationschool-post-classes.md)|[educationClass](../resources/educationClass.md)|Create classes by posting to the classes collection.|
|[List users](../api/educationschool-list-users.md)|[educationUser](../resources/educationUser.md) collection|Get the educationUsers from the users navigation property.|
|[Create users](../api/educationschool-post-users.md)|[educationUser](../resources/educationUser.md)|Create users by posting to the users collection.|
|[Get administrativeUnit](../api/administrativeunit-get.md)|[administrativeUnit](../resources/administrativeUnit.md)|Read properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicalAddress.md)||
|createdBy|[identitySet](../resources/identitySet.md)||
|description|String| Inherited from [educationOrganization](../resources/educationOrganization.md)|
|displayName|String| Inherited from [educationOrganization](../resources/educationOrganization.md)|
|externalId|String||
|externalPrincipalId|String||
|externalSource|Enumeration| Inherited from [educationOrganization](../resources/educationOrganization.md). Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|fax|String||
|highestGrade|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lowestGrade|String||
|phone|String||
|principalEmail|String||
|principalName|String||
|schoolNumber|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|administrativeUnit|[administrativeUnit](../resources/administrativeUnit.md)||
|classes|[educationClass](../resources/educationClass.md) collection||
|users|[educationUser](../resources/educationUser.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "String",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryOrRegion": "String",
    "postalCode": "String"
  }
}
```

