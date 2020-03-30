---
title: "Create payloadResponse"
description: "Create a new payloadResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create payloadResponse

Namespace: microsoft.graph

Create a new [payloadResponse](../resources/payloadresponse.md) object.

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
POST /payloadResponse
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [payloadResponse](../resources/payloadresponse.md) object.

The following table shows the properties that are required when you create the [payloadResponse](../resources/payloadresponse.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [payloadResponse](../resources/payloadresponse.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_payloadresponse_from_payloadresponse"
}
-->
``` http
POST https://graph.microsoft.com/beta/payloadResponse
Content-type: application/json
Content-length: 57

{
  "@odata.type": "#microsoft.graph.payloadResponse"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.payloadresponse"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 106

{
  "@odata.type": "#microsoft.graph.payloadResponse",
  "id": "a8aaf2d3-f2d3-a8aa-d3f2-aaa8d3f2aaa8"
}
```

