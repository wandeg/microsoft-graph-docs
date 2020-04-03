---
title: "Get windowsManagementAppHealthState"
description: "Read properties and relationships of the windowsManagementAppHealthState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsManagementAppHealthState

Namespace: microsoft.graph

Read properties and relationships of the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.

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
GET /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
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
If successful, this method returns a `200 OK` response code and [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsmanagementapphealthstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 381

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
    "id": "9b7a28ff-28ff-9b7a-ff28-7a9bff287a9b",
    "healthState": "String",
    "installedVersion": "Installed Version value",
    "lastCheckInDateTime": "2017-01-01T00:01:51.930237+00:00",
    "deviceName": "Device Name value",
    "deviceOSVersion": "Device OSVersion value"
  }
}
```

