---
title: "Add healthStates"
description: "Add healthStates by posting to the healthStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add healthStates

Namespace: microsoft.graph

Add healthStates by posting to the healthStates collection.

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
POST /deviceAppManagement/windowsManagementApp/healthStates/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.

The following table shows the properties that are required when you create the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|healthState|Enumeration|Windows management app health state. Possible values are: `unknown`, `healthy`, `unhealthy`.|
|installedVersion|String|Windows management app installed version.|
|lastCheckInDateTime|DateTimeOffset|Windows management app last check-in time.|
|deviceName|String|Name of the device on which Windows management app is installed.|
|deviceOSVersion|String|Windows 10 OS version of the device on which Windows management app is installed.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object in the response body.

## Examples

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
Content-length: 299

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2017-01-01T00:00:34.709818+03:00",
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
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "9ff70d22-0d22-9ff7-220d-f79f220df79f",
  "healthState": "String",
  "installedVersion": "Installed Version value",
  "lastCheckInDateTime": "2017-01-01T00:00:34.709818+03:00",
  "deviceName": "Device Name value",
  "deviceOSVersion": "Device OSVersion value"
}
```

