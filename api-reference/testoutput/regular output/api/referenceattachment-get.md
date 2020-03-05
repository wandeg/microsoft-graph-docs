---
title: "Get referenceAttachment"
description: "Read properties and relationships of the referenceAttachment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get referenceAttachment

Namespace: microsoft.graph

Read properties and relationships of the [referenceAttachment](../resources/referenceattachment.md) object.

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
GET ** Entity URI for microsoft.graph.referenceAttachment not found
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
If successful, this method returns a `200 OK` response code and [referenceAttachment](../resources/referenceattachment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_referenceattachment"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.referenceAttachment not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.referenceAttachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 305

{
  "value": {
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "id": "6432d743-d743-6432-43d7-326443d73264",
    "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
    "name": "Name value",
    "contentType": "Content Type value",
    "size": 4,
    "isInline": true
  }
}
```

