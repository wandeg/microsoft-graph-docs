---
title: "List sessions"
description: "Get the sessions from the sessions navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sessions

Namespace: microsoft.graph.callRecords

Get the sessions from the sessions navigation property.

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
GET /communications/callRecords/{callRecordId}/sessions
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
If successful, this method returns a `200 OK` response code and a collection of [session](../resources/session.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_session"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.session)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.callRecords.session",
      "id": "974db089-b089-974d-89b0-4d9789b04d97",
      "modalities": [
        "String"
      ],
      "startDateTime": "2017-01-01T00:03:24.4987822+03:00",
      "endDateTime": "2016-12-31T23:59:38.6819041+03:00",
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

