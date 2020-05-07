---
title: "Update DecoratedProfileSearchResult"
description: "Update the properties of a DecoratedProfileSearchResult object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update DecoratedProfileSearchResult

Namespace: microsoft.graph

Update the properties of a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

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
PATCH /decoratedProfileSearchResults/{decoratedProfileSearchResultsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

The following table shows the properties that are required when you create the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|query|[DecoratedProfileSearchQuery](../resources/decoratedprofilesearchquery.md)|**TODO: Add Description**|
|exactMatch|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_decoratedprofilesearchresult"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/decoratedProfileSearchResults/{decoratedProfileSearchResultsId}
Content-Type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
  "query": {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
  },
  "exactMatch": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
  "id": "a9a04de3-4de3-a9a0-e34d-a0a9e34da0a9",
  "query": {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
  },
  "exactMatch": "Boolean"
}
```

