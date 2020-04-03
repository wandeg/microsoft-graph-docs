---
title: "List taskGroups"
description: "Get the outlookTaskGroups from the taskGroups navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List taskGroups

Namespace: microsoft.graph

Get the outlookTaskGroups from the taskGroups navigation property.

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
GET /me/outlook/taskGroups
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
If successful, this method returns a `200 OK` response code and a collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
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
      "id": "719e0123-0123-719e-2301-9e7123019e71",
      "changeKey": "Change Key value",
      "isDefaultGroup": true,
      "name": "Name value",
      "groupKey": "15950dce-0dce-1595-ce0d-9515ce0d9515"
    }
  ]
}
```

