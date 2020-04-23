---
title: "List contentTypes"
description: "Get the contentTypes from the contentTypes navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List contentTypes

Namespace: microsoft.graph

Get the contentTypes from the contentTypes navigation property.

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
GET /sites/{sitesId}/contentTypes
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
If successful, this method returns a `200 OK` response code and a collection of [contentType](../resources/contenttype.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/contentTypes
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.contenttype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contentType",
      "id": "91739170-9170-9173-7091-739170917391",
      "description": "Description value",
      "group": "Group value",
      "hidden": true,
      "inheritedFrom": {
        "@odata.type": "microsoft.graph.itemReference",
        "driveId": "Drive Id value",
        "driveType": "Drive Type value",
        "id": "Id value",
        "name": "Name value",
        "path": "Path value",
        "shareId": "Share Id value",
        "sharepointIds": {
          "@odata.type": "microsoft.graph.sharepointIds",
          "listId": "List Id value",
          "listItemId": "List Item Id value",
          "listItemUniqueId": "List Item Unique Id value",
          "siteId": "Site Id value",
          "siteUrl": "https://example.com/siteUrl/",
          "webId": "Web Id value"
        }
      },
      "name": "Name value",
      "order": {
        "@odata.type": "microsoft.graph.contentTypeOrder",
        "default": true,
        "position": 8
      },
      "parentId": "Parent Id value",
      "readOnly": true,
      "sealed": true
    }
  ]
}
```

