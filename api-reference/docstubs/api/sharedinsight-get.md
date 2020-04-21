---
title: "Get sharedInsight"
description: "Read properties and relationships of a sharedInsight object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get sharedInsight

Namespace: microsoft.graph

Read properties and relationships of a [sharedInsight](../resources/sharedinsight.md) object.

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
GET /invitations/{invitationsId}/invitedUser/insights/shared/{sharedInsightId}
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
If successful, this method returns a `200 OK` response code and a [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sharedinsight"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/insights/shared/{sharedInsightId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedInsight"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.sharedInsight",
    "id": "fe9096da-96da-fe90-da96-90feda9690fe",
    "lastShared": {
      "@odata.type": "microsoft.graph.sharingDetail",
      "sharedBy": {
        "@odata.type": "microsoft.graph.insightIdentity",
        "displayName": "Display Name value",
        "id": "Id value",
        "address": "Address value"
      },
      "sharedDateTime": "2016-12-31T23:59:21.0108234+00:00",
      "sharingSubject": "Sharing Subject value",
      "sharingType": "Sharing Type value",
      "sharingReference": {
        "@odata.type": "microsoft.graph.resourceReference",
        "webUrl": "https://example.com/webUrl/",
        "type": "Type value"
      }
    },
    "sharingHistory": [
      {
        "@odata.type": "microsoft.graph.sharingDetail"
      }
    ],
    "resourceVisualization": {
      "@odata.type": "microsoft.graph.resourceVisualization",
      "title": "Title value",
      "mediaType": "Media Type value",
      "previewImageUrl": "https://example.com/previewImageUrl/",
      "previewText": "Preview Text value",
      "containerWebUrl": "https://example.com/containerWebUrl/",
      "containerDisplayName": "Container Display Name value",
      "containerType": "Container Type value"
    },
    "resourceReference": {
      "@odata.type": "microsoft.graph.resourceReference"
    }
  }
}
```

