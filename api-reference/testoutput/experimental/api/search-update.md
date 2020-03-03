---
title: "Update search"
description: "Update the properties of a search object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update search

Update the properties of a [search](../resources/search.md) object.

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
PATCH /search
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [search](../resources/search.md) object.

The following table shows the properties that are required when you create the [search](../resources/search.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [search](../resources/search.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_search"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/search
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
  "id": "52db7545-7545-52db-4575-db524575db52"
}
```

