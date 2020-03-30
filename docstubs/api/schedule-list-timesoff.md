---
title: "List timesOff"
description: "Get the timeOffs from the timesOff navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List timesOff

Namespace: microsoft.graph

Get the timeOffs from the timesOff navigation property.

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
GET /me/joinedGroups/{groupId}/team/schedule/timesOff
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [timeOff](../resources/timeoff.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_timeoff"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timesOff
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timeoff)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1120

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.timeOff",
      "id": "bf8cf545-f545-bf8c-45f5-8cbf45f58cbf",
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
        },
        "device": {
          "@odata.type": "microsoft.graph.identity"
        },
        "user": {
          "@odata.type": "microsoft.graph.identity"
        }
      },
      "sharedTimeOff": {
        "@odata.type": "microsoft.graph.timeOffItem",
        "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
        "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
        "theme": "String",
        "timeOffReasonId": "Time Off Reason Id value"
      },
      "draftTimeOff": {
        "@odata.type": "microsoft.graph.timeOffItem"
      },
      "userId": "User Id value"
    }
  ]
}
```

