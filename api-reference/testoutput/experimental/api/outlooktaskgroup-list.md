---
title: "List outlookTaskGroups"
description: "List properties and relationships of the outlookTaskGroup objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List outlookTaskGroups

Namespace: microsoft.graph

List properties and relationships of the [outlookTaskGroup](../resources/outlooktaskgroup.md) objects.

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
GET /me/outlook/taskGroups
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/outlook/taskGroups
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlooktaskgroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTaskGroup",
      "id": "40c340e6-40e6-40c3-e640-c340e640c340",
      "changeKey": "Change Key value",
      "isDefaultGroup": true,
      "name": "Name value",
      "groupKey": "27262869-2869-2726-6928-262769282627"
    }
  ]
}
```

