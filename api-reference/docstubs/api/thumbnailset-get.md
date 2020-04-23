---
title: "Get thumbnailSet"
description: "Read the properties and relationships of a thumbnailSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get thumbnailSet

Namespace: microsoft.graph

Read the properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.

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
GET /workbooks/{workbooksId}/thumbnails/{thumbnailSetId}
GET /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/thumbnails/{thumbnailSetId}
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
If successful, this method returns a `200 OK` response code and a [thumbnailSet](../resources/thumbnailset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/thumbnails/{thumbnailSetId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.thumbnailSet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.thumbnailSet",
    "id": "f9c9ebe5-ebe5-f9c9-e5eb-c9f9e5ebc9f9",
    "large": {
      "@odata.type": "microsoft.graph.thumbnail",
      "content": "Stream",
      "height": 6,
      "sourceItemId": "Source Item Id value",
      "url": "Url value",
      "width": 5
    },
    "medium": {
      "@odata.type": "microsoft.graph.thumbnail"
    },
    "small": {
      "@odata.type": "microsoft.graph.thumbnail"
    },
    "source": {
      "@odata.type": "microsoft.graph.thumbnail"
    }
  }
}
```

