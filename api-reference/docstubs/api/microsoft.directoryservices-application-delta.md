---
title: "application: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# delta

Namespace: Microsoft.DirectoryServices

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
If successful, this function returns a `200 OK` response code and a [application](../resources/microsoft.directoryservices-application.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "application_delta"
}
-->
``` http
GET https://graph.microsoft.com/changelog/applications/delta
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.directoryservices.application)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.DirectoryServices.application",
      "id": "9ce4c367-c367-9ce4-67c3-e49c67c3e49c",
      "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
      "api": {
        "@odata.type": "Microsoft.DirectoryServices.apiApplication"
      },
      "appId": "App Id value",
      "appRoles": [
        {
          "@odata.type": "Microsoft.DirectoryServices.appRole"
        }
      ],
      "createdDateTime": "2017-01-01T00:03:17.7218452+00:00",
      "isFallbackPublicClient": true,
      "identifierUris": [
        "Identifier Uris value"
      ],
      "groupMembershipClaims": 5,
      "info": {
        "@odata.type": "Microsoft.DirectoryServices.informationalUrl"
      },
      "isDeviceOnlyAuthSupported": true,
      "keyCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.keyCredential"
        }
      ],
      "logo": "Stream",
      "optionalClaims": {
        "@odata.type": "Microsoft.DirectoryServices.optionalClaims"
      },
      "parentalControlSettings": {
        "@odata.type": "Microsoft.DirectoryServices.parentalControlSettings"
      },
      "passwordCredentials": [
        {
          "@odata.type": "Microsoft.DirectoryServices.passwordCredential"
        }
      ],
      "publicClient": {
        "@odata.type": "Microsoft.DirectoryServices.publicClientApplication"
      },
      "publisherDomain": "Publisher Domain value",
      "requiredResourceAccess": [
        {
          "@odata.type": "Microsoft.DirectoryServices.requiredResourceAccess"
        }
      ],
      "signInAudience": "Sign In Audience value",
      "tags": [
        "Tags value"
      ],
      "tokenEncryptionKeyId": "992a9363-9363-992a-6393-2a9963932a99",
      "web": {
        "@odata.type": "Microsoft.DirectoryServices.webApplication"
      }
    }
  ]
}
```

