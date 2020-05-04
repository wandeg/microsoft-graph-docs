---
title: "Update user"
description: "Update the properties of a user object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update user

Namespace: microsoft.graph

Update the properties of a [user](../resources/user.md) object.

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
PATCH /me
PATCH /users/{usersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [user](../resources/user.md) object.

The following table shows the properties that are required when you create the [user](../resources/user.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|signInActivity|[signInActivity](../resources/signinactivity.md)|**TODO: Add Description**|
|accountEnabled|Boolean|**TODO: Add Description**|
|ageGroup|String|**TODO: Add Description**|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description**|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description**|
|businessPhones|String collection|**TODO: Add Description**|
|city|String|**TODO: Add Description**|
|companyName|String|**TODO: Add Description**|
|consentProvidedForMinor|String|**TODO: Add Description**|
|country|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|creationType|String|**TODO: Add Description**|
|department|String|**TODO: Add Description**|
|deviceKeys|[deviceKey](../resources/devicekey.md) collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|employeeId|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|givenName|String|**TODO: Add Description**|
|identities|[objectIdentity](../resources/objectidentity.md) collection|**TODO: Add Description**|
|imAddresses|String collection|**TODO: Add Description**|
|isResourceAccount|Boolean|**TODO: Add Description**|
|jobTitle|String|**TODO: Add Description**|
|lastPasswordChangeDateTime|DateTimeOffset|**TODO: Add Description**|
|legalAgeGroupClassification|String|**TODO: Add Description**|
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseassignmentstate.md) collection|**TODO: Add Description**|
|mail|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|mobilePhone|String|**TODO: Add Description**|
|onPremisesDistinguishedName|String|**TODO: Add Description**|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description**|
|onPremisesImmutableId|String|**TODO: Add Description**|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description**|
|onPremisesSecurityIdentifier|String|**TODO: Add Description**|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description**|
|onPremisesDomainName|String|**TODO: Add Description**|
|onPremisesSamAccountName|String|**TODO: Add Description**|
|onPremisesUserPrincipalName|String|**TODO: Add Description**|
|otherMails|String collection|**TODO: Add Description**|
|passwordPolicies|String|**TODO: Add Description**|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description**|
|officeLocation|String|**TODO: Add Description**|
|postalCode|String|**TODO: Add Description**|
|preferredDataLocation|String|**TODO: Add Description**|
|preferredLanguage|String|**TODO: Add Description**|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description**|
|proxyAddresses|String collection|**TODO: Add Description**|
|refreshTokensValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|showInAddressList|Boolean|**TODO: Add Description**|
|signInSessionsValidFromDateTime|DateTimeOffset|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|streetAddress|String|**TODO: Add Description**|
|surname|String|**TODO: Add Description**|
|usageLocation|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|externalUserState|String|**TODO: Add Description**|
|externalUserStateChangeDateTime|String|**TODO: Add Description**|
|userType|String|**TODO: Add Description**|
|mailboxSettings|[mailboxSettings](../resources/mailboxsettings.md)|**TODO: Add Description**|
|identityUserRisk|[identityUserRisk](../resources/identityuserrisk.md)|**TODO: Add Description**|
|deviceEnrollmentLimit|Int32|The limit on the maximum number of devices that the user is permitted to enroll. Allowed values are 5 or 1000.|
|aboutMe|String|**TODO: Add Description**|
|birthday|DateTimeOffset|**TODO: Add Description**|
|hireDate|DateTimeOffset|**TODO: Add Description**|
|interests|String collection|**TODO: Add Description**|
|mySite|String|**TODO: Add Description**|
|pastProjects|String collection|**TODO: Add Description**|
|preferredName|String|**TODO: Add Description**|
|responsibilities|String collection|**TODO: Add Description**|
|schools|String collection|**TODO: Add Description**|
|skills|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [user](../resources/user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_user"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me
Content-Type: application/json
Content-length: 7483

{
  "@odata.type": "#microsoft.graph.user",
  "deletedDateTime": "2016-12-31T23:58:36.0226893+03:00",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity",
    "lastSignInDateTime": "2016-12-31T23:56:42.8288013+03:00",
    "lastSignInRequestId": "Last Sign In Request Id value"
  },
  "accountEnabled": true,
  "ageGroup": "Age Group value",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "0e01a038-a038-0e01-38a0-010e38a0010e"
      ],
      "skuId": "5ae52abf-2abf-5ae5-bf2a-e55abf2ae55a"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:02:38.7080644+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "96113b9d-3b9d-9611-9d3b-11969d3b1196"
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
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey",
      "keyType": "Key Type value",
      "keyMaterial": "a2V5TWF0ZXJpYWw=",
      "deviceId": "a868e7f1-e7f1-a868-f1e7-68a8f1e768a8"
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
  "lastPasswordChangeDateTime": "2017-01-01T00:00:28.983404+03:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:44.6618878+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:58.2206726+03:00"
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
  "refreshTokensValidFromDateTime": "2016-12-31T23:58:39.2189521+03:00",
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2017-01-01T00:02:12.4864055+03:00",
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
      "startTime": "12:03:27.3180000",
      "endTime": "12:03:31.0050000",
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
    "lastChangedDateTime": "2016-12-31T23:59:12.339171+03:00"
  },
  "deviceEnrollmentLimit": 5,
  "aboutMe": "About Me value",
  "birthday": "2017-01-01T00:00:47.3962323+03:00",
  "hireDate": "2017-01-01T00:01:52.3488882+03:00",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "5c95de49-de49-5c95-49de-955c49de955c",
  "deletedDateTime": "2016-12-31T23:58:36.0226893+03:00",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity",
    "lastSignInDateTime": "2016-12-31T23:56:42.8288013+03:00",
    "lastSignInRequestId": "Last Sign In Request Id value"
  },
  "accountEnabled": true,
  "ageGroup": "Age Group value",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "0e01a038-a038-0e01-38a0-010e38a0010e"
      ],
      "skuId": "5ae52abf-2abf-5ae5-bf2a-e55abf2ae55a"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:02:38.7080644+03:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "96113b9d-3b9d-9611-9d3b-11969d3b1196"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "city": "City value",
  "companyName": "Company Name value",
  "consentProvidedForMinor": "Consent Provided For Minor value",
  "country": "Country value",
  "createdDateTime": "2016-12-31T23:57:35.7108579+03:00",
  "creationType": "Creation Type value",
  "department": "Department value",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey",
      "keyType": "Key Type value",
      "keyMaterial": "a2V5TWF0ZXJpYWw=",
      "deviceId": "a868e7f1-e7f1-a868-f1e7-68a8f1e768a8"
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
  "lastPasswordChangeDateTime": "2017-01-01T00:00:28.983404+03:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:01:44.6618878+03:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2016-12-31T23:56:58.2206726+03:00"
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
  "refreshTokensValidFromDateTime": "2016-12-31T23:58:39.2189521+03:00",
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2017-01-01T00:02:12.4864055+03:00",
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
      "startTime": "12:03:27.3180000",
      "endTime": "12:03:31.0050000",
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
    "lastChangedDateTime": "2016-12-31T23:59:12.339171+03:00"
  },
  "deviceEnrollmentLimit": 5,
  "aboutMe": "About Me value",
  "birthday": "2017-01-01T00:00:47.3962323+03:00",
  "hireDate": "2017-01-01T00:01:52.3488882+03:00",
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
```

