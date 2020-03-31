---
title: "Create DecoratedProfileSearchResult"
description: "Create a new DecoratedProfileSearchResult object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create DecoratedProfileSearchResult

Namespace: microsoft.graph

Create a new [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

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
POST /decoratedProfileSearchResults
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.

The following table shows the properties that are required when you create the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|query|[DecoratedProfileSearchQuery](../resources/decoratedprofilesearchquery.md)||
|exactMatch|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_decoratedprofilesearchresult_from_decoratedprofilesearchresults"
}
-->
``` http
POST https://graph.microsoft.com/beta/decoratedProfileSearchResults
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
  "query": {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery",
    "email": "Email value",
    "firstName": "First Name value",
    "lastName": "Last Name value",
    "keywords": "Keywords value"
  },
  "exactMatch": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.decoratedprofilesearchresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 366

{
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
```

