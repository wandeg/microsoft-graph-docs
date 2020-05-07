---
title: "Create runSummary"
description: "Create a new runSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create runSummary

Namespace: microsoft.graph

Create a new runSummary object.

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
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
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
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|noIssueDetectedDeviceCount|Int32|**TODO: Add Description**|
|issueDetectedDeviceCount|Int32|**TODO: Add Description**|
|detectionScriptErrorDeviceCount|Int32|**TODO: Add Description**|
|detectionScriptPendingDeviceCount|Int32|**TODO: Add Description**|
|issueRemediatedDeviceCount|Int32|**TODO: Add Description**|
|remediationSkippedDeviceCount|Int32|**TODO: Add Description**|
|issueReoccurredDeviceCount|Int32|**TODO: Add Description**|
|remediationScriptErrorDeviceCount|Int32|**TODO: Add Description**|
|lastScriptRunDateTime|DateTimeOffset|**TODO: Add Description**|
|issueRemediatedCumulativeDeviceCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscriptrunsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-Type: application/json
Content-length: 546

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscriptrunsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "4f66a7ac-a7ac-4f66-aca7-664faca7664f",
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

