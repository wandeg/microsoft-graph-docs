---
title: "Add deviceRunStates"
description: "Add deviceRunStates by posting to the deviceRunStates collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceRunStates

Namespace: microsoft.graph

Add deviceRunStates by posting to the deviceRunStates collection.

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
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|detectionState|Enumeration| Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset||
|expectedStateUpdateDateTime|DateTimeOffset||
|lastSyncDateTime|DateTimeOffset||
|preRemediationDetectionScriptOutput|String||
|preRemediationDetectionScriptError|String||
|remediationScriptError|String||
|postRemediationDetectionScriptOutput|String||
|postRemediationDetectionScriptError|String||
|remediationState|Enumeration| Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscriptdevicestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
Content-type: application/json
Content-length: 760

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "String",
  "lastStateUpdateDateTime": "2017-01-01T00:02:15.8162309+03:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:11.0759599+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscriptdevicestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 809

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "e36b6a2a-6a2a-e36b-2a6a-6be32a6a6be3",
  "detectionState": "String",
  "lastStateUpdateDateTime": "2017-01-01T00:02:15.8162309+03:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:11.0759599+03:00",
  "lastSyncDateTime": "2017-01-01T00:03:05.8629729+03:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "String"
}
```

