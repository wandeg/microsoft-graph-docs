---
title: "List tabs"
description: "Get the teamsTabs from the tabs navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List tabs

Namespace: microsoft.graph

Get the teamsTabs from the tabs navigation property.

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
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/tabs
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsTab](../resources/teamstab.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamstab"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/channels/{channelId}/tabs
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamstab)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 707

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsTab",
      "id": "bcab996c-996c-bcab-6c99-abbc6c99abbc",
      "name": "Name value",
      "displayName": "Display Name value",
      "teamsAppId": "Teams App Id value",
      "sortOrderIndex": "Sort Order Index value",
      "messageId": "Message Id value",
      "webUrl": "https://example.com/webUrl/",
      "configuration": {
        "@odata.type": "microsoft.graph.teamsTabConfiguration",
        "entityId": "Entity Id value",
        "contentUrl": "https://example.com/contentUrl/",
        "removeUrl": "https://example.com/removeUrl/",
        "websiteUrl": "https://example.com/websiteUrl/"
      }
    }
  ]
}
```

