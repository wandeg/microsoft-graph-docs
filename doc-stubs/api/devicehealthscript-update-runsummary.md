---
title: "Update runSummary"
description: "Update the properties of a runSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update runSummary

Namespace: microsoft.graph

Update the properties of a runSummary object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

The following table shows the properties that are required when you create the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the device health script run summary entity. This property is read-only.|
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
<!-- {
  "blockType": "request",
  "name": "update_runsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-Type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": "Integer",
  "issueDetectedDeviceCount": "Integer",
  "detectionScriptErrorDeviceCount": "Integer",
  "detectionScriptPendingDeviceCount": "Integer",
  "issueRemediatedDeviceCount": "Integer",
  "remediationSkippedDeviceCount": "Integer",
  "issueReoccurredDeviceCount": "Integer",
  "remediationScriptErrorDeviceCount": "Integer",
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": "Integer"
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
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptRunSummary",
  "id": "3dac74d0-74d0-3dac-d074-ac3dd074ac3d",
  "noIssueDetectedDeviceCount": "Integer",
  "issueDetectedDeviceCount": "Integer",
  "detectionScriptErrorDeviceCount": "Integer",
  "detectionScriptPendingDeviceCount": "Integer",
  "issueRemediatedDeviceCount": "Integer",
  "remediationSkippedDeviceCount": "Integer",
  "issueReoccurredDeviceCount": "Integer",
  "remediationScriptErrorDeviceCount": "Integer",
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": "Integer"
}
```

