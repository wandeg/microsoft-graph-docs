---
title: "Get teamsTab"
description: "Read properties and relationships of the teamsTab object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get teamsTab

Namespace: microsoft.graph

Read properties and relationships of the [teamsTab](../resources/teamstab.md) object.

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
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}
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
If successful, this method returns a `200 OK` response code and [teamsTab](../resources/teamstab.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamstab"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/channels/{channelId}/tabs/{teamsTabId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsTab"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 663

{
  "value": {
    "@odata.type": "#microsoft.graph.teamsTab",
    "id": "9b19b38c-b38c-9b19-8cb3-199b8cb3199b",
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
}
```

