---
title: "Update taskGroups"
description: "Update the properties of a taskGroups object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update taskGroups

Namespace: microsoft.graph

Update the properties of a taskGroups object.

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
PATCH /invitations/{invitationsId}/invitedUser/outlook/taskGroups
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [outlookTaskGroup](../resources/outlooktaskgroup.md) object.

The following table shows the properties that are required when you create the [outlookTaskGroup](../resources/outlooktaskgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|changeKey|String|**TODO: Add Description**|
|isDefaultGroup|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|groupKey|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_taskgroups"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/outlook/taskGroups
Content-Type: application/json
Content-length: 201

{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "4403b5f4-b5f4-4403-f4b5-0344f4b50344"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookTaskGroup",
  "id": "e7ff486a-486a-e7ff-6a48-ffe76a48ffe7",
  "changeKey": "Change Key value",
  "isDefaultGroup": true,
  "name": "Name value",
  "groupKey": "4403b5f4-b5f4-4403-f4b5-0344f4b50344"
}
```

