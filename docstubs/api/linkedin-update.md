---
title: "Update linkedIn"
description: "Update the properties of a linkedIn object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update linkedIn

Namespace: microsoft.graph

Update the properties of a [linkedIn](../resources/linkedin.md) object.

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
PATCH /linkedIn
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [linkedIn](../resources/linkedin.md) object.

The following table shows the properties that are required when you create the [linkedIn](../resources/linkedin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [linkedIn](../resources/linkedin.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_linkedin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/linkedIn
Content-type: application/json
Content-length: 50

{
  "@odata.type": "#microsoft.graph.linkedIn"
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
Content-Length: 99

{
  "@odata.type": "#microsoft.graph.linkedIn",
  "id": "2a6fc100-c100-2a6f-00c1-6f2a00c16f2a"
}
```

