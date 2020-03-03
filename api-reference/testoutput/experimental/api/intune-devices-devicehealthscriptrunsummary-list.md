---
title: "List deviceHealthScriptRunSummaries"
description: "List properties and relationships of the deviceHealthScriptRunSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceHealthScriptRunSummaries

Namespace: microsoft.graph

List properties and relationships of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.deviceHealthScriptRunSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicehealthscriptrunsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.deviceHealthScriptRunSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicehealthscriptrunsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 624

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
      "id": "994a6ada-6ada-994a-da6a-4a99da6a4a99",
      "noIssueDetectedDeviceCount": 10,
      "issueDetectedDeviceCount": 8,
      "detectionScriptErrorDeviceCount": 15,
      "detectionScriptPendingDeviceCount": 1,
      "issueRemediatedDeviceCount": 10,
      "remediationSkippedDeviceCount": 13,
      "issueReoccurredDeviceCount": 10,
      "remediationScriptErrorDeviceCount": 1,
      "lastScriptRunDateTime": "2016-12-31T23:58:05.1341989+03:00",
      "issueRemediatedCumulativeDeviceCount": 4
    }
  ]
}
```

