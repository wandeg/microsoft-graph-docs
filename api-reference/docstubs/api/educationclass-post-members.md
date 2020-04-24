---
title: "Add members"
description: "Add members by posting to the members collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add members

Namespace: microsoft.graph

Add members by posting to the members collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /education/classes/{educationClassId}/members/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationUser](../resources/educationuser.md) object.

The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|relatedContacts|[relatedContact](../resources/relatedcontact.md) collection|**TODO: Add Description**|
|primaryRole|educationUserRole|**TODO: Add Description**. Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|middleName|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|student|[educationStudent](../resources/educationstudent.md)|**TODO: Add Description**|
|teacher|[educationTeacher](../resources/educationteacher.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|accountEnabled|Boolean|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|refreshTokensValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|
|onPremisesInfo|[educationOnPremisesInfo](../resources/educationonpremisesinfo.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and an [educationUser](../resources/educationuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/$ref
Content-Type: application/json
Content-length: 3380

{
  "@odata.type": "#microsoft.graph.educationUser",
  "relatedContacts": [
    {
      "@odata.type": "microsoft.graph.relatedContact",
      "id": "Id value",
      "displayName": "Display Name value",
      "emailAddress": "Email Address value",
      "mobilePhone": "Mobile Phone value",
      "relationship": "String",
      "accessConsent": true
    }
  ],
  "primaryRole": "String",
  "middleName": "Middle Name value",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "Post Office Box value",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent",
    "graduationYear": "Graduation Year value",
    "grade": "Grade value",
    "birthDate": "Date",
    "gender": "String",
    "studentNumber": "Student Number value",
    "externalId": "External Id value"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "Teacher Number value"
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
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "4dd31bf7-1bf7-4dd3-f71b-d34df71bd34d"
      ],
      "skuId": "747ec031-c031-747e-31c0-7e7431c07e74"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2016-12-31T23:56:57.6905634+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "ba5fb184-b184-ba5f-84b1-5fba84b15fba"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "mobilePhone": "Mobile Phone value",
  "passwordPolicies": "Password Policies value",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "Password value",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "Office Location value",
  "preferredLanguage": "Preferred Language value",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "refreshTokensValidFromDateTime": "2017-01-01T00:02:34.0512177+03:00",
  "showInAddressList": true,
  "surname": "Surname value",
  "usageLocation": "Usage Location value",
  "userPrincipalName": "User Principal Name value",
  "userType": "User Type value",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo",
    "immutableId": "Immutable Id value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationuser"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "bb09b26a-b26a-bb09-6ab2-09bb6ab209bb",
  "relatedContacts": [
    {
      "@odata.type": "microsoft.graph.relatedContact",
      "id": "Id value",
      "displayName": "Display Name value",
      "emailAddress": "Email Address value",
      "mobilePhone": "Mobile Phone value",
      "relationship": "String",
      "accessConsent": true
    }
  ],
  "primaryRole": "String",
  "middleName": "Middle Name value",
  "externalSource": "String",
  "residenceAddress": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "Post Office Box value",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "postalCode": "Postal Code value"
  },
  "mailingAddress": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "student": {
    "@odata.type": "microsoft.graph.educationStudent",
    "graduationYear": "Graduation Year value",
    "grade": "Grade value",
    "birthDate": "Date",
    "gender": "String",
    "studentNumber": "Student Number value",
    "externalId": "External Id value"
  },
  "teacher": {
    "@odata.type": "microsoft.graph.educationTeacher",
    "teacherNumber": "Teacher Number value"
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
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "4dd31bf7-1bf7-4dd3-f71b-d34df71bd34d"
      ],
      "skuId": "747ec031-c031-747e-31c0-7e7431c07e74"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2016-12-31T23:56:57.6905634+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "ba5fb184-b184-ba5f-84b1-5fba84b15fba"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "department": "Department value",
  "displayName": "Display Name value",
  "givenName": "Given Name value",
  "mail": "Mail value",
  "mailNickname": "Mail Nickname value",
  "mobilePhone": "Mobile Phone value",
  "passwordPolicies": "Password Policies value",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile",
    "password": "Password value",
    "forceChangePasswordNextSignIn": true,
    "forceChangePasswordNextSignInWithMfa": true
  },
  "officeLocation": "Office Location value",
  "preferredLanguage": "Preferred Language value",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan",
      "provisioningStatus": "Provisioning Status value"
    }
  ],
  "refreshTokensValidFromDateTime": "2017-01-01T00:02:34.0512177+03:00",
  "showInAddressList": true,
  "surname": "Surname value",
  "usageLocation": "Usage Location value",
  "userPrincipalName": "User Principal Name value",
  "userType": "User Type value",
  "onPremisesInfo": {
    "@odata.type": "microsoft.graph.educationOnPremisesInfo",
    "immutableId": "Immutable Id value"
  }
}
```

