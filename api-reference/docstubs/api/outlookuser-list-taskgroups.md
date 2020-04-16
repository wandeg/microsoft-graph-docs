---
title: "List taskGroups"
description: "Get the outlookTaskGroups from the taskGroups navigation property."
author: "**TODO: Provide Github Name**"
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
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlooktaskgroup)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTaskGroup",
      "id": "47446577-6577-4744-7765-444777654447",
      "changeKey": "Change Key value",
      "isDefaultGroup": true,
      "name": "Name value",
      "groupKey": "7971407f-407f-7971-7f40-71797f407179"
    }
  ]
}
```

