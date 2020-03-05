---
title: "Get outlookItem"
description: "Read properties and relationships of the outlookItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get outlookItem

Namespace: microsoft.graph

Read properties and relationships of the [outlookItem](../resources/outlookitem.md) object.

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
GET ** Entity URI for microsoft.graph.outlookItem not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [outlookItem](../resources/outlookitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlookitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.outlookItem not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 343

{
  "value": {
    "@odata.type": "#microsoft.graph.outlookItem",
    "id": "fda0099c-099c-fda0-9c09-a0fd9c09a0fd",
    "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
    "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ]
  }
}
```

