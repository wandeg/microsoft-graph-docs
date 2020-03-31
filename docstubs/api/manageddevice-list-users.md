---
title: "List users"
description: "Get the users from the users navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List users

Namespace: microsoft.graph

Get the users from the users navigation property.

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
GET /me/managedDevices/{managedDeviceId}/users
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
If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/users
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8461

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "b3809e16-9e16-b380-169e-80b3169e80b3",
      "deletedDateTime": "2016-12-31T23:59:31.2455853+03:00",
      "signInActivity": {
        "@odata.type": "microsoft.graph.signInActivity",
        "lastSignInDateTime": "2017-01-01T00:00:53.7541608+03:00",
        "lastSignInRequestId": "Last Sign In Request Id value"
      },
      "accountEnabled": true,
      "ageGroup": "Age Group value",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "23bcc8f3-c8f3-23bc-f3c8-bc23f3c8bc23"
          ],
          "skuId": "728dbca0-bca0-728d-a0bc-8d72a0bc8d72"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2017-01-01T00:03:20.114256+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "4a8ded43-ed43-4a8d-43ed-8d4a43ed8d4a"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "companyName": "Company Name value",
      "consentProvidedForMinor": "Consent Provided For Minor value",
      "country": "Country value",
      "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
      "creationType": "Creation Type value",
      "department": "Department value",
      "deviceKeys": [
        {
          "@odata.type": "microsoft.graph.deviceKey",
          "keyType": "Key Type value",
          "keyMaterial": "a2V5TWF0ZXJpYWw=",
          "deviceId": "3f2de8e9-e8e9-3f2d-e9e8-2d3fe9e82d3f"
        }
      ],
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
      "lastPasswordChangeDateTime": "2016-12-31T23:59:06.0219826+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:58:50.4582097+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:58:07.4517849+03:00"
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
      "preferredDataLocation": "Preferred Data Location value",
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:56:52.8080157+03:00",
      "showInAddressList": true,
      "signInSessionsValidFromDateTime": "2017-01-01T00:00:32.7035815+03:00",
      "state": "State value",
      "streetAddress": "Street Address value",
      "surname": "Surname value",
      "usageLocation": "Usage Location value",
      "userPrincipalName": "User Principal Name value",
      "externalUserState": "External User State value",
      "externalUserStateChangeDateTime": "External User State Change Date Time value",
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
          "startTime": "11:57:52.0820000",
          "endTime": "11:57:36.0600000",
          "timeZone": {
            "@odata.type": "microsoft.graph.timeZoneBase",
            "name": "Name value"
          }
        },
        "dateFormat": "Date Format value",
        "timeFormat": "Time Format value"
      },
      "identityUserRisk": {
        "@odata.type": "microsoft.graph.identityUserRisk",
        "level": "String",
        "lastChangedDateTime": "2016-12-31T23:56:24.4471189+03:00"
      },
      "deviceEnrollmentLimit": 5,
      "aboutMe": "About Me value",
      "birthday": "2017-01-01T00:01:20.4229096+03:00",
      "hireDate": "2016-12-31T23:58:48.1976292+03:00",
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
  ]
}
```

