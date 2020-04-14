---
title: "Get presence"
description: "Read properties and relationships of the presence object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get presence

Namespace: microsoft.graph

Read properties and relationships of the [presence](../resources/presence.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/presence
GET /users/{usersId}/presence
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
If successful, this method returns a `200 OK` response code and [presence](../resources/presence.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_presence"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/presence
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.presence"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 200

{
  "value": {
    "@odata.type": "#microsoft.graph.presence",
    "id": "c2485198-5198-c248-9851-48c2985148c2",
    "availability": "Availability value",
    "activity": "Activity value"
  }
}
```

