---
title: "List itemAttachments"
description: "List properties and relationships of the itemAttachment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List itemAttachments

Namespace: microsoft.graph

List properties and relationships of the [itemAttachment](../resources/itemattachment.md) objects.

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
GET ** Collection URI for microsoft.graph.itemAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [itemAttachment](../resources/itemattachment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemattachment"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.itemAttachment not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemattachment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemAttachment",
      "id": "54731367-1367-5473-6713-735467137354",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "name": "Name value",
      "contentType": "Content Type value",
      "size": 4,
      "isInline": true
    }
  ]
}
```

