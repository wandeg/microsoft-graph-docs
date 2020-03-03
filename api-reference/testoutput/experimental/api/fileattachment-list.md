---
title: "List fileAttachments"
description: "List properties and relationships of the fileAttachment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List fileAttachments

Namespace: microsoft.graph

List properties and relationships of the [fileAttachment](../resources/fileattachment.md) objects.

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
GET ** Collection URI for microsoft.graph.fileAttachment not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [fileAttachment](../resources/fileattachment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_fileattachment"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.fileAttachment not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.fileattachment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 465

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fileAttachment",
      "id": "599d1c24-1c24-599d-241c-9d59241c9d59",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "name": "Name value",
      "contentType": "Content Type value",
      "size": 4,
      "isInline": true,
      "contentId": "Content Id value",
      "contentLocation": "Content Location value",
      "contentBytes": "Y29udGVudEJ5dGVz"
    }
  ]
}
```

