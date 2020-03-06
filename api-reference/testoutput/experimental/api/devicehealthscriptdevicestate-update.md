---
title: "Update deviceHealthScriptDeviceState"
description: "Update the properties of a deviceHealthScriptDeviceState object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceHealthScriptDeviceState

Namespace: microsoft.graph

Update the properties of a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|detectionState|Enumeration|Detection state from the lastest device health script execution. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|The last timestamp of when the device health script executed|
|expectedStateUpdateDateTime|DateTimeOffset|The next timestamp of when the device health script is expected to execute|
|lastSyncDateTime|DateTimeOffset|The last time that Intune Managment Extension synced with Intune|
|preRemediationDetectionScriptOutput|String|Output of the detection script before remediation|
|preRemediationDetectionScriptError|String|Error from the detection script before remediation|
|remediationScriptError|String|Error output of the remediation script|
|postRemediationDetectionScriptOutput|String|Detection script output after remediation|
|postRemediationDetectionScriptError|String|Error from the detection script after remediation|
|remediationState|Enumeration|Remediation state from the lastest device health script execution. Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicehealthscriptdevicestate"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 759

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
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
Content-Length: 808

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
```

