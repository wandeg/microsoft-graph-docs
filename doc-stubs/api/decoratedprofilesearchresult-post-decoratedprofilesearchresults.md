---
title: "Create DecoratedProfileSearchResult"
description: "Create a new DecoratedProfileSearchResult object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create DecoratedProfileSearchResult

Namespace: microsoft.graph

Create a new [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

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
POST /decoratedProfileSearchResults
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

If successful, this method returns a `201 Created` response code and a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_decoratedprofilesearchresult_from_decoratedprofilesearchresults"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/decoratedProfileSearchResults
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
  "truncated": true,
  "@odata.type": "microsoft.graph.decoratedprofilesearchresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
  "id": "2280d58b-d58b-2280-8bd5-80228bd58022",
  "query": {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
  },
  "exactMatch": "Boolean"
}
```

