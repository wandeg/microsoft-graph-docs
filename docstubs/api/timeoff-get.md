---
title: "Get timeOff"
description: "Read properties and relationships of the timeOff object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get timeOff

Namespace: microsoft.graph

Read properties and relationships of the [timeOff](../resources/timeoff.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/timesOff/{timeOffId}
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
If successful, this method returns a `200 OK` response code and [timeOff](../resources/timeoff.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_timeoff"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timesOff/{timeOffId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "value": {
    "@odata.type": "#microsoft.graph.timeOff",
    "id": "9f5898e0-98e0-9f58-e098-589fe098589f",
    "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
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
      "startDateTime": "2016-12-31T23:58:03.4514069+03:00",
      "endDateTime": "2017-01-01T00:00:11.5602866+03:00",
      "theme": "String",
      "timeOffReasonId": "Time Off Reason Id value"
    },
    "draftTimeOff": {
      "@odata.type": "microsoft.graph.timeOffItem"
    },
    "userId": "User Id value"
  }
}
```

