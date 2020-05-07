---
title: "Create deviceRunStates"
description: "Create a new deviceRunStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceRunStates

Namespace: microsoft.graph

Create a new deviceRunStates object.

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
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|detectionState|runState|**TODO: Add Description**. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|expectedStateUpdateDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|preRemediationDetectionScriptOutput|String|**TODO: Add Description**|
|preRemediationDetectionScriptError|String|**TODO: Add Description**|
|remediationScriptError|String|**TODO: Add Description**|
|postRemediationDetectionScriptOutput|String|**TODO: Add Description**|
|postRemediationDetectionScriptError|String|**TODO: Add Description**|
|remediationState|remediationState|**TODO: Add Description**. Possible values are: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|



## Response

If successful, this method returns a `201 Created` response code and a [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscriptdevicestate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
Content-Type: application/json
Content-length: 535

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscriptdevicestate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "0286b1e3-b1e3-0286-e3b1-8602e3b18602",
  "detectionState": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "expectedStateUpdateDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "preRemediationDetectionScriptOutput": "String",
  "preRemediationDetectionScriptError": "String",
  "remediationScriptError": "String",
  "postRemediationDetectionScriptOutput": "String",
  "postRemediationDetectionScriptError": "String",
  "remediationState": "String"
}
```

