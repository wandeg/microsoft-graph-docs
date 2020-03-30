---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /applications/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [application](../resources/application.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "application_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.application)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1851

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "713468fa-68fa-7134-fa68-3471fa683471",
      "deletedDateTime": "2016-12-31T23:58:41.2829368+00:00",
      "api": {
        "@odata.type": "microsoft.graph.apiApplication"
      },
      "appId": "App Id value",
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "isFallbackPublicClient": true,
      "identifierUris": [
        "Identifier Uris value"
      ],
      "displayName": "Display Name value",
      "groupMembershipClaims": "Group Membership Claims value",
      "info": {
        "@odata.type": "microsoft.graph.informationalUrl"
      },
      "isDeviceOnlyAuthSupported": true,
      "keyCredentials": [
        {
          "@odata.type": "microsoft.graph.keyCredential"
        }
      ],
      "logo": "Stream",
      "optionalClaims": {
        "@odata.type": "microsoft.graph.optionalClaims"
      },
      "parentalControlSettings": {
        "@odata.type": "microsoft.graph.parentalControlSettings"
      },
      "passwordCredentials": [
        {
          "@odata.type": "microsoft.graph.passwordCredential"
        }
      ],
      "publicClient": {
        "@odata.type": "microsoft.graph.publicClientApplication"
      },
      "publisherDomain": "Publisher Domain value",
      "requiredResourceAccess": [
        {
          "@odata.type": "microsoft.graph.requiredResourceAccess"
        }
      ],
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "373f31b3-31b3-373f-b331-3f37b3313f37",
      "web": {
        "@odata.type": "microsoft.graph.webApplication"
      }
    }
  ]
}
```

