---
title: "Get user"
description: "Read properties and relationships of the user object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get user

Namespace: microsoft.graph

Read properties and relationships of the [user](../resources/user.md) object.

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
GET /me
GET /users/{usersId}
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
If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/beta/me
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
Content-Length: 6701

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "ea56017e-017e-ea56-7e01-56ea7e0156ea",
    "deletedDateTime": "2017-01-01T00:03:00.2666497+00:00",
    "accountEnabled": true,
    "ageGroup": "Age Group value",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense",
        "disabledPlans": [
          "bd180a63-0a63-bd18-630a-18bd630a18bd"
        ],
        "skuId": "6130b7f7-b7f7-6130-f7b7-3061f7b73061"
      }
    ],
    "assignedPlans": [
      {
        "@odata.type": "microsoft.graph.assignedPlan",
        "assignedDateTime": "2017-01-01T00:02:35.836838+00:00",
        "capabilityStatus": "Capability Status value",
        "service": "Service value",
        "servicePlanId": "5e0ed8cd-d8cd-5e0e-cdd8-0e5ecdd80e5e"
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
    "lastPasswordChangeDateTime": "2016-12-31T23:59:37.5898695+00:00",
    "legalAgeGroupClassification": "Legal Age Group Classification value",
    "licenseAssignmentStates": [
      {
        "@odata.type": "microsoft.graph.licenseAssignmentState",
        "assignedByGroup": "Assigned By Group value",
        "state": "State value",
        "error": "Error value"
      }
    ],
    "mail": "Mail value",
    "mailNickname": "Mail Nickname value",
    "mobilePhone": "Mobile Phone value",
    "onPremisesDistinguishedName": "On Premises Distinguished Name value",
    "onPremisesExtensionAttributes": {
      "@odata.type": "microsoft.graph.onPremisesExtensionAttributes",
      "extensionAttribute1": "Extension Attribute1 value",
      "extensionAttribute2": "Extension Attribute2 value",
      "extensionAttribute3": "Extension Attribute3 value",
      "extensionAttribute4": "Extension Attribute4 value",
      "extensionAttribute5": "Extension Attribute5 value",
      "extensionAttribute6": "Extension Attribute6 value",
      "extensionAttribute7": "Extension Attribute7 value",
      "extensionAttribute8": "Extension Attribute8 value",
      "extensionAttribute9": "Extension Attribute9 value",
      "extensionAttribute10": "Extension Attribute10 value",
      "extensionAttribute11": "Extension Attribute11 value",
      "extensionAttribute12": "Extension Attribute12 value",
      "extensionAttribute13": "Extension Attribute13 value",
      "extensionAttribute14": "Extension Attribute14 value",
      "extensionAttribute15": "Extension Attribute15 value"
    },
    "onPremisesImmutableId": "On Premises Immutable Id value",
    "onPremisesLastSyncDateTime": "2016-12-31T23:59:08.2684686+00:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:57:07.3788647+00:00"
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
      "@odata.type": "microsoft.graph.passwordProfile",
      "password": "Password value",
      "forceChangePasswordNextSignIn": true,
      "forceChangePasswordNextSignInWithMfa": true
    },
    "officeLocation": "Office Location value",
    "postalCode": "Postal Code value",
    "preferredLanguage": "Preferred Language value",
    "provisionedPlans": [
      {
        "@odata.type": "microsoft.graph.provisionedPlan",
        "provisioningStatus": "Provisioning Status value"
      }
    ],
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "showInAddressList": true,
    "signInSessionsValidFromDateTime": "2017-01-01T00:02:25.5716028+00:00",
    "state": "State value",
    "streetAddress": "Street Address value",
    "surname": "Surname value",
    "usageLocation": "Usage Location value",
    "userPrincipalName": "User Principal Name value",
    "userType": "User Type value",
    "mailboxSettings": {
      "@odata.type": "microsoft.graph.mailboxSettings",
      "automaticRepliesSetting": {
        "@odata.type": "microsoft.graph.automaticRepliesSetting",
        "status": "String",
        "externalAudience": "String",
        "scheduledStartDateTime": {
          "@odata.type": "microsoft.graph.dateTimeTimeZone",
          "dateTime": "Date Time value",
          "timeZone": "Time Zone value"
        },
        "scheduledEndDateTime": {
          "@odata.type": "microsoft.graph.dateTimeTimeZone"
        },
        "internalReplyMessage": "Internal Reply Message value",
        "externalReplyMessage": "External Reply Message value"
      },
      "archiveFolder": "Archive Folder value",
      "language": {
        "@odata.type": "microsoft.graph.localeInfo",
        "locale": "Locale value"
      },
      "workingHours": {
        "@odata.type": "microsoft.graph.workingHours",
        "daysOfWeek": [
          "String"
        ],
        "startTime": "11:59:04.6360000",
        "endTime": "12:00:44.4630000",
        "timeZone": {
          "@odata.type": "microsoft.graph.timeZoneBase",
          "name": "Name value"
        }
      },
      "dateFormat": "Date Format value",
      "timeFormat": "Time Format value"
    },
    "deviceEnrollmentLimit": 5,
    "aboutMe": "About Me value",
    "birthday": "2016-12-31T23:58:38.0220892+00:00",
    "hireDate": "2016-12-31T23:57:20.4054175+00:00",
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

