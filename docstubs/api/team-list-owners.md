---
title: "List owners"
description: "Get the users from the owners navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List owners

Namespace: microsoft.graph

Get the users from the owners navigation property.

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
GET /teams/{teamsId}/owners
GET /me/joinedGroups/{groupId}/team/owners
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
GET https://graph.microsoft.com/beta/teams/{teamsId}/owners
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
      "id": "eb39667f-667f-eb39-7f66-39eb7f6639eb",
      "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
      "signInActivity": {
        "@odata.type": "microsoft.graph.signInActivity",
        "lastSignInDateTime": "2016-12-31T23:58:41.2687271+03:00",
        "lastSignInRequestId": "Last Sign In Request Id value"
      },
      "accountEnabled": true,
      "ageGroup": "Age Group value",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "a7670532-0532-a767-3205-67a7320567a7"
          ],
          "skuId": "5e903406-3406-5e90-0634-905e0634905e"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2017-01-01T00:03:00.2256577+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "c7e63634-3634-c7e6-3436-e6c73436e6c7"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "companyName": "Company Name value",
      "consentProvidedForMinor": "Consent Provided For Minor value",
      "country": "Country value",
      "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
      "creationType": "Creation Type value",
      "department": "Department value",
      "deviceKeys": [
        {
          "@odata.type": "microsoft.graph.deviceKey",
          "keyType": "Key Type value",
          "keyMaterial": "a2V5TWF0ZXJpYWw=",
          "deviceId": "f4be8a66-8a66-f4be-668a-bef4668abef4"
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
      "lastPasswordChangeDateTime": "2016-12-31T23:58:57.697114+03:00",
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
      "onPremisesLastSyncDateTime": "2016-12-31T23:59:58.9687424+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2016-12-31T23:57:55.1037507+03:00"
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
      "refreshTokensValidFromDateTime": "2016-12-31T23:57:26.2095535+03:00",
      "showInAddressList": true,
      "signInSessionsValidFromDateTime": "2016-12-31T23:59:30.1824608+03:00",
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
          "startTime": "12:01:03.5830000",
          "endTime": "12:00:51.9520000",
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
        "lastChangedDateTime": "2017-01-01T00:02:40.0833773+03:00"
      },
      "deviceEnrollmentLimit": 5,
      "aboutMe": "About Me value",
      "birthday": "2016-12-31T23:59:46.3060075+03:00",
      "hireDate": "2016-12-31T23:58:42.5495433+03:00",
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

