---
title: "group: evaluateDynamicMembership"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# evaluateDynamicMembership

Namespace: microsoft.graph



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
POST /groups/{groupsId}/evaluateDynamicMembership
POST /me/joinedGroups/{groupId}/evaluateDynamicMembership
POST /users/{usersId}/joinedGroups/{groupId}/evaluateDynamicMembership
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
|memberId|String||



## Response
If successful, this action returns a `200 OK` response code and a [evaluateDynamicMembershipResult](../resources/evaluatedynamicmembershipresult.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "group_evaluatedynamicmembership"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/evaluateDynamicMembership

Content-type: application/json
Content-length: 37

{
  "memberId": "Member Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.evaluatedynamicmembershipresult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 93

{
  "value": {
    "@odata.type": "microsoft.graph.evaluateDynamicMembershipResult"
  }
}
```

