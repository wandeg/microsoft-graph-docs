---
title: "Add shared"
description: "Add shared by posting to the shared collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add shared

Add shared by posting to the shared collection.

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
POST /me/insights/shared/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the sharedInsight object.

The following table shows the properties that are required when you create the sharedInsight.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastShared|[sharingDetail](../resources/sharingDetail.md)||
|sharingHistory|[sharingDetail](../resources/sharingDetail.md) collection||
|resourceVisualization|[resourceVisualization](../resources/resourceVisualization.md)||
|resourceReference|[resourceReference](../resources/resourceReference.md)||



## Response
If successful, this method returns a `201 Created` response code and a [sharedInsight](../resources/sharedinsight.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sharedinsight_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/insights/shared
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "Display Name value",
      "id": "Id value",
      "address": "Address value"
    },
    "sharedDateTime": "2016-12-31T23:59:25.6718097+03:00",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharedinsight"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1313

{
  "@odata.type": "#microsoft.graph.sharedInsight",
  "id": "f61710fa-10fa-f617-fa10-17f6fa1017f6",
  "lastShared": {
    "@odata.type": "microsoft.graph.sharingDetail",
    "sharedBy": {
      "@odata.type": "microsoft.graph.insightIdentity",
      "displayName": "Display Name value",
      "id": "Id value",
      "address": "Address value"
    },
    "sharedDateTime": "2016-12-31T23:59:25.6718097+03:00",
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
```

