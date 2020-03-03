---
title: "educationUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationUsers](../api/educationuser-list.md)|[educationUser](../resources/educationuser.md) collection|List properties and relationships of the [educationUser](../resources/educationuser.md) objects.|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationuser.md)|Read properties and relationships of the [educationUser](../resources/educationuser.md) object.|
|[Create educationUser](../api/educationuser-create.md)|[educationUser](../resources/educationuser.md)|Create a new [educationUser](../resources/educationuser.md) object.|
|[Delete educationUser](../api/educationuser-delete.md)|None|Deletes a [educationUser](../resources/educationuser.md).|
|[Update educationUser](../api/educationuser-update.md)|[educationUser](../resources/educationuser.md)|Update the properties of a [educationUser](../resources/educationuser.md) object.|
|[delta](../api/educationuser-delta.md)|[educationUser](../resources/educationuser.md) collection||
|[List assignments](../api/educationuser-list-assignments.md)|[educationAssignment](../resources/educationassignment.md) collection|Get the educationAssignments from the assignments navigation property.|
|[Add assignments](../api/educationuser-post-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Add assignments by posting to the assignments collection.|
|[List rubrics](../api/educationuser-list-rubrics.md)|[educationRubric](../resources/educationrubric.md) collection|Get the educationRubrics from the rubrics navigation property.|
|[Add rubrics](../api/educationuser-post-rubrics.md)|[educationRubric](../resources/educationrubric.md)|Add rubrics by posting to the rubrics collection.|
|[List classes](../api/educationuser-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Create classes](../api/educationuser-post-classes.md)|[educationClass](../resources/educationclass.md)|Create classes by posting to the classes collection.|
|[List taughtClasses](../api/educationuser-list-taughtclasses.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the taughtClasses navigation property.|
|[Create taughtClasses](../api/educationuser-post-taughtclasses.md)|[educationClass](../resources/educationclass.md)|Create taughtClasses by posting to the taughtClasses collection.|
|[List schools](../api/educationuser-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Create schools](../api/educationuser-post-schools.md)|[educationSchool](../resources/educationschool.md)|Create schools by posting to the schools collection.|
|[Get user](../api/user-get.md)|[user](../resources/user.md)|Read properties and relationships of the [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|createdBy|[identitySet](../resources/identityset.md)||
|department|String||
|displayName|String||
|externalSource|Enumeration|. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|givenName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|mail|String||
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)||
|mailNickname|String||
|middleName|String||
|mobilePhone|String||
|officeLocation|String||
|onPremisesInfo|[educationOnPremisesInfo](../resources/educationonpremisesinfo.md)||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)||
|preferredLanguage|String||
|primaryRole|Enumeration|. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|relatedContacts|[relatedContact](../resources/relatedcontact.md) collection||
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)||
|showInAddressList|Boolean||
|student|[educationStudent](../resources/educationstudent.md)||
|surname|String||
|teacher|[educationTeacher](../resources/educationteacher.md)||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[educationAssignment](../resources/educationassignment.md) collection||
|classes|[educationClass](../resources/educationclass.md) collection||
|rubrics|[educationRubric](../resources/educationrubric.md) collection||
|schools|[educationSchool](../resources/educationschool.md) collection||
|taughtClasses|[educationClass](../resources/educationclass.md) collection||
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
  "relatedContacts": [
    {
      "@odata.type": "microsoft.graph.relatedContact",
      "id": "String",
      "emailAddress": "String",
      "relationship": "String",
      "accessConsent": true
    }
  ],
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "String",
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
      "@odata.type": "microsoft.graph.identity"
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
  "userType": "String",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo",
    "immutableId": "String"
  }
}
```

