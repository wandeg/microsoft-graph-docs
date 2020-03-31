---
title: "Get DecoratedProfileSearchResult"
description: "Read properties and relationships of the DecoratedProfileSearchResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get DecoratedProfileSearchResult

Namespace: microsoft.graph

Read properties and relationships of the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

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
GET /decoratedProfileSearchResults/{decoratedProfileSearchResultsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_decoratedprofilesearchresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/decoratedProfileSearchResults/{decoratedProfileSearchResultsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.DecoratedProfileSearchResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 405

{
  "value": {
    "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
    "id": "f33daa8f-aa8f-f33d-8faa-3df38faa3df3",
    "query": {
      "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery",
      "email": "Email value",
      "firstName": "First Name value",
      "lastName": "Last Name value",
      "keywords": "Keywords value"
    },
    "exactMatch": true
  }
}
```

