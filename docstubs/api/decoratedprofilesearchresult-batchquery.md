---
title: "batchQuery"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# batchQuery

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /decoratedProfileSearchResults/batchQuery
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|queries|[DecoratedProfileSearchQuery](../resources/decoratedprofilesearchquery.md) collection||



## Response
If successful, this function returns a `200 OK` response code and a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "decoratedprofilesearchresult_batchquery"
}
-->
``` http
GET https://graph.microsoft.com/beta/decoratedProfileSearchResults/batchQuery(queries=[
  {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
  }
])
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.decoratedprofilesearchresult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
      "id": "4ea4074d-074d-4ea4-4d07-a44e4d07a44e",
      "query": {
        "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
      },
      "exactMatch": true
    }
  ]
}
```

