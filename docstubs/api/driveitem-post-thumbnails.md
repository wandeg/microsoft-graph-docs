---
title: "Create thumbnails"
description: "Create a new thumbnails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create thumbnails

Namespace: microsoft.graph

Create a new thumbnails object.

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
POST /workbooks/{workbooksId}/thumbnails
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/thumbnails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [thumbnailSet](../resources/thumbnailset.md) object.

The following table shows the properties that are required when you create the [thumbnailSet](../resources/thumbnailset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|large|[thumbnail](../resources/thumbnail.md)|**TODO: Add Description**|
|medium|[thumbnail](../resources/thumbnail.md)|**TODO: Add Description**|
|small|[thumbnail](../resources/thumbnail.md)|**TODO: Add Description**|
|source|[thumbnail](../resources/thumbnail.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [thumbnailSet](../resources/thumbnailset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_thumbnailset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/thumbnails
Content-Type: application/json
Content-length: 459

{
  "@odata.type": "#microsoft.graph.thumbnailSet",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.thumbnailset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```

