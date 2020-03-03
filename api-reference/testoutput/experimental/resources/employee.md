---
title: "employee resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# employee resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get employee](../api/employee-get.md)|[employee](../resources/employee.md)|Read properties and relationships of the [employee](../resources/employee.md) object.|
|[Delete employee](../api/employee-delete.md)|None|Deletes a [employee](../resources/employee.md).|
|[Update employee](../api/employee-update.md)|[employee](../resources/employee.md)|Update the properties of a [employee](../resources/employee.md) object.|
|[List picture](../api/employee-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Add picture](../api/employee-post-picture.md)|[picture](../resources/picture.md)|Add picture by posting to the picture collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postalAddressType.md)||
|birthDate|Date||
|displayName|String||
|email|String||
|employmentDate|Date||
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|jobTitle|String||
|lastModifiedDateTime|DateTimeOffset||
|middleName|String||
|mobilePhone|String||
|number|String||
|personalEmail|String||
|phoneNumber|String||
|statisticsGroupCode|String||
|status|String||
|surname|String||
|terminationDate|Date||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|picture|[picture](../resources/picture.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryLetterCode": "String",
    "postalCode": "String"
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

