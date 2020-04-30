---
title: "Get user"
description: "Read properties and relationships of an user object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get user

Namespace: Microsoft.DirectoryServices

Read properties and relationships of an [user](../resources/microsoft.directoryservices-user.md) object.

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
GET /me
GET /users/{usersId}
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
If successful, this method returns a `200 OK` response code and an [user](../resources/microsoft.directoryservices-user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/changelog/me
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.user"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.DirectoryServices.user",
    "id": "b1872668-2668-b187-6826-87b1682687b1",
    "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
    "accountEnabled": true,
    "ageGroup": "Age Group value",
    "assignedLicenses": [
      {
        "@odata.type": "Microsoft.DirectoryServices.assignedLicense",
        "disabledPlans": [
          "c406e236-e236-c406-36e2-06c436e206c4"
        ],
        "skuId": "92ad2f35-2f35-92ad-352f-ad92352fad92"
      }
    ],
    "assignedPlans": [
      {
        "@odata.type": "Microsoft.DirectoryServices.assignedPlan",
        "assignedDateTime": "2017-01-01T00:01:08.5371837+00:00",
        "capabilityStatus": "Capability Status value",
        "service": "Service value",
        "servicePlanId": "4545cb79-cb79-4545-79cb-454579cb4545"
      }
    ],
    "businessPhones": [
      "Business Phones value"
    ],
    "city": "City value",
    "companyName": "Company Name value",
    "consentProvidedForMinor": "Consent Provided For Minor value",
    "country": "Country value",
    "createdDateTime": "2017-01-01T00:03:17.7218452+00:00",
    "creationType": "Creation Type value",
    "department": "Department value",
    "deviceKeys": [
      {
        "@odata.type": "Microsoft.DirectoryServices.deviceKey",
        "keyType": "Key Type value",
        "keyMaterial": "a2V5TWF0ZXJpYWw=",
        "deviceId": "345458fe-58fe-3454-fe58-5434fe585434"
      }
    ],
    "displayName": "Display Name value",
    "employeeId": "Employee Id value",
    "faxNumber": "Fax Number value",
    "givenName": "Given Name value",
    "identities": [
      {
        "@odata.type": "Microsoft.DirectoryServices.objectIdentity",
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
    "lastPasswordChangeDateTime": "2016-12-31T23:59:08.109435+00:00",
    "legalAgeGroupClassification": "Legal Age Group Classification value",
    "licenseAssignmentStates": [
      {
        "@odata.type": "Microsoft.DirectoryServices.licenseAssignmentState",
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
      "@odata.type": "Microsoft.DirectoryServices.onPremisesExtensionAttributes",
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
    "onPremisesLastSyncDateTime": "2017-01-01T00:01:50.2848835+00:00",
    "onPremisesProvisioningErrors": [
      {
        "@odata.type": "Microsoft.DirectoryServices.onPremisesProvisioningError",
        "value": "Value value",
        "category": "Category value",
        "propertyCausingError": "Property Causing Error value",
        "occurredDateTime": "2016-12-31T23:56:32.7107544+00:00"
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
      "@odata.type": "Microsoft.DirectoryServices.passwordProfile",
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
        "@odata.type": "Microsoft.DirectoryServices.provisionedPlan",
        "provisioningStatus": "Provisioning Status value"
      }
    ],
    "proxyAddresses": [
      "Proxy Addresses value"
    ],
    "refreshTokensValidFromDateTime": "2016-12-31T23:59:51.9706017+00:00",
    "showInAddressList": true,
    "signInSessionsValidFromDateTime": "2017-01-01T00:03:19.4591516+00:00",
    "state": "State value",
    "streetAddress": "Street Address value",
    "surname": "Surname value",
    "usageLocation": "Usage Location value",
    "userPrincipalName": "User Principal Name value",
    "externalUserState": "External User State value",
    "externalUserStateChangeDateTime": "External User State Change Date Time value",
    "userType": "User Type value"
  }
}
```

