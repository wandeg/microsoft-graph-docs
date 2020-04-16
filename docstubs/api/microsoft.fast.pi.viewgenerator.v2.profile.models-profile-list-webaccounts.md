---
title: "List webAccounts"
description: "Get the webAccounts from the webAccounts navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List webAccounts

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

Get the webAccounts from the webAccounts navigation property.

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
GET /user/{userId}/profile/webAccounts
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
If successful, this method returns a `200 OK` response code and a collection of [webAccount](../resources/webaccount.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_webaccount"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/{userId}/profile/webAccounts
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.fast.pi.viewgenerator.v2.profile.models.webaccount)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.webAccount",
      "id": "c0b9cc26-cc26-c0b9-26cc-b9c026ccb9c0",
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
      "description": "Description value",
      "userId": "User Id value",
      "service": {
        "@odata.type": "Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.serviceInformation",
        "name": "Name value",
        "webUrl": "https://example.com/webUrl/"
      },
      "statusMessage": "Status Message value",
      "webUrl": "https://example.com/webUrl/"
    }
  ]
}
```

