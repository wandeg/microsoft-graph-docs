---
title: "List files"
description: "Get the agreementFiles from the files navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List files

Namespace: microsoft.graph

Get the agreementFiles from the files navigation property.

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
GET /agreements/{agreementsId}/files
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [agreementFile](../resources/agreementfile.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agreementfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/agreements/{agreementsId}/files
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.agreementfile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 366

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agreementFile",
      "id": "b5790a1d-0a1d-b579-1d0a-79b51d0a79b5",
      "language": "Language value",
      "fileName": "File Name value",
      "fileData": {
        "@odata.type": "microsoft.graph.agreementFileData",
        "data": "ZGF0YQ=="
      },
      "isDefault": true
    }
  ]
}
```

