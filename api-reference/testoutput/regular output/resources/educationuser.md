---
title: "educationUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationUser resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationUser.md)|Read properties and relationships of the [educationUser](../resources/educationuser.md) object.|
|[Delete educationUser](../api/educationuser-delete.md)|None|Deletes a [educationUser](../resources/educationuser.md).|
|[Update educationUser](../api/educationuser-update.md)|[educationUser](../resources/educationUser.md)|Update the properties of a [educationUser](../resources/educationuser.md) object.|
|[List schools](../api/educationuser-list-schools.md)|[educationSchool](../resources/educationSchool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationuser-post-schools.md)|[educationSchool](../resources/educationSchool.md)|Create schools by posting to the schools collection.|
|[List classes](../api/educationuser-list-classes.md)|[educationClass](../resources/educationClass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationuser-post-classes.md)|[educationClass](../resources/educationClass.md)|Create classes by posting to the classes collection.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedLicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedPlan.md) collection||
|businessPhones|String collection||
|createdBy|[identitySet](../resources/identitySet.md)||
|department|String||
|displayName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|mail|String||
|mailingAddress|[physicalAddress](../resources/physicalAddress.md)||
|mailNickname|String||
|middleName|String||
|mobilePhone|String||
|officeLocation|String||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordProfile.md)||
|preferredLanguage|String||
|primaryRole|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`.|
|provisionedPlans|[provisionedPlan](../resources/provisionedPlan.md) collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|residenceAddress|[physicalAddress](../resources/physicalAddress.md)||
|showInAddressList|Boolean||
|student|[educationStudent](../resources/educationStudent.md)||
|surname|String||
|teacher|[educationTeacher](../resources/educationTeacher.md)||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|classes|[educationClass](../resources/educationClass.md) collection||
|schools|[educationSchool](../resources/educationSchool.md) collection||
|user|[user](../resources/user.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "String (identifier)",
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "String",
    "countryOrRegion": "String"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent",
    "graduationYear": "String",
    "grade": "String",
    "birthDate": "Date",
    "gender": "String",
    "studentNumber": "String",
    "externalId": "String"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "String"
  },
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
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "businessPhones": [
    "String"
  ],
  "department": "String",
  "displayName": "String",
  "givenName": "String",
  "mail": "String",
  "mailNickname": "String",
  "mobilePhone": "String",
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "showInAddressList": true,
  "surname": "String",
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```

