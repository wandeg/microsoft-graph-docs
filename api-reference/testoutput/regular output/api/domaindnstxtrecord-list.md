---
title: "List domainDnsTxtRecords"
description: "List properties and relationships of the domainDnsTxtRecord objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domainDnsTxtRecords

Namespace: microsoft.graph

List properties and relationships of the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) objects.

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
GET ** Collection URI for microsoft.graph.domainDnsTxtRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnstxtrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.domainDnsTxtRecord not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domaindnstxtrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 350

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainDnsTxtRecord",
      "id": "9086ef6d-ef6d-9086-6def-86906def8690",
      "isOptional": true,
      "label": "Label value",
      "recordType": "Record Type value",
      "supportedService": "Supported Service value",
      "ttl": 3,
      "text": "Text value"
    }
  ]
}
```

