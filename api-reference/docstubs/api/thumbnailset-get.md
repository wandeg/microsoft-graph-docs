---
title: "Get thumbnailSet"
description: "Read properties and relationships of a thumbnailSet object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get thumbnailSet

Namespace: microsoft.graph

Read properties and relationships of a [thumbnailSet](../resources/thumbnailset.md) object.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/thumbnails/{thumbnailSetId}
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "47dcd481-d481-47dc-81d4-dc4781d4dc47",
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

