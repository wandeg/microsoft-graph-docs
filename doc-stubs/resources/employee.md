---
title: "employee resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# employee resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List picture](../api/employee-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Create picture](../api/employee-post-picture.md)|[picture](../resources/picture.md)|Create a new picture object.|
|[Delete picture](../api/employee-delete-picture.md)|None|Delete a [picture](../resources/picture.md) object.|
|[Update picture](../api/employee-update-picture.md)|[picture](../resources/picture.md)|Update the properties of a picture object.|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read the properties and relationships of a [picture](../resources/picture.md) object.|
|[List employees](../api/company-list-employees.md)|[employee](../resources/employee.md) collection|Get the employees from the employees navigation property.|
|[Create employees](../api/company-post-employees.md)|[employee](../resources/employee.md)|Create a new employees object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|birthDate|Date|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|employmentDate|Date|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|jobTitle|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|middleName|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|personalEmail|String|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|statisticsGroupCode|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|terminationDate|Date|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|picture|[picture](../resources/picture.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.employee",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.employee",
  "id": "String (identifier)",
  "number": "String",
  "displayName": "String",
  "givenName": "String",
  "middleName": "String",
  "surname": "String",
  "jobTitle": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "mobilePhone": "String",
  "email": "String",
  "personalEmail": "String",
  "employmentDate": "Date",
  "terminationDate": "Date",
  "status": "String",
  "birthDate": "Date",
  "statisticsGroupCode": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

