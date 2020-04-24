---
title: "List createdByUser"
description: "Get the users from the createdByUser navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List createdByUser

Namespace: microsoft.graph

Get the users from the createdByUser navigation property.

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
GET /workbooks/{workbooksId}/createdByUser
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
If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/createdByUser
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "id": "0b1b652d-652d-0b1b-2d65-1b0b2d651b0b",
      "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
      "signInActivity": {
        "@odata.type": "microsoft.graph.signInActivity",
        "lastSignInDateTime": "2017-01-01T00:02:42.0454364+03:00",
        "lastSignInRequestId": "Last Sign In Request Id value"
      },
      "accountEnabled": true,
      "ageGroup": "Age Group value",
      "assignedLicenses": [
        {
          "@odata.type": "microsoft.graph.assignedLicense",
          "disabledPlans": [
            "4dd31bf7-1bf7-4dd3-f71b-d34df71bd34d"
          ],
          "skuId": "747ec031-c031-747e-31c0-7e7431c07e74"
        }
      ],
      "assignedPlans": [
        {
          "@odata.type": "microsoft.graph.assignedPlan",
          "assignedDateTime": "2016-12-31T23:56:57.6905634+03:00",
          "capabilityStatus": "Capability Status value",
          "service": "Service value",
          "servicePlanId": "ba5fb184-b184-ba5f-84b1-5fba84b15fba"
        }
      ],
      "businessPhones": [
        "Business Phones value"
      ],
      "city": "City value",
      "companyName": "Company Name value",
      "consentProvidedForMinor": "Consent Provided For Minor value",
      "country": "Country value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "creationType": "Creation Type value",
      "department": "Department value",
      "deviceKeys": [
        {
          "@odata.type": "microsoft.graph.deviceKey",
          "keyType": "Key Type value",
          "keyMaterial": "a2V5TWF0ZXJpYWw=",
          "deviceId": "4b7bbe37-be37-4b7b-37be-7b4b37be7b4b"
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
      "lastPasswordChangeDateTime": "2016-12-31T23:56:36.317459+03:00",
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
      "onPremisesLastSyncDateTime": "2017-01-01T00:01:17.7456992+03:00",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError",
          "value": "Value value",
          "category": "Category value",
          "propertyCausingError": "Property Causing Error value",
          "occurredDateTime": "2017-01-01T00:01:31.6341616+03:00"
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
      "refreshTokensValidFromDateTime": "2017-01-01T00:02:34.0512177+03:00",
      "showInAddressList": true,
      "signInSessionsValidFromDateTime": "2017-01-01T00:02:55.6294098+03:00",
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
          "startTime": "11:58:07.5130000",
          "endTime": "11:57:24.1090000",
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
        "lastChangedDateTime": "2016-12-31T23:56:57.8486996+03:00"
      },
      "deviceEnrollmentLimit": 5,
      "aboutMe": "About Me value",
      "birthday": "2017-01-01T00:03:19.3691456+03:00",
      "hireDate": "2016-12-31T23:56:54.3148236+03:00",
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

