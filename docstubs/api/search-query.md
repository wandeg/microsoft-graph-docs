---
title: "query"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# query

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
POST /search/query
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|requests|[searchRequest](../resources/searchrequest.md) collection||



## Response
If successful, this action returns a `200 OK` response code and a [searchResponse](../resources/searchresponse.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "search_query"
}
-->
``` http
POST https://graph.microsoft.com/beta/search/query

Content-type: application/json
Content-length: 570

{
  "requests": [
    {
      "@odata.type": "microsoft.graph.searchRequest",
      "entityTypes": [
        "String"
      ],
      "contentSources": [
        "Content Sources value"
      ],
      "query": {
        "@odata.type": "microsoft.graph.searchQuery",
        "query_string": {
          "@odata.type": "microsoft.graph.searchQueryString",
          "query": "Query value"
        }
      },
      "from": 4,
      "size": 4,
      "stored_fields": [
        "Stored_fields value"
      ],
      "enableTopResults": true
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.searchresponse)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 92

{
  "value": [
    {
      "@odata.type": "microsoft.graph.searchResponse"
    }
  ]
}
```

