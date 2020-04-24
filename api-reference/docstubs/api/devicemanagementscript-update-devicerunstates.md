---
title: "Update deviceRunStates"
description: "Update the properties of a deviceRunStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceRunStates

Namespace: microsoft.graph

Update the properties of a deviceRunStates object.

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
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object.

The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|runState|runState|State of latest run of the device management script. Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|resultMessage|String|Details of execution output.|
|lastStateUpdateDateTime|DateTimeOffset|Latest time the device management script executes.|
|errorCode|Int32|Error code corresponding to erroneous execution of the device management script.|
|errorDescription|String|Error description corresponding to erroneous execution of the device management script.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/devicemanagementscriptdevicestate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicerunstates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "String",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:30.8589467+03:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
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
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "faab363a-363a-faab-3a36-abfa3a36abfa",
  "runState": "String",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:30.8589467+03:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

