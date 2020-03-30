---
title: "Update deviceManagementScriptRunSummary"
description: "Update the properties of a deviceManagementScriptRunSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementScriptRunSummary

Namespace: microsoft.graph

Update the properties of a [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.

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

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.

The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|successDeviceCount|Int32||
|errorDeviceCount|Int32||
|successUserCount|Int32||
|errorUserCount|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementscriptrunsummary"
}
-->
``` http

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
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "61be0438-0438-61be-3804-be613804be61",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

