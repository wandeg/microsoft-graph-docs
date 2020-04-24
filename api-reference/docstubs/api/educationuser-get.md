---
title: "Get educationUser"
description: "Read the properties and relationships of an educationUser object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationUser

Namespace: microsoft.graph

Read the properties and relationships of an [educationUser](../resources/educationuser.md) object.

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
GET /education/me
GET /education/users/{educationUserId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [educationUser](../resources/educationuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/me
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

