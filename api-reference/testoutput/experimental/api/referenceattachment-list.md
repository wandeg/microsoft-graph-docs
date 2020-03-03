---
title: "List referenceAttachments"
description: "List properties and relationships of the referenceAttachment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List referenceAttachments

List properties and relationships of the [referenceAttachment](../resources/referenceattachment.md) objects.

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_referenceattachment"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.referenceAttachment not found
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
Content-Length: 594

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.referenceAttachment",
      "id": "9895a6d5-a6d5-9895-d5a6-9598d5a69598",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
      "name": "Name value",
      "contentType": "Content Type value",
      "size": 4,
      "isInline": true,
      "sourceUrl": "https://example.com/sourceUrl/",
      "providerType": "String",
      "thumbnailUrl": "https://example.com/thumbnailUrl/",
      "previewUrl": "https://example.com/previewUrl/",
      "permission": "String",
      "isFolder": true
    }
  ]
}
```

