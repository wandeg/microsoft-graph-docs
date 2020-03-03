---
title: "List updateRecordingStatusOperations"
description: "List properties and relationships of the updateRecordingStatusOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List updateRecordingStatusOperations

List properties and relationships of the [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) objects.

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
GET ** Collection URI for microsoft.graph.updateRecordingStatusOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_updaterecordingstatusoperation"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.updateRecordingStatusOperation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.updaterecordingstatusoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 403

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.updateRecordingStatusOperation",
      "id": "ee013eab-3eab-ee01-ab3e-01eeab3e01ee",
      "status": "String",
      "clientContext": "Client Context value",
      "resultInfo": {
        "@odata.type": "microsoft.graph.ResultInfo",
        "code": 4,
        "subcode": 7,
        "message": "Message value"
      }
    }
  ]
}
```

