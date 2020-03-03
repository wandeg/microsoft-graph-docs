---
title: "List windowsManagementAppHealthStates"
description: "List properties and relationships of the windowsManagementAppHealthState objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsManagementAppHealthStates

Namespace: microsoft.graph

List properties and relationships of the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) objects.

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
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsmanagementapphealthstate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/windowsManagementApp/healthStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsmanagementapphealthstate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5abfe192-e192-5abf-92e1-bf5a92e1bf5a",
      "healthState": "String",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```

