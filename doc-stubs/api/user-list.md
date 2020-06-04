---
title: "List users"
description: "Get a list of the user objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List users
Namespace: microsoft.graph

Get a list of the [user](../resources/user.md) objects and their properties.

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
GET /users
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

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
GET https://graph.microsoft.com/beta/users
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
      "id": "c8cf5983-5983-c8cf-8359-cfc88359cfc8",
      "deletedDateTime": "String (timestamp)",
      "accountEnabled": "Boolean",
      "ageGroup": "String",
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
        "String"
      ],
      "city": "String",
      "companyName": "String",
      "consentProvidedForMinor": "String",
      "country": "String",
      "createdDateTime": "String (timestamp)",
      "creationType": "String",
      "department": "String",
      "deviceKeys": [
        {
          "@odata.type": "microsoft.graph.deviceKey"
        }
      ],
      "displayName": "String",
      "employeeId": "String",
      "faxNumber": "String",
      "givenName": "String",
      "identities": [
        {
          "@odata.type": "microsoft.graph.objectIdentity"
        }
      ],
      "imAddresses": [
        "String"
      ],
      "isResourceAccount": "Boolean",
      "jobTitle": "String",
      "lastPasswordChangeDateTime": "String (timestamp)",
      "legalAgeGroupClassification": "String",
      "licenseAssignmentStates": [
        {
          "@odata.type": "microsoft.graph.licenseAssignmentState"
        }
      ],
      "mail": "String",
      "mailNickname": "String",
      "mobilePhone": "String",
      "onPremisesDistinguishedName": "String",
      "onPremisesExtensionAttributes": {
        "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
      },
      "onPremisesImmutableId": "String",
      "onPremisesLastSyncDateTime": "String (timestamp)",
      "onPremisesProvisioningErrors": [
        {
          "@odata.type": "microsoft.graph.onPremisesProvisioningError"
        }
      ],
      "onPremisesSecurityIdentifier": "String",
      "onPremisesSyncEnabled": "Boolean",
      "onPremisesDomainName": "String",
      "onPremisesSamAccountName": "String",
      "onPremisesUserPrincipalName": "String",
      "otherMails": [
        "String"
      ],
      "passwordPolicies": "String",
      "passwordProfile": {
        "@odata.type": "microsoft.graph.passwordProfile"
      },
      "officeLocation": "String",
      "postalCode": "String",
      "preferredDataLocation": "String",
      "preferredLanguage": "String",
      "provisionedPlans": [
        {
          "@odata.type": "microsoft.graph.provisionedPlan"
        }
      ],
      "proxyAddresses": [
        "String"
      ],
      "refreshTokensValidFromDateTime": "String (timestamp)",
      "showInAddressList": "Boolean",
      "signInSessionsValidFromDateTime": "String (timestamp)",
      "state": "String",
      "streetAddress": "String",
      "surname": "String",
      "usageLocation": "String",
      "userPrincipalName": "String",
      "externalUserState": "String",
      "externalUserStateChangeDateTime": "String",
      "userType": "String"
    }
  ]
}
```

