---
title: "List windowsManagementAppHealthSummaries"
description: "List properties and relationships of the windowsManagementAppHealthSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List windowsManagementAppHealthSummaries

List properties and relationships of the [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) objects.

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
GET ** Collection URI for microsoft.graph.windowsManagementAppHealthSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthSummary](../resources/windowsmanagementapphealthsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsmanagementapphealthsummary"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.windowsManagementAppHealthSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.windowsmanagementapphealthsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
      "id": "ac84d481-d481-ac84-81d4-84ac81d484ac",
      "healthyDeviceCount": 2,
      "unhealthyDeviceCount": 4,
      "unknownDeviceCount": 2
    }
  ]
}
```

