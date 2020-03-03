---
title: "List enrollmentTroubleshootingEvents"
description: "List properties and relationships of the enrollmentTroubleshootingEvent objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List enrollmentTroubleshootingEvents

Namespace: microsoft.graph

List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) objects.

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
GET ** Collection URI for microsoft.graph.enrollmentTroubleshootingEvent not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_enrollmenttroubleshootingevent"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.enrollmentTroubleshootingEvent not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.enrollmenttroubleshootingevent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 623

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
      "id": "b7e9f5c5-f5c5-b7e9-c5f5-e9b7c5f5e9b7",
      "eventDateTime": "2017-01-01T00:01:24.8579345+03:00",
      "correlationId": "Correlation Id value",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "operatingSystem": "Operating System value",
      "osVersion": "Os Version value",
      "userId": "User Id value",
      "deviceId": "Device Id value",
      "enrollmentType": "String",
      "failureCategory": "String",
      "failureReason": "Failure Reason value"
    }
  ]
}
```

