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

## HTTP request
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

## Examples

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
      "id": "70c86c1f-6c1f-70c8-1f6c-c8701f6cc870",
      "eventDateTime": "2016-12-31T23:57:35.6099262+03:00",
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

