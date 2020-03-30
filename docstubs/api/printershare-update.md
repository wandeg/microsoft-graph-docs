---
title: "Update printerShare"
description: "Update the properties of a printerShare object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printerShare

Namespace: microsoft.graph

Update the properties of a [printerShare](../resources/printershare.md) object.

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
PATCH /print/printerShares/{printerShareId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [printerShare](../resources/printershare.md) object.

The following table shows the properties that are required when you create the [printerShare](../resources/printershare.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|createdDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printerShares/{printerShareId}
Content-type: application/json
Content-length: 79

{
  "@odata.type": "#microsoft.graph.printerShare",
  "name": "Name value"
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
Content-Length: 187

{
  "@odata.type": "#microsoft.graph.printerShare",
  "id": "c2bfbe94-be94-c2bf-94be-bfc294bebfc2",
  "name": "Name value",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00"
}
```

