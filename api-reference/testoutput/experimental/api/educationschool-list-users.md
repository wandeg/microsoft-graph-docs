---
title: "List users"
description: "Get the educationUsers from the users navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List users

Namespace: microsoft.graph

Get the educationUsers from the users navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/users
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/users
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationuser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3890

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "b1002e7a-2e7a-b100-7a2e-00b17a2e00b1",
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
            "3c38c39b-c39b-3c38-9bc3-383c9bc3383c"
          ],
          "skuId": "25470e04-0e04-2547-040e-4725040e4725"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:56:36.9997901+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "430099a8-99a8-4300-a899-0043a8990043"
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:59:47.8427372+03:00",
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
  ]
}
```

