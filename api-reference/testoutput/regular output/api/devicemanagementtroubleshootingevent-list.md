---
title: "List deviceManagementTroubleshootingEvents"
description: "List properties and relationships of the deviceManagementTroubleshootingEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List deviceManagementTroubleshootingEvents

Namespace: microsoft.graph

List properties and relationships of the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) objects.

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
GET /deviceManagement/troubleshootingEvents
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementtroubleshootingevent"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/troubleshootingEvents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementtroubleshootingevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 277

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
      "id": "9a0757eb-57eb-9a07-eb57-079aeb57079a",
      "eventDateTime": "2017-01-01T00:01:24.8579345+03:00",
      "correlationId": "Correlation Id value"
    }
  ]
}
```

