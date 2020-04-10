---
title: "user: reprocessLicenseAssignment"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# reprocessLicenseAssignment

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
POST /me/reprocessLicenseAssignment
POST /users/{usersId}/reprocessLicenseAssignment
POST /me/managedDevices/{managedDeviceId}/users/{userId}/reprocessLicenseAssignment
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [user](../resources/user.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_reprocesslicenseassignment"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/reprocessLicenseAssignment
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4448

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "def2f845-f845-def2-45f8-f2de45f8f2de",
    "deletedDateTime": "2017-01-01T00:01:42.7296606+00:00",
    "signInActivity": {
      "@odata.type": "microsoft.graph.signInActivity"
    },
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
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "creationType": "Creation Type value",
    "department": "Department value",
    "deviceKeys": [
      {
        "@odata.type": "microsoft.graph.deviceKey"
      }
    ],
    "displayName": "Display Name value",
    "employeeId": "Employee Id value",
    "faxNumber": "Fax Number value",
    "givenName": "Given Name value",
    "identities": [
      {
        "@odata.type": "microsoft.graph.objectIdentity"
      }
    ],
    "imAddresses": [
      "Im Addresses value"
    ],
    "isResourceAccount": true,
    "jobTitle": "Job Title value",
    "lastPasswordChangeDateTime": "2016-12-31T23:58:37.4242739+00:00",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:02:42.7451887+00:00",
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
    "preferredDataLocation": "Preferred Data Location value",
    "preferredLanguage": "Preferred Language value",
    "provisionedPlans": [
      {
        "@odata.type": "microsoft.graph.provisionedPlan"
      }
    ],
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "refreshTokensValidFromDateTime": "2017-01-01T00:03:14.1936431+00:00",
    "showInAddressList": true,
    "signInSessionsValidFromDateTime": "2016-12-31T23:59:52.3274921+00:00",
    "state": "State value",
    "streetAddress": "Street Address value",
    "surname": "Surname value",
    "usageLocation": "Usage Location value",
    "userPrincipalName": "User Principal Name value",
    "externalUserState": "External User State value",
    "externalUserStateChangeDateTime": "External User State Change Date Time value",
    "userType": "User Type value",
    "mailboxSettings": {
      "@odata.type": "microsoft.graph.mailboxSettings"
    },
    "identityUserRisk": {
      "@odata.type": "microsoft.graph.identityUserRisk"
    },
    "deviceEnrollmentLimit": 5,
    "aboutMe": "About Me value",
    "birthday": "2017-01-01T00:00:04.2178204+00:00",
    "hireDate": "2016-12-31T23:59:17.7591763+00:00",
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

