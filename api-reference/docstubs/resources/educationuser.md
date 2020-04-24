---
title: "educationUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationUser resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationUser](../api/educationuser-get.md)|[educationUser](../resources/educationuser.md)|Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.|
|[Update educationUser](../api/educationuser-update.md)|[educationUser](../resources/educationuser.md)|Update the properties of an [educationUser](../resources/educationuser.md) object.|
|[delta](../api/educationuser-delta.md)|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|
|[List assignments](../api/educationuser-list-assignments.md)|[educationAssignment](../resources/educationassignment.md) collection|Get the educationAssignments from the assignments navigation property.|
|[Create assignments](../api/educationuser-post-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Create a new assignments object.|
|[Delete assignments](../api/educationuser-delete-assignments.md)|None|Delete an [educationAssignment](../resources/educationassignment.md) object.|
|[Update assignments](../api/educationuser-update-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Update the properties of an assignments object.|
|[Get educationAssignment](../api/educationassignment-get.md)|[educationAssignment](../resources/educationassignment.md)|Read the properties and relationships of an [educationAssignment](../resources/educationassignment.md) object.|
|[List rubrics](../api/educationuser-list-rubrics.md)|[educationRubric](../resources/educationrubric.md) collection|Get the educationRubrics from the rubrics navigation property.|
|[Create rubrics](../api/educationuser-post-rubrics.md)|[educationRubric](../resources/educationrubric.md)|Create a new rubrics object.|
|[Delete rubrics](../api/educationuser-delete-rubrics.md)|None|Delete a [educationRubric](../resources/educationrubric.md) object.|
|[Update rubrics](../api/educationuser-update-rubrics.md)|[educationRubric](../resources/educationrubric.md)|Update the properties of a rubrics object.|
|[Get educationRubric](../api/educationrubric-get.md)|[educationRubric](../resources/educationrubric.md)|Read the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.|
|[List classes](../api/educationuser-list-classes.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the classes navigation property.|
|[Add classes](../api/educationuser-post-classes.md)|[educationClass](../resources/educationclass.md)|Add classes by posting to the classes collection.|
|[Remove classes](../api/educationuser-delete-classes.md)|None|Remove a [educationClass](../resources/educationclass.md) object.|
|[List taughtClasses](../api/educationuser-list-taughtclasses.md)|[educationClass](../resources/educationclass.md) collection|Get the educationClasses from the taughtClasses navigation property.|
|[Add taughtClasses](../api/educationuser-post-taughtclasses.md)|[educationClass](../resources/educationclass.md)|Add taughtClasses by posting to the taughtClasses collection.|
|[Remove taughtClasses](../api/educationuser-delete-taughtclasses.md)|None|Remove a [educationClass](../resources/educationclass.md) object.|
|[List schools](../api/educationuser-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchools from the schools navigation property.|
|[Add schools](../api/educationuser-post-schools.md)|[educationSchool](../resources/educationschool.md)|Add schools by posting to the schools collection.|
|[Remove schools](../api/educationuser-delete-schools.md)|None|Remove a [educationSchool](../resources/educationschool.md) object.|
|[List user](../api/educationuser-list-user.md)|[user](../resources/user.md) collection|Get the users from the user navigation property.|
|[Add user](../api/educationuser-post-user.md)|[user](../resources/user.md)|Add user by posting to the user collection.|
|[Remove user](../api/educationuser-delete-user.md)|None|Remove a [user](../resources/user.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountEnabled|Boolean|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|givenName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|mail|String|**TODO: Add Description**|
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|middleName|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|onPremisesInfo|[educationOnPremisesInfo](../resources/educationonpremisesinfo.md)|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|primaryRole|educationUserRole|**TODO: Add Description**. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|refreshTokensValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|relatedContacts|[relatedContact](../resources/relatedcontact.md) collection|**TODO: Add Description**|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|student|[educationStudent](../resources/educationstudent.md)|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|teacher|[educationTeacher](../resources/educationteacher.md)|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[educationAssignment](../resources/educationassignment.md) collection|**TODO: Add Description**|
|classes|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|rubrics|[educationRubric](../resources/educationrubric.md) collection|**TODO: Add Description**|
|schools|[educationSchool](../resources/educationschool.md) collection|**TODO: Add Description**|
|taughtClasses|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|user|[user](../resources/user.md)|**TODO: Add Description**|

## JSON representation
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
      "emailAddress": "String",
      "mobilePhone": "String",
      "relationship": "String",
      "accessConsent": true
    }
  ],
  "primaryRole": "String",
  "middleName": "String",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
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
    "studentNumber": "String"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "String"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "accountEnabled": true,
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "Guid"
      ],
      "skuId": "Guid"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "String (timestamp)",
      "capabilityStatus": "String",
      "service": "String",
      "servicePlanId": "Guid"
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
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "String",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "String",
  "preferredLanguage": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "String"
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

