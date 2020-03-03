---
title: "List workbookRangeFormats"
description: "List properties and relationships of the workbookRangeFormat objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookRangeFormats

Namespace: microsoft.graph

List properties and relationships of the [workbookRangeFormat](../resources/workbookrangeformat.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookRangeFormat not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookRangeFormat](../resources/workbookrangeformat.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookrangeformat"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeFormat not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookrangeformat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 354

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookRangeFormat",
      "id": "ce2c6c73-6c73-ce2c-736c-2cce736c2cce",
      "columnWidth": "Double",
      "horizontalAlignment": "Horizontal Alignment value",
      "rowHeight": "Double",
      "verticalAlignment": "Vertical Alignment value",
      "wrapText": true
    }
  ]
}
```

