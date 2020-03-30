---
title: "Create teachers"
description: "Create teachers by posting to the teachers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create teachers

Namespace: microsoft.graph

Create teachers by posting to the teachers collection.

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
POST /education/classes/{educationClassId}/teachers/$ref
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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/teachers
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
        "0da5f7be-f7be-0da5-bef7-a50dbef7a50d"
      ],
      "skuId": "66647408-7408-6664-0874-646608746466"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:48.5840397+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "d07e23bc-23bc-d07e-bc23-7ed0bc237ed0"
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
  "refreshTokensValidFromDateTime": "2016-12-31T23:56:55.8992192+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "0f9c9d0c-9d0c-0f9c-0c9d-9c0f0c9d9c0f",
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
        "0da5f7be-f7be-0da5-bef7-a50dbef7a50d"
      ],
      "skuId": "66647408-7408-6664-0874-646608746466"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:48.5840397+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "d07e23bc-23bc-d07e-bc23-7ed0bc237ed0"
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
  "refreshTokensValidFromDateTime": "2016-12-31T23:56:55.8992192+03:00",
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

