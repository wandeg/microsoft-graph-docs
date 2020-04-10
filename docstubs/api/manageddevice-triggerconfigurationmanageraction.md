---
title: "managedDevice: triggerConfigurationManagerAction"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# triggerConfigurationManagerAction

Namespace: microsoft.graph



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
POST /me/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /users/{usersId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|configurationManagerAction|[configurationManagerAction](../resources/configurationmanageraction.md)||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "manageddevice_triggerconfigurationmanageraction"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction

Content-type: application/json
Content-length: 134

{
  "configurationManagerAction": {
    "@odata.type": "microsoft.graph.configurationManagerAction",
    "action": "String"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

