---
title: "Get deviceHealthScriptRunSummary"
description: "Read properties and relationships of the deviceHealthScriptRunSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceHealthScriptRunSummary

Namespace: microsoft.graph

Read properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

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
GET /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
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
If successful, this method returns a `200 OK` response code and [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscriptrunsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 586

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
    "id": "9be74e26-4e26-9be7-264e-e79b264ee79b",
    "noIssueDetectedDeviceCount": 10,
    "issueDetectedDeviceCount": 8,
    "detectionScriptErrorDeviceCount": 15,
    "detectionScriptPendingDeviceCount": 1,
    "issueRemediatedDeviceCount": 10,
    "remediationSkippedDeviceCount": 13,
    "issueReoccurredDeviceCount": 10,
    "remediationScriptErrorDeviceCount": 1,
    "lastScriptRunDateTime": "2016-12-31T23:59:45.1470112+00:00",
    "issueRemediatedCumulativeDeviceCount": 4
  }
}
```

