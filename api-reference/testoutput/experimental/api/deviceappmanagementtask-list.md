---
title: "List deviceAppManagementTasks"
description: "List properties and relationships of the deviceAppManagementTask objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceAppManagementTasks

Namespace: microsoft.graph

List properties and relationships of the [deviceAppManagementTask](../resources/deviceappmanagementtask.md) objects.

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
GET /deviceAppManagement/deviceAppManagementTasks
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceAppManagementTask](../resources/deviceappmanagementtask.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_deviceappmanagementtask"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/deviceAppManagementTasks
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.deviceappmanagementtask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 571

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAppManagementTask",
      "id": "81fcc215-c215-81fc-15c2-fc8115c2fc81",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "dueDateTime": "2017-01-01T00:01:36.4685818+03:00",
      "category": "String",
      "priority": "String",
      "creator": "Creator value",
      "creatorNotes": "Creator Notes value",
      "assignedTo": "Assigned To value",
      "status": "String"
    }
  ]
}
```

