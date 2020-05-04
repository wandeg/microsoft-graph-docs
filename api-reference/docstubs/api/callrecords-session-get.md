---
title: "Get session"
description: "Read properties and relationships of a session object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get session

Namespace: microsoft.graph.callRecords

Read properties and relationships of a [session](../resources/callrecords-session.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /communications/callRecords/{callRecordId}/sessions/{sessionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [session](../resources/callrecords-session.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_session"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions/{sessionId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callRecords.session"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.callRecords.session",
    "id": "f1f4f9dc-f9dc-f1f4-dcf9-f4f1dcf9f4f1",
    "modalities": [
      "String"
    ],
    "startDateTime": "2017-01-01T00:02:48.9283739+03:00",
    "endDateTime": "2016-12-31T23:59:31.7607156+03:00",
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
}
```

