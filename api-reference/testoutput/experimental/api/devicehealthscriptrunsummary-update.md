---
title: "Update deviceHealthScriptRunSummary"
description: "Update the properties of a deviceHealthScriptRunSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceHealthScriptRunSummary

Namespace: microsoft.graph

Update the properties of a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|noIssueDetectedDeviceCount|Int32|Number of devices for which the detection script did not find an issue and the device is healthy|
|issueDetectedDeviceCount|Int32|Number of devices for which the detection script found an issue|
|detectionScriptErrorDeviceCount|Int32|Number of devices on which the detection script execution encountered an error and did not complete|
|detectionScriptPendingDeviceCount|Int32|Number of devices which have not yet run the latest version of the device health script|
|issueRemediatedDeviceCount|Int32|Number of devices for which the remediation script was able to resolve the detected issue|
|remediationSkippedDeviceCount|Int32|Number of devices for which remediation was skipped|
|issueReoccurredDeviceCount|Int32|Number of devices for which the remediation script executed successfully but failed to resolve the detected issue|
|remediationScriptErrorDeviceCount|Int32|Number of devices for which the remediation script execution encountered an error and did not complete|
|lastScriptRunDateTime|DateTimeOffset|Last run time for the script across all devices|
|issueRemediatedCumulativeDeviceCount|Int32|Number of devices that were remediated over the last 30 days|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicehealthscriptrunsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:02:49.5824592+03:00",
  "issueRemediatedCumulativeDeviceCount": 4
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
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "788f1e96-1e96-788f-961e-8f78961e8f78",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:02:49.5824592+03:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

