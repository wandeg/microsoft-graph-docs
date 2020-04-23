---
title: "List members"
description: "Get the educationUsers from the members navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List members

Namespace: microsoft.graph

Get the educationUsers from the members navigation property.

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
GET /education/classes/{educationClassId}/members
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
If successful, this method returns a `200 OK` response code and a collection of [educationUser](../resources/educationuser.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/members
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationuser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationUser",
      "id": "096d79c0-79c0-096d-c079-6d09c0796d09",
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
            "354f28a6-28a6-354f-a628-4f35a6284f35"
          ],
          "skuId": "8d3d7251-7251-8d3d-5172-3d8d51723d8d"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:56:42.7834953+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "09f08a83-8a83-09f0-838a-f009838af009"
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:59:22.7578051+03:00",
      "showInAddressList": true,
      "surname": "Surname value",
      "usageLocation": "Usage Location value",
      "userPrincipalName": "User Principal Name value",
      "userType": "User Type value"
    }
  ]
}
```

