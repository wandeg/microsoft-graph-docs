---
title: "List referenceAttachments"
description: "List properties and relationships of the referenceAttachment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List referenceAttachments

Namespace: microsoft.graph

List properties and relationships of the [referenceAttachment](../resources/referenceattachment.md) objects.

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
GET ** Collection URI for microsoft.graph.referenceAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [referenceAttachment](../resources/referenceattachment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_referenceattachment"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.referenceAttachment not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.referenceattachment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.referenceAttachment",
      "id": "6432d743-d743-6432-43d7-326443d73264",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "name": "Name value",
      "contentType": "Content Type value",
      "size": 4,
      "isInline": true
    }
  ]
}
```

