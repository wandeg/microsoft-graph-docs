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
GET https://graph.microsoft.com/v1.0/me
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
Content-Length: 7040

{
  "value": {
    "@odata.type": "#microsoft.graph.user",
    "id": "df8ee5e4-e5e4-df8e-e4e5-8edfe4e58edf",
    "deletedDateTime": "2016-12-31T23:57:17.775585+00:00",
    "accountEnabled": true,
    "ageGroup": "Age Group value",
    "assignedLicenses": [
      {
        "@odata.type": "microsoft.graph.assignedLicense",
        "disabledPlans": [
          "d7e7e684-e684-d7e7-84e6-e7d784e6e7d7"
        ],
        "skuId": "52c0ce4f-ce4f-52c0-4fce-c0524fcec052"
      }
    ],
    "assignedPlans": [
      {
        "@odata.type": "microsoft.graph.assignedPlan",
        "assignedDateTime": "2016-12-31T23:56:41.5651918+00:00",
        "capabilityStatus": "Capability Status value",
        "service": "Service value",
        "servicePlanId": "ef35ab56-ab56-ef35-56ab-35ef56ab35ef"
      }
    ],
    "businessPhones": [
      "Business Phones value"
    ],
    "city": "City value",
    "companyName": "Company Name value",
    "consentProvidedForMinor": "Consent Provided For Minor value",
    "country": "Country value",
    "creationType": "Creation Type value",
    "department": "Department value",
    "displayName": "Display Name value",
    "employeeId": "Employee Id value",
    "faxNumber": "Fax Number value",
    "givenName": "Given Name value",
    "identities": [
      {
        "@odata.type": "microsoft.graph.objectIdentity",
        "signInType": "Sign In Type value",
        "issuer": "Issuer value",
        "issuerAssignedId": "Issuer Assigned Id value"
      }
    ],
    "imAddresses": [
      "Im Addresses value"
    ],
    "isResourceAccount": true,
    "jobTitle": "Job Title value",
    "lastPasswordChangeDateTime": "2017-01-01T00:02:38.29186+00:00",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:12.29393+00:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "microsoft.graph.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2017-01-01T00:01:07.7595324+00:00"
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
    "signInSessionsValidFromDateTime": "2016-12-31T23:57:41.9345266+00:00",
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
      "delegateMeetingMessageDeliveryOptions": "String",
      "workingHours": {
        "@odata.type": "microsoft.graph.workingHours",
        "daysOfWeek": [
          "String"
        ],
        "startTime": "12:02:13.0200000",
        "endTime": "11:59:29.6250000",
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
    "birthday": "2016-12-31T23:56:54.1307041+00:00",
    "hireDate": "2017-01-01T00:01:48.8695058+00:00",
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

