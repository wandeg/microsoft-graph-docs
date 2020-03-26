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
GET /graph/query
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
|queryId|String||
|queryParams|[StringMapElement](../resources/stringmapelement.md) collection||



## Response
If successful, this function returns a `200 OK` response code and a [Result](../resources/result.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "result_query"
}
-->
``` http
GET https://graph.microsoft.com/beta/graph/query(queryId='parameterValue',queryParams=[
  {
    "@odata.type": "microsoft.graph.StringMapElement"
  }
])
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.result)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.Result",
      "id": "94a0ce1f-ce1f-94a0-1fce-a0941fcea094",
      "entities": {
        "@odata.type": "microsoft.graph.ResultEntities"
      },
      "aggregations": [
        {
          "@odata.type": "microsoft.graph.LIAggregations"
        }
      ],
      "metadata": {
        "@odata.type": "microsoft.graph.Metadata"
      }
    }
  ]
}
```

