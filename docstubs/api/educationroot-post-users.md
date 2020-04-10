---
title: "Add users"
description: "Add users by posting to the users collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add users

Namespace: microsoft.graph

Add users by posting to the users collection.

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
POST /education/users/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationUser](../resources/educationuser.md) object.

The following table shows the properties that are required when you create the [educationUser](../resources/educationuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|relatedContacts|[relatedContact](../resources/relatedcontact.md) collection||
|primaryRole|Enumeration| Possible values are: `student`, `teacher`, `none`, `unknownFutureValue`, `faculty`.|
|middleName|String||
|externalSource|Enumeration| Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|residenceAddress|[physicalAddress](../resources/physicaladdress.md)||
|mailingAddress|[physicalAddress](../resources/physicaladdress.md)||
|student|[educationStudent](../resources/educationstudent.md)||
|teacher|[educationTeacher](../resources/educationteacher.md)||
|createdBy|[identitySet](../resources/identityset.md)||
|accountEnabled|Boolean||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|department|String||
|displayName|String||
|givenName|String||
|mail|String||
|mailNickname|String||
|mobilePhone|String||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)||
|officeLocation|String||
|preferredLanguage|String||
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|showInAddressList|Boolean||
|surname|String||
|usageLocation|String||
|userPrincipalName|String||
|userType|String||
|onPremisesInfo|[educationOnPremisesInfo](../resources/educationonpremisesinfo.md)||



## Response
If successful, this method returns a `201 Created` response code and a [educationUser](../resources/educationuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/users
Content-type: application/json
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
        "360c11c0-11c0-360c-c011-0c36c0110c36"
      ],
      "skuId": "860ff1b8-f1b8-860f-b8f1-0f86b8f10f86"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:02:08.3128832+00:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "439cd6b6-d6b6-439c-b6d6-9c43b6d69c43"
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
  "refreshTokensValidFromDateTime": "2017-01-01T00:03:14.1936431+00:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationuser"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3429

{
  "@odata.type": "#microsoft.graph.educationUser",
  "id": "a1e95679-5679-a1e9-7956-e9a17956e9a1",
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
        "360c11c0-11c0-360c-c011-0c36c0110c36"
      ],
      "skuId": "860ff1b8-f1b8-860f-b8f1-0f86b8f10f86"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:02:08.3128832+00:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "439cd6b6-d6b6-439c-b6d6-9c43b6d69c43"
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
  "refreshTokensValidFromDateTime": "2017-01-01T00:03:14.1936431+00:00",
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

