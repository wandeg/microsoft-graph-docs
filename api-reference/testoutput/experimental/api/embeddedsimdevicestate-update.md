---
title: "Update embeddedSIMDeviceState"
description: "Update the properties of a embeddedSIMDeviceState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update embeddedSIMDeviceState

Namespace: microsoft.graph

Update the properties of a [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.

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
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.

The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|The time the embedded SIM device status was created. Generated service side.|
|modifiedDateTime|DateTimeOffset|The time the embedded SIM device status was last modified. Updated service side.|
|lastSyncDateTime|DateTimeOffset|The time the embedded SIM device last checked in. Updated service side.|
|universalIntegratedCircuitCardIdentifier|String|The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.|
|deviceName|String|Device name to which the subscription was provisioned e.g. DESKTOP-JOE|
|userName|String|Username which the subscription was provisioned to e.g. joe@contoso.com|
|state|Enumeration|The state of the profile operation applied to the device. Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|String description of the provisioning state.|



## Response
If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_embeddedsimdevicestate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/{embeddedSIMDeviceStateId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2016-12-31T23:56:56.1979703+03:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "String",
  "stateDetails": "State Details value"
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
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "0c6ac944-c944-0c6a-44c9-6a0c44c96a0c",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00",
  "lastSyncDateTime": "2016-12-31T23:56:56.1979703+03:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "String",
  "stateDetails": "State Details value"
}
```

