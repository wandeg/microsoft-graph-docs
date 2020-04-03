---
title: "List calendarGroups"
description: "Get the calendarGroups from the calendarGroups navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List calendarGroups

Namespace: microsoft.graph

Get the calendarGroups from the calendarGroups navigation property.

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
GET /me/calendarGroups
GET /users/{usersId}/calendarGroups
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
If successful, this method returns a `200 OK` response code and a collection of [calendarGroup](../resources/calendargroup.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/calendarGroups
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendargroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendarGroup",
      "id": "e4cf93e5-93e5-e4cf-e593-cfe4e593cfe4",
      "name": "Name value",
      "classId": "6506ca4a-ca4a-6506-4aca-06654aca0665",
      "changeKey": "Change Key value"
    }
  ]
}
```

