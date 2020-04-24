---
title: "List deviceRunStates"
description: "Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List deviceRunStates

Namespace: microsoft.graph

Get the deviceHealthScriptDeviceStates from the deviceRunStates navigation property.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptDeviceState](../resources/devicehealthscriptdevicestate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscriptdevicestate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicehealthscriptdevicestate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
      "id": "97e5e797-e797-97e5-97e7-e59797e7e597",
      "detectionState": "String",
      "lastStateUpdateDateTime": "2017-01-01T00:02:30.8589467+03:00",
      "expectedStateUpdateDateTime": "2016-12-31T23:56:35.0146324+03:00",
      "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
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

