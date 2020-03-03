---
title: "List importedWindowsAutopilotDeviceIdentityUploads"
description: "List properties and relationships of the importedWindowsAutopilotDeviceIdentityUpload objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List importedWindowsAutopilotDeviceIdentityUploads

List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) objects.

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
GET ** Collection URI for microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_importedwindowsautopilotdeviceidentityupload"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.importedwindowsautopilotdeviceidentityupload)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 269

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
      "id": "b89b18f2-18f2-b89b-f218-9bb8f2189bb8",
      "createdDateTimeUtc": "2016-12-31T23:58:05.5093446+03:00",
      "status": "String"
    }
  ]
}
```

