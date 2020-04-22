---
title: "application: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /applications/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [application](../resources/application.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "application_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/delta
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.application)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.application",
      "id": "f7ea2a25-2a25-f7ea-252a-eaf7252aeaf7",
      "deletedDateTime": "2016-12-31T23:59:39.086137+00:00",
      "addIns": [
        {
          "@odata.type": "microsoft.graph.addIn"
        }
      ],
      "api": {
        "@odata.type": "microsoft.graph.apiApplication"
      },
      "appId": "App Id value",
      "applicationTemplateId": "Application Template Id value",
      "appRoles": [
        {
          "@odata.type": "microsoft.graph.appRole"
        }
      ],
      "isFallbackPublicClient": true,
      "identifierUris": [
        "Identifier Uris value"
      ],
      "createdDateTime": "2017-01-01T00:02:14.13292+00:00",
      "publicClient": {
        "@odata.type": "microsoft.graph.publicClientApplication"
      },
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
      "oauth2RequirePostResponse": true,
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
      "tokenEncryptionKeyId": "ad1a7c43-7c43-ad1a-437c-1aad437c1aad",
      "web": {
        "@odata.type": "microsoft.graph.webApplication"
      }
    }
  ]
}
```

