---
title: "Get outlookTaskGroup"
description: "Read properties and relationships of the outlookTaskGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get outlookTaskGroup

Namespace: microsoft.graph

Read properties and relationships of the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

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
GET /me/outlook/taskGroups/{outlookTaskGroupId}
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
If successful, this method returns a `200 OK` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/{outlookTaskGroupId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 281

{
  "value": {
    "@odata.type": "#microsoft.graph.outlookTaskGroup",
    "id": "f4bc2b74-2b74-f4bc-742b-bcf4742bbcf4",
    "changeKey": "Change Key value",
    "isDefaultGroup": true,
    "name": "Name value",
    "groupKey": "52e10844-0844-52e1-4408-e1524408e152"
  }
}
```

