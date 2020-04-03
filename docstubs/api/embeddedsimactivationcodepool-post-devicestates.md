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
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object.

The following table shows the properties that are required when you create the [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|modifiedDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|universalIntegratedCircuitCardIdentifier|String||
|deviceName|String||
|userName|String||
|state|Enumeration| Possible values are: `notEvaluated`, `failed`, `installing`, `installed`, `deleting`, `error`, `deleted`, `removedByUser`.|
|stateDetails|String||



## Response
If successful, this method returns a `201 Created` response code and a [embeddedSIMDeviceState](../resources/embeddedsimdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_embeddedsimdevicestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "lastSyncDateTime": "2016-12-31T23:57:21.5163223+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.embeddedsimdevicestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 529

{
  "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
  "id": "6666ab97-ab97-6666-97ab-666697ab6666",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
  "modifiedDateTime": "2016-12-31T23:58:55.6791311+00:00",
  "lastSyncDateTime": "2016-12-31T23:57:21.5163223+00:00",
  "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
  "deviceName": "Device Name value",
  "userName": "User Name value",
  "state": "String",
  "stateDetails": "State Details value"
}
```

