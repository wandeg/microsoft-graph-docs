---
title: "Get outlookTaskGroup"
description: "Read properties and relationships of an outlookTaskGroup object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get outlookTaskGroup

Namespace: microsoft.graph

Read properties and relationships of an [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

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
GET /invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}
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
If successful, this method returns a `200 OK` response code and an [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}
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
{
  "value": {
    "@odata.type": "#microsoft.graph.outlookTaskGroup",
    "id": "e7ff486a-486a-e7ff-6a48-ffe76a48ffe7",
    "changeKey": "Change Key value",
    "isDefaultGroup": true,
    "name": "Name value",
    "groupKey": "4403b5f4-b5f4-4403-f4b5-0344f4b50344"
  }
}
```

