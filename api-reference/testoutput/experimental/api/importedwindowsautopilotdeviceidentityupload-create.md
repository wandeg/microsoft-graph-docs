---
title: "Create importedWindowsAutopilotDeviceIdentityUpload"
description: "Create a new importedWindowsAutopilotDeviceIdentityUpload object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create importedWindowsAutopilotDeviceIdentityUpload

Namespace: microsoft.graph

Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object.

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
POST ** Collection URI for microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object.

The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTimeUtc|DateTimeOffset|DateTime when the entity is created.|
|status|Enumeration|Upload status. Possible values are: `noUpload`, `pending`, `complete`, `error`.|



## Response
If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_importedwindowsautopilotdeviceidentityupload_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload not found
Content-type: application/json
Content-length: 171

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:58:32.5709497+03:00",
  "status": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedwindowsautopilotdeviceidentityupload"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 220

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "7579b981-b981-7579-81b9-797581b97975",
  "createdDateTimeUtc": "2016-12-31T23:58:32.5709497+03:00",
  "status": "String"
}
```

