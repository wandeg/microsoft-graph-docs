---
title: "List tabs"
description: "Get the teamsTabs from the tabs navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tabs

Namespace: microsoft.graph

Get the teamsTabs from the tabs navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/channels/{channelId}/tabs
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
If successful, this method returns a `200 OK` response code and a collection of [teamsTab](../resources/teamstab.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamstab"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/channels/{channelId}/tabs
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamstab)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsTab",
      "id": "b4f3b694-b694-b4f3-94b6-f3b494b6f3b4",
      "displayName": "Display Name value",
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

