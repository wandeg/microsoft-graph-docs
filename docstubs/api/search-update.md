---
title: "Update search"
description: "Update the properties of a search object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update search

Namespace: microsoft.graph

Update the properties of a [search](../resources/search.md) object.

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
PATCH /search
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [search](../resources/search.md) object.

The following table shows the properties that are required when you create the [search](../resources/search.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [search](../resources/search.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_search"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/search
Content-type: application/json
Content-length: 48

{
  "@odata.type": "#microsoft.graph.search"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 97

{
  "@odata.type": "#microsoft.graph.search",
  "id": "b3f72c7a-2c7a-b3f7-7a2c-f7b37a2cf7b3"
}
```

