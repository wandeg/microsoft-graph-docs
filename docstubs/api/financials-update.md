---
title: "Update financials"
description: "Update the properties of a financials object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update financials

Namespace: microsoft.graph

Update the properties of a [financials](../resources/financials.md) object.

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
PATCH /financials
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [financials](../resources/financials.md) object.

The following table shows the properties that are required when you create the [financials](../resources/financials.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [financials](../resources/financials.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_financials"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials
Content-type: application/json
Content-length: 52

{
  "@odata.type": "#microsoft.graph.financials"
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
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.financials",
  "id": "5b8f9c7d-9c7d-5b8f-7d9c-8f5b7d9c8f5b"
}
```

