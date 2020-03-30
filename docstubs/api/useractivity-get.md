---
title: "Get userActivity"
description: "Read properties and relationships of the userActivity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userActivity

Namespace: microsoft.graph

Read properties and relationships of the [userActivity](../resources/useractivity.md) object.

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
GET /me/activities/{userActivityId}
GET /users/{usersId}/activities/{userActivityId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [userActivity](../resources/useractivity.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_useractivity"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/activities/{userActivityId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userActivity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1358

{
  "value": {
    "@odata.type": "#microsoft.graph.userActivity",
    "id": "7436b7a0-b7a0-7436-a0b7-3674a0b73674",
    "visualElements": {
      "@odata.type": "microsoft.graph.visualInfo",
      "attribution": {
        "@odata.type": "microsoft.graph.imageInfo",
        "iconUrl": "https://example.com/iconUrl/",
        "alternativeText": "Alternative Text value",
        "alternateText": "Alternate Text value",
        "addImageQuery": true
      },
      "backgroundColor": "Background Color value",
      "description": "Description value",
      "displayText": "Display Text value",
      "content": {
        "@odata.type": "microsoft.graph.Json"
      }
    },
    "activitySourceHost": "Activity Source Host value",
    "activationUrl": "https://example.com/activationUrl/",
    "appActivityId": "App Activity Id value",
    "appDisplayName": "App Display Name value",
    "contentUrl": "https://example.com/contentUrl/",
    "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
    "expirationDateTime": "2016-12-31T23:59:40.5485728+00:00",
    "fallbackUrl": "https://example.com/fallbackUrl/",
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
    "userTimezone": "User Timezone value",
    "contentInfo": {
      "@odata.type": "microsoft.graph.Json"
    },
    "status": "String"
  }
}
```

