---
title: "Add users"
description: "Add users by posting to the users collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add users

Namespace: microsoft.graph

Add users by posting to the users collection.

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
POST /me/managedDevices/{managedDeviceId}/users/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [user](../resources/user.md) object.

The following table shows the properties that are required when you create the [user](../resources/user.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|signInActivity|[signInActivity](../resources/signinactivity.md)||
|accountEnabled|Boolean||
|ageGroup|String||
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection||
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection||
|businessPhones|String collection||
|city|String||
|companyName|String||
|consentProvidedForMinor|String||
|country|String||
|createdDateTime|DateTimeOffset||
|creationType|String||
|department|String||
|deviceKeys|[deviceKey](../resources/devicekey.md) collection||
|displayName|String||
|employeeId|String||
|faxNumber|String||
|givenName|String||
|identities|[objectIdentity](../resources/objectidentity.md) collection||
|imAddresses|String collection||
|isResourceAccount|Boolean||
|jobTitle|String||
|lastPasswordChangeDateTime|DateTimeOffset||
|legalAgeGroupClassification|String||
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseassignmentstate.md) collection||
|mail|String||
|mailNickname|String||
|mobilePhone|String||
|onPremisesDistinguishedName|String||
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)||
|onPremisesImmutableId|String||
|onPremisesLastSyncDateTime|DateTimeOffset||
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection||
|onPremisesSecurityIdentifier|String||
|onPremisesSyncEnabled|Boolean||
|onPremisesDomainName|String||
|onPremisesSamAccountName|String||
|onPremisesUserPrincipalName|String||
|otherMails|String collection||
|passwordPolicies|String||
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)||
|officeLocation|String||
|postalCode|String||
|preferredDataLocation|String||
|preferredLanguage|String||
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection||
|proxyAddresses|String collection||
|refreshTokensValidFromDateTime|DateTimeOffset||
|showInAddressList|Boolean||
|signInSessionsValidFromDateTime|DateTimeOffset||
|state|String||
|streetAddress|String||
|surname|String||
|usageLocation|String||
|userPrincipalName|String||
|externalUserState|String||
|externalUserStateChangeDateTime|String||
|userType|String||
|mailboxSettings|[mailboxSettings](../resources/mailboxsettings.md)||
|identityUserRisk|[identityUserRisk](../resources/identityuserrisk.md)||
|deviceEnrollmentLimit|Int32||
|aboutMe|String||
|birthday|DateTimeOffset||
|hireDate|DateTimeOffset||
|interests|String collection||
|mySite|String||
|pastProjects|String collection||
|preferredName|String||
|responsibilities|String collection||
|schools|String collection||
|skills|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/users
Content-type: application/json
Content-length: 7485

{
  "@odata.type": "#microsoft.graph.user",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity",
    "lastSignInDateTime": "2017-01-01T00:03:32.9277539+00:00",
    "lastSignInRequestId": "Last Sign In Request Id value"
  },
  "accountEnabled": true,
  "ageGroup": "Age Group value",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "c2c74c42-4c42-c2c7-424c-c7c2424cc7c2"
      ],
      "skuId": "65e2edee-edee-65e2-eeed-e265eeede265"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:39.2870043+00:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "be0a7a38-7a38-be0a-387a-0abe387a0abe"
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
      "deviceId": "4ec050f2-50f2-4ec0-f250-c04ef250c04e"
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
  "lastPasswordChangeDateTime": "2016-12-31T23:57:16.1115942+00:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:00:01.9470378+00:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:00:40.7718948+00:00"
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
  "refreshTokensValidFromDateTime": "2017-01-01T00:03:11.1387757+00:00",
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2016-12-31T23:56:58.3658021+00:00",
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
      "startTime": "12:02:02.2840000",
      "endTime": "11:57:44.4220000",
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
    "lastChangedDateTime": "2017-01-01T00:02:50.0550119+00:00"
  },
  "deviceEnrollmentLimit": 5,
  "aboutMe": "About Me value",
  "birthday": "2016-12-31T23:58:50.7295567+00:00",
  "hireDate": "2016-12-31T23:58:08.2857048+00:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7593

{
  "@odata.type": "#microsoft.graph.user",
  "id": "69beb2d1-b2d1-69be-d1b2-be69d1b2be69",
  "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity",
    "lastSignInDateTime": "2017-01-01T00:03:32.9277539+00:00",
    "lastSignInRequestId": "Last Sign In Request Id value"
  },
  "accountEnabled": true,
  "ageGroup": "Age Group value",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense",
      "disabledPlans": [
        "c2c74c42-4c42-c2c7-424c-c7c2424cc7c2"
      ],
      "skuId": "65e2edee-edee-65e2-eeed-e265eeede265"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan",
      "assignedDateTime": "2017-01-01T00:00:39.2870043+00:00",
      "capabilityStatus": "Capability Status value",
      "service": "Service value",
      "servicePlanId": "be0a7a38-7a38-be0a-387a-0abe387a0abe"
    }
  ],
  "businessPhones": [
    "Business Phones value"
  ],
  "city": "City value",
  "companyName": "Company Name value",
  "consentProvidedForMinor": "Consent Provided For Minor value",
  "country": "Country value",
  "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
  "creationType": "Creation Type value",
  "department": "Department value",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey",
      "keyType": "Key Type value",
      "keyMaterial": "a2V5TWF0ZXJpYWw=",
      "deviceId": "4ec050f2-50f2-4ec0-f250-c04ef250c04e"
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
  "lastPasswordChangeDateTime": "2016-12-31T23:57:16.1115942+00:00",
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
  "onPremisesLastSyncDateTime": "2017-01-01T00:00:01.9470378+00:00",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError",
      "value": "Value value",
      "category": "Category value",
      "propertyCausingError": "Property Causing Error value",
      "occurredDateTime": "2017-01-01T00:00:40.7718948+00:00"
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
  "refreshTokensValidFromDateTime": "2017-01-01T00:03:11.1387757+00:00",
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "2016-12-31T23:56:58.3658021+00:00",
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
      "startTime": "12:02:02.2840000",
      "endTime": "11:57:44.4220000",
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
    "lastChangedDateTime": "2017-01-01T00:02:50.0550119+00:00"
  },
  "deviceEnrollmentLimit": 5,
  "aboutMe": "About Me value",
  "birthday": "2016-12-31T23:58:50.7295567+00:00",
  "hireDate": "2016-12-31T23:58:08.2857048+00:00",
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

