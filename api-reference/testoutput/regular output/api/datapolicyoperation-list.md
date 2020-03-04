---
title: "List dataPolicyOperations"
description: "List properties and relationships of the dataPolicyOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List dataPolicyOperations

Namespace: microsoft.graph

List properties and relationships of the [dataPolicyOperation](../resources/datapolicyoperation.md) objects.

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
GET /dataPolicyOperations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [dataPolicyOperation](../resources/datapolicyoperation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataPolicyOperations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.datapolicyoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataPolicyOperation",
      "id": "3680e807-e807-3680-07e8-803607e88036",
      "completedDateTime": "2017-01-01T00:02:34.4104649+03:00",
      "status": "String",
      "storageLocation": "Storage Location value",
      "userId": "User Id value",
      "submittedDateTime": "2016-12-31T23:57:08.0830502+03:00",
      "progress": "Double"
    }
  ]
}
```

