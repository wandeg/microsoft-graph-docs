---
title: "assignLicense"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# assignLicense

Namespace: microsoft.graph



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
POST /me/assignLicense
POST /users/{usersId}/assignLicense
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|addLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|removeLicenses|Guid collection||



## Response
If successful, this action returns a `200 OK` response code and a [user](../resources/user.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "user_assignlicense"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/assignLicense

Content-type: application/json
Content-length: 172

{
  "addLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "removeLicenses": [
    "5a54272e-272e-5a54-2e27-545a2e27545a"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3680

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "11c1470d-470d-11c1-0d47-c1110d47c111",
    "deletedDateTime": "2016-12-31T23:57:00.4445976+03:00",
    "accountEnabled": true,
    "ageGroup": "Age Group value",
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
      "Business Phones value"
    ],
    "city": "City value",
    "companyName": "Company Name value",
    "consentProvidedForMinor": "Consent Provided For Minor value",
    "country": "Country value",
    "department": "Department value",
    "displayName": "Display Name value",
    "employeeId": "Employee Id value",
    "faxNumber": "Fax Number value",
    "givenName": "Given Name value",
    "imAddresses": [
      "Im Addresses value"
    ],
    "isResourceAccount": true,
    "jobTitle": "Job Title value",
    "lastPasswordChangeDateTime": "2016-12-31T23:58:49.4033387+03:00",
    "legalAgeGroupClassification": "Legal Age Group Classification value",
    "licenseAssignmentStates": [
      {
        "@odata.type": "microsoft.graph.licenseAssignmentState"
      }
    ],
    "mail": "Mail value",
    "mailNickname": "Mail Nickname value",
    "mobilePhone": "Mobile Phone value",
    "onPremisesDistinguishedName": "On Premises Distinguished Name value",
    "onPremisesExtensionAttributes": {
      "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
    },
    "onPremisesImmutableId": "On Premises Immutable Id value",
    "onPremisesLastSyncDateTime": "2017-01-01T00:00:06.2458912+03:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError"
      }
    ],
    "onPremisesSecurityIdentifier": "On Premises Security Identifier value",
    "onPremisesSyncEnabled": true,
    "onPremisesDomainName": "On Premises Domain Name value",
    "onPremisesSamAccountName": "On Premises Sam Account Name value",
    "onPremisesUserPrincipalName": "On Premises User Principal Name value",
    "otherMails": [
      "Other Mails value"
    ],
    "passwordPolicies": "Password Policies value",
    "passwordProfile": {
      "@odata.type": "microsoft.graph.passwordProfile"
    },
    "officeLocation": "Office Location value",
    "postalCode": "Postal Code value",
    "preferredLanguage": "Preferred Language value",
    "provisionedPlans": [
      {
        "@odata.type": "microsoft.graph.provisionedPlan"
      }
    ],
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "showInAddressList": true,
    "signInSessionsValidFromDateTime": "2016-12-31T23:57:49.5155549+03:00",
    "state": "State value",
    "streetAddress": "Street Address value",
    "surname": "Surname value",
    "usageLocation": "Usage Location value",
    "userPrincipalName": "User Principal Name value",
    "userType": "User Type value",
    "mailboxSettings": {
      "@odata.type": "microsoft.graph.mailboxSettings"
    },
    "deviceEnrollmentLimit": 5,
    "aboutMe": "About Me value",
    "birthday": "2017-01-01T00:03:29.4887116+03:00",
    "hireDate": "2016-12-31T23:59:16.1341104+03:00",
    "interests": [
      "Interests value"
    ],
    "mySite": "My Site value",
    "pastProjects": [
      "Past Projects value"
    ],
    "preferredName": "Preferred Name value",
    "responsibilities": [
      "Responsibilities value"
    ],
    "schools": [
      "Schools value"
    ],
    "skills": [
      "Skills value"
    ]
  }
}
```

