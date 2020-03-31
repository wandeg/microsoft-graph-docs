---
title: "Update external"
description: "Update the properties of a external object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update external

Namespace: microsoft.graph

Update the properties of a [external](../resources/external.md) object.

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
PATCH /external
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [external](../resources/external.md) object.

The following table shows the properties that are required when you create the [external](../resources/external.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [external](../resources/external.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_external"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/external
Content-type: application/json
Content-length: 50

{
  "@odata.type": "#microsoft.graph.external"
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
  "@odata.type": "#microsoft.graph.external",
  "id": "54b2fa73-fa73-54b2-73fa-b25473fab254"
}
```

