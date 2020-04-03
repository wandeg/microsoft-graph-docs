---
title: "Update deviceManagementReports"
description: "Update the properties of a deviceManagementReports object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementReports

Namespace: microsoft.graph

Update the properties of a [deviceManagementReports](../resources/devicemanagementreports.md) object.

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
PATCH /deviceManagement/reports
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementReports](../resources/devicemanagementreports.md) object.

The following table shows the properties that are required when you create the [deviceManagementReports](../resources/devicemanagementreports.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/devicemanagementreports.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementreports"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
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
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "21a4201b-201b-21a4-1b20-a4211b20a421"
}
```

