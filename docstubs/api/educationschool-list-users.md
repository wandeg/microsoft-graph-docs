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
GET /education/classes/{educationClassId}/schools/{educationSchoolId}/users
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
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
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/schools/{educationSchoolId}/users
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
Content-Length: 3375

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "307e8711-8711-307e-1187-7e3011877e30",
      "primaryRole": "String",
      "middleName": "Middle Name value",
      "externalSource": "String",
      "residenceAddress": {
        "@odata.type": "microsoft.graph.physicalAddress",
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
          "@odata.type": "microsoft.graph.identity",
          "displayName": "Display Name value",
          "id": "Id value"
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
            "6b350595-0595-6b35-9505-356b9505356b"
          ],
          "skuId": "801835b8-35b8-8018-b835-1880b8351880"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2017-01-01T00:03:13.0174127+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "f3074411-4411-f307-1144-07f3114407f3"
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:59:30.0072379+03:00",
      "showInAddressList": true,
      "surname": "Surname value",
      "usageLocation": "Usage Location value",
      "userPrincipalName": "User Principal Name value",
      "userType": "User Type value"
    }
  ]
}
```

