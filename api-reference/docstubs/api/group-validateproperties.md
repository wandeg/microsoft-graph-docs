---
title: "group: validateProperties"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# validateProperties

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /groups/{groupsId}/validateProperties
POST /me/joinedGroups/{groupId}/validateProperties
POST /users/{usersId}/joinedGroups/{groupId}/validateProperties
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|onBehalfOfUserId|Guid|**TODO: Add Description**|



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/validateProperties

Content-Type: application/json
Content-length: 148

{
  "displayName": "Display Name value",
  "mailNickname": "Mail Nickname value",
  "onBehalfOfUserId": "3ed52c23-2c23-3ed5-232c-d53e232cd53e"
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
HTTP/1.1 204 No Content
```

