---
title: "Update printService"
description: "Update the properties of a printService object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printService

Namespace: microsoft.graph

Update the properties of a [printService](../resources/printservice.md) object.

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
PATCH /print/services/{printServiceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [printService](../resources/printservice.md) object.

The following table shows the properties that are required when you create the [printService](../resources/printservice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [printService](../resources/printservice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printservice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/services/{printServiceId}
Content-type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.printService"
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
Content-Length: 103

{
  "@odata.type": "#microsoft.graph.printService",
  "id": "bd1c847a-847a-bd1c-7a84-1cbd7a841cbd"
}
```

