---
title: "Get application"
description: "Read the properties and relationships of an application object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get application

Namespace: microsoft.graph

Read the properties and relationships of an [application](../resources/application.md) object.

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
GET /applications/{applicationsId}
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

If successful, this method returns a `200 OK` response code and an [application](../resources/application.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_application"
}
-->
``` http
GET https://graph.microsoft.com/beta/applications/{applicationsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.application",
    "id": "d090e6b3-e6b3-d090-b3e6-90d0b3e690d0",
    "deletedDateTime": "String (timestamp)",
    "api": {
      "@odata.type": "microsoft.graph.apiApplication"
    },
    "appId": "String",
    "appRoles": [
      {
        "@odata.type": "microsoft.graph.appRole"
      }
    ],
    "createdDateTime": "String (timestamp)",
    "isFallbackPublicClient": "Boolean",
    "identifierUris": [
      "String"
    ],
    "groupMembershipClaims": "Integer",
    "info": {
      "@odata.type": "microsoft.graph.informationalUrl"
    },
    "isDeviceOnlyAuthSupported": "Boolean",
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
    "publisherDomain": "String",
    "requiredResourceAccess": [
      {
        "@odata.type": "microsoft.graph.requiredResourceAccess"
      }
    ],
    "signInAudience": "String",
    "tags": [
      "String"
    ],
    "tokenEncryptionKeyId": "Guid",
    "web": {
      "@odata.type": "microsoft.graph.webApplication"
    }
  }
}
```

