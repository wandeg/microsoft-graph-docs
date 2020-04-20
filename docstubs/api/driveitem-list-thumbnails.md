---
title: "List thumbnails"
description: "Get the thumbnailSets from the thumbnails navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List thumbnails

Namespace: microsoft.graph

Get the thumbnailSets from the thumbnails navigation property.

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
GET /workbooks/{workbooksId}/thumbnails
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/thumbnails
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
If successful, this method returns a `200 OK` response code and a collection of [thumbnailSet](../resources/thumbnailset.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_thumbnailset"
}
-->
``` http
GET https://graph.microsoft.com/beta/workbooks/{workbooksId}/thumbnails
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.thumbnailset)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.thumbnailSet",
      "id": "d6e1884a-884a-d6e1-4a88-e1d64a88e1d6",
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
  ]
}
```

