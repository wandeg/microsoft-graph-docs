---
title: "Get deviceHealthScriptDeviceState"
description: "Read properties and relationships of the deviceHealthScriptDeviceState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceHealthScriptDeviceState

Namespace: microsoft.graph

Read properties and relationships of the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
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
If successful, this method returns a `200 OK` response code and [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscriptdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceHealthScriptDeviceState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 852

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
    "id": "993a7bc3-7bc3-993a-c37b-3a99c37b3a99",
    "detectionState": "String",
    "lastStateUpdateDateTime": "2016-12-31T23:59:16.4588852+03:00",
    "expectedStateUpdateDateTime": "2016-12-31T23:57:40.8293183+03:00",
    "lastSyncDateTime": "2016-12-31T23:56:30.9655764+03:00",
    "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
    "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
    "remediationScriptError": "Remediation Script Error value",
    "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
    "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
    "remediationState": "String"
  }
}
```

