---
title: "Add deviceStates"
description: "Add deviceStates by posting to the deviceStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceStates

Namespace: microsoft.graph

Add deviceStates by posting to the deviceStates collection.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||
|userName|String||
|deviceDisplayName|String||
|lastReportedDateTime|DateTimeOffset||
|state|Enumeration| Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|deviceId|String||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/devicemanagementintentdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementintentdevicestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2016-12-31T23:58:03.7571898+03:00",
  "state": "String",
  "deviceId": "Device Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintentdevicestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 384

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "e6d40166-0166-e6d4-6601-d4e66601d4e6",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2016-12-31T23:58:03.7571898+03:00",
  "state": "String",
  "deviceId": "Device Id value"
}
```

