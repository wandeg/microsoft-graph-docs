---
title: "List sessions"
description: "List properties and relationships of the session objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sessions

Namespace: microsoft.graph.callRecords

List properties and relationships of the [session](../resources/session.md) objects.

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
GET /communications/callRecords/{callRecordId}/sessions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [session](../resources/session.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_session"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/callRecords/{callRecordId}/sessions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.session)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 881

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.callRecords.session",
      "id": "26004e0a-4e0a-2600-0a4e-00260a4e0026",
      "modalities": [
        "String"
      ],
      "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
      "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
      "caller": {
        "@odata.type": "microsoft.graph.callRecords.endpoint",
        "userAgent": {
          "@odata.type": "microsoft.graph.callRecords.userAgent",
          "headerValue": "Header Value value",
          "applicationVersion": "Application Version value"
        }
      },
      "callee": {
        "@odata.type": "microsoft.graph.callRecords.endpoint"
      },
      "failureInfo": {
        "@odata.type": "microsoft.graph.callRecords.failureInfo",
        "stage": "String",
        "reason": "Reason value"
      }
    }
  ]
}
```

