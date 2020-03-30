---
title: "Update windowsManagementAppHealthState"
description: "Update the properties of a windowsManagementAppHealthState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsManagementAppHealthState

Namespace: microsoft.graph

Update the properties of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.

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
PATCH /deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.

The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|healthState|Enumeration| Possible values are: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|String||
|lastCheckInDateTime|DateTimeOffset||
|deviceName|String||
|deviceOSVersion|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsmanagementapphealthstate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates/{windowsManagementAppHealthStateId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2017-01-01T00:00:21.1402098+00:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "b758c46b-c46b-b758-6bc4-58b76bc458b7",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2017-01-01T00:00:21.1402098+00:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

