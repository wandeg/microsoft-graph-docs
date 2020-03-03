---
title: "List names"
description: "Get the personNames from the names navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List names

Namespace: microsoft.graph

Get the personNames from the names navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/profile/names
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [personName](../resources/personname.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_personname"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/profile/names
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.personname)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.personName",
      "id": "cde5325e-325e-cde5-5e32-e5cd5e32e5cd",
      "allowedAudiences": "String",
      "inference": {
        "@odata.type": "microsoft.graph.inferenceData",
        "confidenceScore": "Double",
        "userHasVerifiedAccuracy": true
      },
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "displayName": "Display Name value",
      "first": "First value",
      "initials": "Initials value",
      "last": "Last value",
      "languageTag": "Language Tag value",
      "maiden": "Maiden value",
      "middle": "Middle value",
      "nickname": "Nickname value",
      "suffix": "Suffix value",
      "title": "Title value",
      "pronunciation": {
        "@odata.type": "microsoft.graph.yomiPersonName"
      }
    }
  ]
}
```

