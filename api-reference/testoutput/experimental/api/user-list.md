---
title: "List users"
description: "List properties and relationships of the user objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List users

Namespace: microsoft.graph

List properties and relationships of the [user](../resources/user.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/managedDevices/{managedDeviceId}/users
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/managedDevices/{managedDeviceId}/users
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
Content-Length: 8458

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "a6723cb8-3cb8-a672-b83c-72a6b83c72a6",
      "deletedDateTime": "2017-01-01T00:00:12.2826741+03:00",
      "signInActivity": {
        "@odata.type": "microsoft.graph.signInActivity",
        "lastSignInDateTime": "2017-01-01T00:00:44.698105+03:00",
        "lastSignInRequestId": "Last Sign In Request Id value"
      },
      "accountEnabled": true,
      "ageGroup": "Age Group value",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "d28f3feb-3feb-d28f-eb3f-8fd2eb3f8fd2"
          ],
          "skuId": "766f47e4-47e4-766f-e447-6f76e4476f76"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:58:09.350506+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "2f12abad-abad-2f12-adab-122fadab122f"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "companyName": "Company Name value",
      "consentProvidedForMinor": "Consent Provided For Minor value",
      "country": "Country value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "creationType": "Creation Type value",
      "department": "Department value",
      "deviceKeys": [
        {
          "@odata.type": "microsoft.graph.deviceKey",
          "keyType": "Key Type value",
          "keyMaterial": "a2V5TWF0ZXJpYWw=",
          "deviceId": "688189fe-89fe-6881-fe89-8168fe898168"
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
      "lastPasswordChangeDateTime": "2016-12-31T23:57:01.5811029+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:58:26.0302388+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2017-01-01T00:00:02.4393137+03:00"
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:56:54.306584+03:00",
      "showInAddressList": true,
      "signInSessionsValidFromDateTime": "2017-01-01T00:01:26.7367124+03:00",
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
          "startTime": "12:02:50.6370000",
          "endTime": "12:02:54.9570000",
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
        "lastChangedDateTime": "2016-12-31T23:58:16.6283733+03:00"
      },
      "deviceEnrollmentLimit": 5,
      "aboutMe": "About Me value",
      "birthday": "2017-01-01T00:01:02.2766982+03:00",
      "hireDate": "2017-01-01T00:03:11.1185624+03:00",
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

