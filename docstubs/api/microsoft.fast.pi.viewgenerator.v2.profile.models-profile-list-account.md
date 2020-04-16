---
title: "List account"
description: "Get the userAccountInformations from the account navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List account

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

Get the userAccountInformations from the account navigation property.

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
GET /user/{userId}/profile/account
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
If successful, this method returns a `200 OK` response code and a collection of [userAccountInformation](../resources/useraccountinformation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/{userId}/profile/account
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.fast.pi.viewgenerator.v2.profile.models.useraccountinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.userAccountInformation",
      "id": "4a3610f1-10f1-4a36-f110-364af110364a",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.inferenceData",
        "confidenceScore": "Double",
        "userHasVerifiedAccuracy": true
      },
      "createdDateTime": "2016-12-31T23:59:45.9448095+03:00",
      "createdBy": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identitySet",
        "application": {
          "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity",
          "displayName": "Display Name value",
          "id": "Id value"
        },
        "device": {
          "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
        },
        "user": {
          "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identity"
        }
      },
      "lastModifiedDateTime": "2017-01-01T00:00:42.7561162+03:00",
      "lastModifiedBy": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.identitySet"
      },
      "ageGroup": "Age Group value",
      "countryCode": "Country Code value",
      "preferredLanguageTag": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.localeInfo",
        "locale": "Locale value"
      },
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```

