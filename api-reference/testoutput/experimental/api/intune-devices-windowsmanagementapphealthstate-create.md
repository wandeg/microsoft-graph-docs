---
title: "Create windowsManagementAppHealthState"
description: "Create a new windowsManagementAppHealthState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsManagementAppHealthState

Namespace: microsoft.graph

Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.

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
POST /deviceAppManagement/windowsManagementApp/healthStates
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.

The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|healthState|Enumeration|Windows management app health state. Possible values are: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|String|Windows management app installed version.|
|lastCheckInDateTime|DateTimeOffset|Windows management app last check-in time.|
|deviceName|String|Name of the device on which Windows management app is installed.|
|deviceOSVersion|String|Windows 10 OS version of the device on which Windows management app is installed.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsmanagementapphealthstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceAppManagement/windowsManagementApp/healthStates
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsmanagementapphealthstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "5abfe192-e192-5abf-92e1-bf5a92e1bf5a",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2016-12-31T23:58:23.4652469+03:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

