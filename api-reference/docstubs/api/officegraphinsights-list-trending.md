---
title: "List trending"
description: "Get the trendings from the trending navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List trending

Namespace: microsoft.graph

Get the trendings from the trending navigation property.

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
GET /invitations/{invitationsId}/invitedUser/insights/trending
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
If successful, this method returns a `200 OK` response code and a collection of [trending](../resources/trending.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_trending"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/insights/trending
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.trending)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.trending",
      "id": "99935c04-5c04-9993-045c-9399045c9399",
      "weight": "Double",
      "resourceVisualization": {
        "@odata.type": "microsoft.graph.resourceVisualization",
        "title": "Title value",
        "type": "Type value",
        "mediaType": "Media Type value",
        "previewImageUrl": "https://example.com/previewImageUrl/",
        "previewText": "Preview Text value",
        "containerWebUrl": "https://example.com/containerWebUrl/",
        "containerDisplayName": "Container Display Name value",
        "containerType": "Container Type value"
      },
      "resourceReference": {
        "@odata.type": "microsoft.graph.resourceReference",
        "webUrl": "https://example.com/webUrl/",
        "id": "Id value"
      },
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
    }
  ]
}
```

