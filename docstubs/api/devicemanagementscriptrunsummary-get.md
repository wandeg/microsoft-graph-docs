---
title: "Get deviceManagementScriptRunSummary"
description: "Read properties and relationships of the deviceManagementScriptRunSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementScriptRunSummary

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.

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
If successful, this method returns a `200 OK` response code and [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementscriptrunsummary"
}
-->
``` http

```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementScriptRunSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 259

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
    "id": "e25f4606-4606-e25f-0646-5fe206465fe2",
    "successDeviceCount": 2,
    "errorDeviceCount": 0,
    "successUserCount": 0,
    "errorUserCount": 14
  }
}
```

