---
title: "Update deviceStates"
description: "Update the properties of a deviceStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceStates

Namespace: microsoft.graph

Update the properties of a deviceStates object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.

The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|The time the embedded SIM device status was created. Generated service side.|
|modifiedDateTime|DateTimeOffset|The time the embedded SIM device status was last modified. Updated service side.|
|lastSyncDateTime|DateTimeOffset|The time the embedded SIM device last checked in. Updated service side.|
|universalIntegratedCircuitCardIdentifier|String|The Universal Integrated Circuit Card Identifier (UICCID) identifying the hardware onto which a profile is to be deployed.|
|deviceName|String|Device name to which the subscription was provisioned e.g. DESKTOP-JOE|
|userName|String|Username which the subscription was provisioned to e.g. joe@contoso.com|
|state|embeddedSIMDeviceStateValue|The state of the profile operation applied to the device. Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String|String description of the provisioning state.|



## Response
If successful, this method returns a `200 OK` response code and an updated [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicestates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-Type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "String",
  "stateDetails": "State Details value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "8d88956d-956d-8d88-6d95-888d6d95888d",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "String",
  "stateDetails": "State Details value"
}
```

