---
title: "Update userFlaggingResource"
description: "Update the properties of a userFlaggingResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userFlaggingResource

Namespace: microsoft.graph

Update the properties of a [userFlaggingResource](../resources/userflaggingresource.md) object.

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
PATCH /userFlagging
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userFlaggingResource](../resources/userflaggingresource.md) object.

The following table shows the properties that are required when you create the [userFlaggingResource](../resources/userflaggingresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [userFlaggingResource](../resources/userflaggingresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_userflaggingresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/userFlagging
Content-type: application/json
Content-length: 62

{
  "@odata.type": "#microsoft.graph.userFlaggingResource"
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
Content-Length: 111

{
  "@odata.type": "#microsoft.graph.userFlaggingResource",
  "id": "ca4048bb-48bb-ca40-bb48-40cabb4840ca"
}
```

