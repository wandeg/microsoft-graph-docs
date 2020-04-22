---
title: "Update thumbnails"
description: "Update the properties of a thumbnails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update thumbnails

Namespace: microsoft.graph

Update the properties of a thumbnails object.

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
PATCH /workbooks/{workbooksId}/thumbnails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [thumbnailSet](../resources/thumbnailset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_thumbnails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbooks/{workbooksId}/thumbnails
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.thumbnailSet",
  "id": "7b27dc0a-dc0a-7b27-0adc-277b0adc277b",
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

