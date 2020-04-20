---
title: "Update planner"
description: "Update the properties of a planner object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update planner

Namespace: microsoft.graph

Update the properties of a planner object.

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
PATCH /groups/{groupsId}/planner
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/planner
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [plannerGroup](../resources/plannergroup.md) object.

The following table shows the properties that are required when you create the [plannerGroup](../resources/plannergroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerGroup](../resources/plannergroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_planner"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/groups/{groupsId}/planner
Content-Type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.plannerGroup"
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
  "@odata.type": "#microsoft.graph.plannerGroup",
  "id": "d1a39378-9378-d1a3-7893-a3d17893a3d1"
}
```

