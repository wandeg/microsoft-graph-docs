---
title: "List deviceRunStates"
description: "Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceRunStates

Namespace: microsoft.graph

Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscriptdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicehealthscriptdevicestate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 889

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
      "id": "bfad9edc-9edc-bfad-dc9e-adbfdc9eadbf",
      "detectionState": "String",
      "lastStateUpdateDateTime": "2017-01-01T00:00:58.0820363+03:00",
      "expectedStateUpdateDateTime": "2017-01-01T00:01:38.580617+03:00",
      "lastSyncDateTime": "2016-12-31T23:56:56.1979703+03:00",
      "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
      "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
      "remediationScriptError": "Remediation Script Error value",
      "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
      "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
      "remediationState": "String"
    }
  ]
}
```

